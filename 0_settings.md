# Development environment tools settings

* VSCode
* Coding standard - airbnb javascript coding guidelines
* Enforce coding standard - Linter - Choose Airbnb
  * `npm install eslint --save-dev`
  * `npm init @eslint/config`
  * Select the option: **To check syntax and find problems**  
  * Save Settings as JSON - `.eslintrc.json`
* Run ESLint - `npx eslint app.js`
* Fix ESlint errors that are possible to fix automatically - `npx eslint app.js --fix`
* Code Formatter - To style code consistently
  * Install prettier extension <https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode>
  * `npm install -save-dev eslint-config-prettier`
  * Edit - `.eslintrc.json`

    ```json
    "extends": [
            "airbnb-base",
            "prettier",
        ],
    ```

  * Dev enviroment setting is done!
