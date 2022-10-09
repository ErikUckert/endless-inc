<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import HelloWorld from './components/HelloWorld.vue'
import NavBar from './components/NavBar.vue'
import HeroPage from './components/HeroPage.vue'
import Footy from './components/Footy.vue'
import TeamSection from './components/TeamSection.vue'
import AboutSection from './components/AboutSection.vue'
import ProductSection from './components/ProductSection.vue'
import ContactSection from './components/ContactSection.vue'
import ContactModal from './components/ContactModal.vue'

const showModal = false
const showContactSection = true
const contactSectionId = 'contact'
const contactModalId = 'contactModal'

function scroll(id) {  
    document.getElementById(id).scrollIntoView({
      behavior: "smooth",
      block: "center"
    })
  }
</script>


<template>

  <NavBar></NavBar>
  <HeroPage></HeroPage>
  <AboutSection></AboutSection>
  <ProductSection></ProductSection>
  <ContactModal
    id="contactModal"
    v-bind:showModal="showModal"
    v-bind:showContactSection="showContactSection" 
    @close="showModal = false, 
    showContactSection = true,
    scroll(contactSectionId)"
    >
  </ContactModal>
  <ContactSection 
    id="contact"
    v-bind:showModal="showModal" 
    v-bind:showContactSection="showContactSection"
    @show="showModal = true, 
    showContactSection = false,
    scroll(contactModalId)">
  </ContactSection>
  <TeamSection></TeamSection>
  <Footy></Footy>
</template>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>