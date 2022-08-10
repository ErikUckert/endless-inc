# Website for Endless Industries

## How to push new version to github pages

1. build everything with
    ```
    $ npm run build
    ```
2. add dist folder
    ```
    $ git add dist -f
    ```
3. Commit
    ```
    $ git commit -m "Adding dist"
    ```
4. Push to subtree for gh-pages
    ```
    $ git subtree push --prefix dist origin gh-pages
    ```