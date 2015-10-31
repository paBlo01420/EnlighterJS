
Contribution
------------

EnlighterJS is OpenSource and managed on [GitHub](https://github.com/AndiDittrich/EnlighterJS) - if you like, you're welcome to contribute!
To simplify the release and quality control process, please follow these remarks:

### Notices ###
* Your commits/pull-request should only contain changes of the `Source/`, `Resources/TestcaseData` directories or the Examples located into the root directory - otherwise i have to merge the request manually
* **Do not change** the files located into the `Examples/` or `Build/` directory - they are automatically generated during the build-process using data from `Resources/TestcaseData`
* Related software packages like MooTools, Bootstrap, ANT-contrib are updated by the maintainer
* If you form a concept of larger project changes, please [discuss](https://github.com/AndiDittrich/EnlighterJS/issues) them with the contributors **before** implementing

### Adding a new Language ###
* First of all: take a look on other languages which are already available to learn about functions and coding styles
* To start with a new language please use the `LanguageDevelopment.phtml` workspace. It will automatically load `Source/Language/Template.mylang.js` (the startup file for your language development).
* Rename your language file `Template.mylang.js` to the **camel-cased** real language name - e.g. `Vhdl.js`
* Add detailed comments to each language rule!
* Keep the code as small as possible: e.g. use regex instead of long keyword lists
* In case your language is a superset of another one, please **extend** the origin language - do not copy the origin file
* Add an language testcase/demo to the `Resouces/TestcaseData` directory
* Finally create a [Pull Request on GitHub](https://help.github.com/articles/creating-a-pull-request/) - your changes will be reviewed and commonly added to the project