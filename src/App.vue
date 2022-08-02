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
</script>

<template>

  <NavBar></NavBar>
  <HeroPage></HeroPage>
  <ProductSection></ProductSection>
  <TeamSection></TeamSection>
  <AboutSection></AboutSection>
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
