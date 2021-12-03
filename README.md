This project is an example of the `TypeError: path__WEBPACK_IMPORTED_MODULE_16___default().join is not a function` issue with storybook 6.4.5 using webpack 5 and yarn3.

To reproduce:

```shell
yarn
yarn storybook
```

Open `http://localhost:6006` and check the console of your browser. You will see the following error:

```shell
Error reading preview.js:
TypeError: path__WEBPACK_IMPORTED_MODULE_16___default().join is not a function
    autoTitleFromSpecifier autoTitle.js:69
    autoTitle autoTitle.js:77
    addStoriesFromExports StoryStoreFacade.js:181
    getProjectAnnotations start.js:132
    getProjectAnnotations start.js:127
    _runResolutions index.js:217
    _runResolutions index.js:214
    then index.js:67
    getProjectAnnotationsOrRenderError PreviewWeb.js:140
    initialize PreviewWeb.js:118
    configure start.js:148
    configure index.js:21
    js generated-stories-entry.js:6
```
