# storybook-config-log

```js
{
  "name": "preview",
  "mode": "development",
  "bail": false,
  "devtool": "cheap-module-source-map",
  "entry": [
    "toybox/storybook-config-log/node_modules/@storybook/core-client/dist/esm/globals/polyfills.js",
    "toybox/storybook-config-log/node_modules/@storybook/core-client/dist/esm/globals/globals.js",
    "toybox/storybook-config-log/.storybook/storybook-init-framework-entry.js",
    "toybox/storybook-config-log/node_modules/@storybook/addon-docs/dist/esm/frameworks/common/config.js-generated-other-entry.js",
    "toybox/storybook-config-log/node_modules/@storybook/addon-docs/dist/esm/frameworks/react/config.js-generated-other-entry.js",
    "toybox/storybook-config-log/node_modules/@storybook/addon-links/dist/esm/preset/addDecorator.js-generated-other-entry.js",
    "toybox/storybook-config-log/node_modules/@storybook/addon-actions/dist/esm/preset/addDecorator.js-generated-other-entry.js",
    "toybox/storybook-config-log/node_modules/@storybook/addon-actions/dist/esm/preset/addArgs.js-generated-other-entry.js",
    "toybox/storybook-config-log/node_modules/@storybook/addon-backgrounds/dist/esm/preset/addDecorator.js-generated-other-entry.js",
    "toybox/storybook-config-log/node_modules/@storybook/addon-backgrounds/dist/esm/preset/addParameter.js-generated-other-entry.js",
    "toybox/storybook-config-log/node_modules/@storybook/addon-measure/dist/esm/preset/preview.js-generated-other-entry.js",
    "toybox/storybook-config-log/node_modules/storybook-addon-outline/dist/esm/preset/addDecorator.js-generated-other-entry.js",
    "toybox/storybook-config-log/.storybook/preview.js-generated-config-entry.js",
    "toybox/storybook-config-log/.storybook/generated-stories-entry.js",
    "toybox/storybook-config-log/node_modules/webpack-hot-middleware/client.js?reload=true&quiet=false&noInfo=undefined"
  ],
  "output": {
    "path": "toybox/storybook-config-log/node_modules/.cache/storybook/public",
    "filename": "[name].iframe.bundle.js",
    "publicPath": ""
  },
  "watchOptions": { "ignored": {} },
  "plugins": [
    { "exclude": [{}] },
    {
      "_staticModules": {
        "toybox/storybook-config-log/.storybook/storybook-init-framework-entry.js": "import '@storybook/react';",
        "toybox/storybook-config-log/node_modules/@storybook/addon-docs/dist/esm/frameworks/common/config.js-generated-other-entry.js": "function ownKeys(object, enumerableOnly) { var keys = Object.keys(object); if (Object.getOwnPropertySymbols) { var symbols = Object.getOwnPropertySymbols(object); if (enumerableOnly) symbols = symbols.filter(function (sym) { return Object.getOwnPropertyDescriptor(object, sym).enumerable; }); keys.push.apply(keys, symbols); } return keys; }\n\nfunction _objectSpread(target) { for (var i = 1; i < arguments.length; i++) { var source = arguments[i] != null ? arguments[i] : {}; if (i % 2) { ownKeys(Object(source), true).forEach(function (key) { _defineProperty(target, key, source[key]); }); } else if (Object.getOwnPropertyDescriptors) { Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)); } else { ownKeys(Object(source)).forEach(function (key) { Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key)); }); } } return target; }\n\nfunction _defineProperty(obj, key, value) { if (key in obj) { Object.defineProperty(obj, key, { value: value, enumerable: true, configurable: true, writable: true }); } else { obj[key] = value; } return obj; }\n\n/* eslint-disable import/no-unresolved */\nimport { addDecorator, addParameters, addLoader, addArgsEnhancer, addArgTypesEnhancer, setGlobalRender } from 'toybox/storybook-config-log/node_modules/@storybook/client-api';\nimport { logger } from 'toybox/storybook-config-log/node_modules/@storybook/client-logger';\nimport * as config from 'toybox/storybook-config-log/node_modules/@storybook/addon-docs/dist/esm/frameworks/common/config.js';\nObject.keys(config).forEach(function (key) {\n  var value = config[key];\n\n  switch (key) {\n    case 'args':\n    case 'argTypes':\n      {\n        return logger.warn('Invalid args/argTypes in config, ignoring.', JSON.stringify(value));\n      }\n\n    case 'decorators':\n      {\n        return value.forEach(function (decorator) {\n          return addDecorator(decorator, false);\n        });\n      }\n\n    case 'loaders':\n      {\n        return value.forEach(function (loader) {\n          return addLoader(loader, false);\n        });\n      }\n\n    case 'parameters':\n      {\n        return addParameters(_objectSpread({}, value), false);\n      }\n\n    case 'argTypesEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgTypesEnhancer(enhancer);\n        });\n      }\n\n    case 'argsEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgsEnhancer(enhancer);\n        });\n      }\n\n    case 'render':\n      {\n        return setGlobalRender(value);\n      }\n\n    case 'globals':\n    case 'globalTypes':\n      {\n        var v = {};\n        v[key] = value;\n        return addParameters(v, false);\n      }\n\n    default:\n      {\n        // eslint-disable-next-line prefer-template\n        return console.log(key + ' was not supported :( !');\n      }\n  }\n});",
        "toybox/storybook-config-log/node_modules/@storybook/addon-docs/dist/esm/frameworks/react/config.js-generated-other-entry.js": "function ownKeys(object, enumerableOnly) { var keys = Object.keys(object); if (Object.getOwnPropertySymbols) { var symbols = Object.getOwnPropertySymbols(object); if (enumerableOnly) symbols = symbols.filter(function (sym) { return Object.getOwnPropertyDescriptor(object, sym).enumerable; }); keys.push.apply(keys, symbols); } return keys; }\n\nfunction _objectSpread(target) { for (var i = 1; i < arguments.length; i++) { var source = arguments[i] != null ? arguments[i] : {}; if (i % 2) { ownKeys(Object(source), true).forEach(function (key) { _defineProperty(target, key, source[key]); }); } else if (Object.getOwnPropertyDescriptors) { Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)); } else { ownKeys(Object(source)).forEach(function (key) { Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key)); }); } } return target; }\n\nfunction _defineProperty(obj, key, value) { if (key in obj) { Object.defineProperty(obj, key, { value: value, enumerable: true, configurable: true, writable: true }); } else { obj[key] = value; } return obj; }\n\n/* eslint-disable import/no-unresolved */\nimport { addDecorator, addParameters, addLoader, addArgsEnhancer, addArgTypesEnhancer, setGlobalRender } from 'toybox/storybook-config-log/node_modules/@storybook/client-api';\nimport { logger } from 'toybox/storybook-config-log/node_modules/@storybook/client-logger';\nimport * as config from 'toybox/storybook-config-log/node_modules/@storybook/addon-docs/dist/esm/frameworks/react/config.js';\nObject.keys(config).forEach(function (key) {\n  var value = config[key];\n\n  switch (key) {\n    case 'args':\n    case 'argTypes':\n      {\n        return logger.warn('Invalid args/argTypes in config, ignoring.', JSON.stringify(value));\n      }\n\n    case 'decorators':\n      {\n        return value.forEach(function (decorator) {\n          return addDecorator(decorator, false);\n        });\n      }\n\n    case 'loaders':\n      {\n        return value.forEach(function (loader) {\n          return addLoader(loader, false);\n        });\n      }\n\n    case 'parameters':\n      {\n        return addParameters(_objectSpread({}, value), false);\n      }\n\n    case 'argTypesEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgTypesEnhancer(enhancer);\n        });\n      }\n\n    case 'argsEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgsEnhancer(enhancer);\n        });\n      }\n\n    case 'render':\n      {\n        return setGlobalRender(value);\n      }\n\n    case 'globals':\n    case 'globalTypes':\n      {\n        var v = {};\n        v[key] = value;\n        return addParameters(v, false);\n      }\n\n    default:\n      {\n        // eslint-disable-next-line prefer-template\n        return console.log(key + ' was not supported :( !');\n      }\n  }\n});",
        "toybox/storybook-config-log/node_modules/@storybook/addon-links/dist/esm/preset/addDecorator.js-generated-other-entry.js": "function ownKeys(object, enumerableOnly) { var keys = Object.keys(object); if (Object.getOwnPropertySymbols) { var symbols = Object.getOwnPropertySymbols(object); if (enumerableOnly) symbols = symbols.filter(function (sym) { return Object.getOwnPropertyDescriptor(object, sym).enumerable; }); keys.push.apply(keys, symbols); } return keys; }\n\nfunction _objectSpread(target) { for (var i = 1; i < arguments.length; i++) { var source = arguments[i] != null ? arguments[i] : {}; if (i % 2) { ownKeys(Object(source), true).forEach(function (key) { _defineProperty(target, key, source[key]); }); } else if (Object.getOwnPropertyDescriptors) { Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)); } else { ownKeys(Object(source)).forEach(function (key) { Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key)); }); } } return target; }\n\nfunction _defineProperty(obj, key, value) { if (key in obj) { Object.defineProperty(obj, key, { value: value, enumerable: true, configurable: true, writable: true }); } else { obj[key] = value; } return obj; }\n\n/* eslint-disable import/no-unresolved */\nimport { addDecorator, addParameters, addLoader, addArgsEnhancer, addArgTypesEnhancer, setGlobalRender } from 'toybox/storybook-config-log/node_modules/@storybook/client-api';\nimport { logger } from 'toybox/storybook-config-log/node_modules/@storybook/client-logger';\nimport * as config from 'toybox/storybook-config-log/node_modules/@storybook/addon-links/dist/esm/preset/addDecorator.js';\nObject.keys(config).forEach(function (key) {\n  var value = config[key];\n\n  switch (key) {\n    case 'args':\n    case 'argTypes':\n      {\n        return logger.warn('Invalid args/argTypes in config, ignoring.', JSON.stringify(value));\n      }\n\n    case 'decorators':\n      {\n        return value.forEach(function (decorator) {\n          return addDecorator(decorator, false);\n        });\n      }\n\n    case 'loaders':\n      {\n        return value.forEach(function (loader) {\n          return addLoader(loader, false);\n        });\n      }\n\n    case 'parameters':\n      {\n        return addParameters(_objectSpread({}, value), false);\n      }\n\n    case 'argTypesEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgTypesEnhancer(enhancer);\n        });\n      }\n\n    case 'argsEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgsEnhancer(enhancer);\n        });\n      }\n\n    case 'render':\n      {\n        return setGlobalRender(value);\n      }\n\n    case 'globals':\n    case 'globalTypes':\n      {\n        var v = {};\n        v[key] = value;\n        return addParameters(v, false);\n      }\n\n    default:\n      {\n        // eslint-disable-next-line prefer-template\n        return console.log(key + ' was not supported :( !');\n      }\n  }\n});",
        "toybox/storybook-config-log/node_modules/@storybook/addon-actions/dist/esm/preset/addDecorator.js-generated-other-entry.js": "function ownKeys(object, enumerableOnly) { var keys = Object.keys(object); if (Object.getOwnPropertySymbols) { var symbols = Object.getOwnPropertySymbols(object); if (enumerableOnly) symbols = symbols.filter(function (sym) { return Object.getOwnPropertyDescriptor(object, sym).enumerable; }); keys.push.apply(keys, symbols); } return keys; }\n\nfunction _objectSpread(target) { for (var i = 1; i < arguments.length; i++) { var source = arguments[i] != null ? arguments[i] : {}; if (i % 2) { ownKeys(Object(source), true).forEach(function (key) { _defineProperty(target, key, source[key]); }); } else if (Object.getOwnPropertyDescriptors) { Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)); } else { ownKeys(Object(source)).forEach(function (key) { Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key)); }); } } return target; }\n\nfunction _defineProperty(obj, key, value) { if (key in obj) { Object.defineProperty(obj, key, { value: value, enumerable: true, configurable: true, writable: true }); } else { obj[key] = value; } return obj; }\n\n/* eslint-disable import/no-unresolved */\nimport { addDecorator, addParameters, addLoader, addArgsEnhancer, addArgTypesEnhancer, setGlobalRender } from 'toybox/storybook-config-log/node_modules/@storybook/client-api';\nimport { logger } from 'toybox/storybook-config-log/node_modules/@storybook/client-logger';\nimport * as config from 'toybox/storybook-config-log/node_modules/@storybook/addon-actions/dist/esm/preset/addDecorator.js';\nObject.keys(config).forEach(function (key) {\n  var value = config[key];\n\n  switch (key) {\n    case 'args':\n    case 'argTypes':\n      {\n        return logger.warn('Invalid args/argTypes in config, ignoring.', JSON.stringify(value));\n      }\n\n    case 'decorators':\n      {\n        return value.forEach(function (decorator) {\n          return addDecorator(decorator, false);\n        });\n      }\n\n    case 'loaders':\n      {\n        return value.forEach(function (loader) {\n          return addLoader(loader, false);\n        });\n      }\n\n    case 'parameters':\n      {\n        return addParameters(_objectSpread({}, value), false);\n      }\n\n    case 'argTypesEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgTypesEnhancer(enhancer);\n        });\n      }\n\n    case 'argsEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgsEnhancer(enhancer);\n        });\n      }\n\n    case 'render':\n      {\n        return setGlobalRender(value);\n      }\n\n    case 'globals':\n    case 'globalTypes':\n      {\n        var v = {};\n        v[key] = value;\n        return addParameters(v, false);\n      }\n\n    default:\n      {\n        // eslint-disable-next-line prefer-template\n        return console.log(key + ' was not supported :( !');\n      }\n  }\n});",
        "toybox/storybook-config-log/node_modules/@storybook/addon-actions/dist/esm/preset/addArgs.js-generated-other-entry.js": "function ownKeys(object, enumerableOnly) { var keys = Object.keys(object); if (Object.getOwnPropertySymbols) { var symbols = Object.getOwnPropertySymbols(object); if (enumerableOnly) symbols = symbols.filter(function (sym) { return Object.getOwnPropertyDescriptor(object, sym).enumerable; }); keys.push.apply(keys, symbols); } return keys; }\n\nfunction _objectSpread(target) { for (var i = 1; i < arguments.length; i++) { var source = arguments[i] != null ? arguments[i] : {}; if (i % 2) { ownKeys(Object(source), true).forEach(function (key) { _defineProperty(target, key, source[key]); }); } else if (Object.getOwnPropertyDescriptors) { Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)); } else { ownKeys(Object(source)).forEach(function (key) { Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key)); }); } } return target; }\n\nfunction _defineProperty(obj, key, value) { if (key in obj) { Object.defineProperty(obj, key, { value: value, enumerable: true, configurable: true, writable: true }); } else { obj[key] = value; } return obj; }\n\n/* eslint-disable import/no-unresolved */\nimport { addDecorator, addParameters, addLoader, addArgsEnhancer, addArgTypesEnhancer, setGlobalRender } from 'toybox/storybook-config-log/node_modules/@storybook/client-api';\nimport { logger } from 'toybox/storybook-config-log/node_modules/@storybook/client-logger';\nimport * as config from 'toybox/storybook-config-log/node_modules/@storybook/addon-actions/dist/esm/preset/addArgs.js';\nObject.keys(config).forEach(function (key) {\n  var value = config[key];\n\n  switch (key) {\n    case 'args':\n    case 'argTypes':\n      {\n        return logger.warn('Invalid args/argTypes in config, ignoring.', JSON.stringify(value));\n      }\n\n    case 'decorators':\n      {\n        return value.forEach(function (decorator) {\n          return addDecorator(decorator, false);\n        });\n      }\n\n    case 'loaders':\n      {\n        return value.forEach(function (loader) {\n          return addLoader(loader, false);\n        });\n      }\n\n    case 'parameters':\n      {\n        return addParameters(_objectSpread({}, value), false);\n      }\n\n    case 'argTypesEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgTypesEnhancer(enhancer);\n        });\n      }\n\n    case 'argsEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgsEnhancer(enhancer);\n        });\n      }\n\n    case 'render':\n      {\n        return setGlobalRender(value);\n      }\n\n    case 'globals':\n    case 'globalTypes':\n      {\n        var v = {};\n        v[key] = value;\n        return addParameters(v, false);\n      }\n\n    default:\n      {\n        // eslint-disable-next-line prefer-template\n        return console.log(key + ' was not supported :( !');\n      }\n  }\n});",
        "toybox/storybook-config-log/node_modules/@storybook/addon-backgrounds/dist/esm/preset/addDecorator.js-generated-other-entry.js": "function ownKeys(object, enumerableOnly) { var keys = Object.keys(object); if (Object.getOwnPropertySymbols) { var symbols = Object.getOwnPropertySymbols(object); if (enumerableOnly) symbols = symbols.filter(function (sym) { return Object.getOwnPropertyDescriptor(object, sym).enumerable; }); keys.push.apply(keys, symbols); } return keys; }\n\nfunction _objectSpread(target) { for (var i = 1; i < arguments.length; i++) { var source = arguments[i] != null ? arguments[i] : {}; if (i % 2) { ownKeys(Object(source), true).forEach(function (key) { _defineProperty(target, key, source[key]); }); } else if (Object.getOwnPropertyDescriptors) { Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)); } else { ownKeys(Object(source)).forEach(function (key) { Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key)); }); } } return target; }\n\nfunction _defineProperty(obj, key, value) { if (key in obj) { Object.defineProperty(obj, key, { value: value, enumerable: true, configurable: true, writable: true }); } else { obj[key] = value; } return obj; }\n\n/* eslint-disable import/no-unresolved */\nimport { addDecorator, addParameters, addLoader, addArgsEnhancer, addArgTypesEnhancer, setGlobalRender } from 'toybox/storybook-config-log/node_modules/@storybook/client-api';\nimport { logger } from 'toybox/storybook-config-log/node_modules/@storybook/client-logger';\nimport * as config from 'toybox/storybook-config-log/node_modules/@storybook/addon-backgrounds/dist/esm/preset/addDecorator.js';\nObject.keys(config).forEach(function (key) {\n  var value = config[key];\n\n  switch (key) {\n    case 'args':\n    case 'argTypes':\n      {\n        return logger.warn('Invalid args/argTypes in config, ignoring.', JSON.stringify(value));\n      }\n\n    case 'decorators':\n      {\n        return value.forEach(function (decorator) {\n          return addDecorator(decorator, false);\n        });\n      }\n\n    case 'loaders':\n      {\n        return value.forEach(function (loader) {\n          return addLoader(loader, false);\n        });\n      }\n\n    case 'parameters':\n      {\n        return addParameters(_objectSpread({}, value), false);\n      }\n\n    case 'argTypesEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgTypesEnhancer(enhancer);\n        });\n      }\n\n    case 'argsEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgsEnhancer(enhancer);\n        });\n      }\n\n    case 'render':\n      {\n        return setGlobalRender(value);\n      }\n\n    case 'globals':\n    case 'globalTypes':\n      {\n        var v = {};\n        v[key] = value;\n        return addParameters(v, false);\n      }\n\n    default:\n      {\n        // eslint-disable-next-line prefer-template\n        return console.log(key + ' was not supported :( !');\n      }\n  }\n});",
        "toybox/storybook-config-log/node_modules/@storybook/addon-backgrounds/dist/esm/preset/addParameter.js-generated-other-entry.js": "function ownKeys(object, enumerableOnly) { var keys = Object.keys(object); if (Object.getOwnPropertySymbols) { var symbols = Object.getOwnPropertySymbols(object); if (enumerableOnly) symbols = symbols.filter(function (sym) { return Object.getOwnPropertyDescriptor(object, sym).enumerable; }); keys.push.apply(keys, symbols); } return keys; }\n\nfunction _objectSpread(target) { for (var i = 1; i < arguments.length; i++) { var source = arguments[i] != null ? arguments[i] : {}; if (i % 2) { ownKeys(Object(source), true).forEach(function (key) { _defineProperty(target, key, source[key]); }); } else if (Object.getOwnPropertyDescriptors) { Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)); } else { ownKeys(Object(source)).forEach(function (key) { Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key)); }); } } return target; }\n\nfunction _defineProperty(obj, key, value) { if (key in obj) { Object.defineProperty(obj, key, { value: value, enumerable: true, configurable: true, writable: true }); } else { obj[key] = value; } return obj; }\n\n/* eslint-disable import/no-unresolved */\nimport { addDecorator, addParameters, addLoader, addArgsEnhancer, addArgTypesEnhancer, setGlobalRender } from 'toybox/storybook-config-log/node_modules/@storybook/client-api';\nimport { logger } from 'toybox/storybook-config-log/node_modules/@storybook/client-logger';\nimport * as config from 'toybox/storybook-config-log/node_modules/@storybook/addon-backgrounds/dist/esm/preset/addParameter.js';\nObject.keys(config).forEach(function (key) {\n  var value = config[key];\n\n  switch (key) {\n    case 'args':\n    case 'argTypes':\n      {\n        return logger.warn('Invalid args/argTypes in config, ignoring.', JSON.stringify(value));\n      }\n\n    case 'decorators':\n      {\n        return value.forEach(function (decorator) {\n          return addDecorator(decorator, false);\n        });\n      }\n\n    case 'loaders':\n      {\n        return value.forEach(function (loader) {\n          return addLoader(loader, false);\n        });\n      }\n\n    case 'parameters':\n      {\n        return addParameters(_objectSpread({}, value), false);\n      }\n\n    case 'argTypesEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgTypesEnhancer(enhancer);\n        });\n      }\n\n    case 'argsEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgsEnhancer(enhancer);\n        });\n      }\n\n    case 'render':\n      {\n        return setGlobalRender(value);\n      }\n\n    case 'globals':\n    case 'globalTypes':\n      {\n        var v = {};\n        v[key] = value;\n        return addParameters(v, false);\n      }\n\n    default:\n      {\n        // eslint-disable-next-line prefer-template\n        return console.log(key + ' was not supported :( !');\n      }\n  }\n});",
        "toybox/storybook-config-log/node_modules/@storybook/addon-measure/dist/esm/preset/preview.js-generated-other-entry.js": "function ownKeys(object, enumerableOnly) { var keys = Object.keys(object); if (Object.getOwnPropertySymbols) { var symbols = Object.getOwnPropertySymbols(object); if (enumerableOnly) symbols = symbols.filter(function (sym) { return Object.getOwnPropertyDescriptor(object, sym).enumerable; }); keys.push.apply(keys, symbols); } return keys; }\n\nfunction _objectSpread(target) { for (var i = 1; i < arguments.length; i++) { var source = arguments[i] != null ? arguments[i] : {}; if (i % 2) { ownKeys(Object(source), true).forEach(function (key) { _defineProperty(target, key, source[key]); }); } else if (Object.getOwnPropertyDescriptors) { Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)); } else { ownKeys(Object(source)).forEach(function (key) { Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key)); }); } } return target; }\n\nfunction _defineProperty(obj, key, value) { if (key in obj) { Object.defineProperty(obj, key, { value: value, enumerable: true, configurable: true, writable: true }); } else { obj[key] = value; } return obj; }\n\n/* eslint-disable import/no-unresolved */\nimport { addDecorator, addParameters, addLoader, addArgsEnhancer, addArgTypesEnhancer, setGlobalRender } from 'toybox/storybook-config-log/node_modules/@storybook/client-api';\nimport { logger } from 'toybox/storybook-config-log/node_modules/@storybook/client-logger';\nimport * as config from 'toybox/storybook-config-log/node_modules/@storybook/addon-measure/dist/esm/preset/preview.js';\nObject.keys(config).forEach(function (key) {\n  var value = config[key];\n\n  switch (key) {\n    case 'args':\n    case 'argTypes':\n      {\n        return logger.warn('Invalid args/argTypes in config, ignoring.', JSON.stringify(value));\n      }\n\n    case 'decorators':\n      {\n        return value.forEach(function (decorator) {\n          return addDecorator(decorator, false);\n        });\n      }\n\n    case 'loaders':\n      {\n        return value.forEach(function (loader) {\n          return addLoader(loader, false);\n        });\n      }\n\n    case 'parameters':\n      {\n        return addParameters(_objectSpread({}, value), false);\n      }\n\n    case 'argTypesEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgTypesEnhancer(enhancer);\n        });\n      }\n\n    case 'argsEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgsEnhancer(enhancer);\n        });\n      }\n\n    case 'render':\n      {\n        return setGlobalRender(value);\n      }\n\n    case 'globals':\n    case 'globalTypes':\n      {\n        var v = {};\n        v[key] = value;\n        return addParameters(v, false);\n      }\n\n    default:\n      {\n        // eslint-disable-next-line prefer-template\n        return console.log(key + ' was not supported :( !');\n      }\n  }\n});",
        "toybox/storybook-config-log/node_modules/storybook-addon-outline/dist/esm/preset/addDecorator.js-generated-other-entry.js": "function ownKeys(object, enumerableOnly) { var keys = Object.keys(object); if (Object.getOwnPropertySymbols) { var symbols = Object.getOwnPropertySymbols(object); if (enumerableOnly) symbols = symbols.filter(function (sym) { return Object.getOwnPropertyDescriptor(object, sym).enumerable; }); keys.push.apply(keys, symbols); } return keys; }\n\nfunction _objectSpread(target) { for (var i = 1; i < arguments.length; i++) { var source = arguments[i] != null ? arguments[i] : {}; if (i % 2) { ownKeys(Object(source), true).forEach(function (key) { _defineProperty(target, key, source[key]); }); } else if (Object.getOwnPropertyDescriptors) { Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)); } else { ownKeys(Object(source)).forEach(function (key) { Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key)); }); } } return target; }\n\nfunction _defineProperty(obj, key, value) { if (key in obj) { Object.defineProperty(obj, key, { value: value, enumerable: true, configurable: true, writable: true }); } else { obj[key] = value; } return obj; }\n\n/* eslint-disable import/no-unresolved */\nimport { addDecorator, addParameters, addLoader, addArgsEnhancer, addArgTypesEnhancer, setGlobalRender } from 'toybox/storybook-config-log/node_modules/@storybook/client-api';\nimport { logger } from 'toybox/storybook-config-log/node_modules/@storybook/client-logger';\nimport * as config from 'toybox/storybook-config-log/node_modules/storybook-addon-outline/dist/esm/preset/addDecorator.js';\nObject.keys(config).forEach(function (key) {\n  var value = config[key];\n\n  switch (key) {\n    case 'args':\n    case 'argTypes':\n      {\n        return logger.warn('Invalid args/argTypes in config, ignoring.', JSON.stringify(value));\n      }\n\n    case 'decorators':\n      {\n        return value.forEach(function (decorator) {\n          return addDecorator(decorator, false);\n        });\n      }\n\n    case 'loaders':\n      {\n        return value.forEach(function (loader) {\n          return addLoader(loader, false);\n        });\n      }\n\n    case 'parameters':\n      {\n        return addParameters(_objectSpread({}, value), false);\n      }\n\n    case 'argTypesEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgTypesEnhancer(enhancer);\n        });\n      }\n\n    case 'argsEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgsEnhancer(enhancer);\n        });\n      }\n\n    case 'render':\n      {\n        return setGlobalRender(value);\n      }\n\n    case 'globals':\n    case 'globalTypes':\n      {\n        var v = {};\n        v[key] = value;\n        return addParameters(v, false);\n      }\n\n    default:\n      {\n        // eslint-disable-next-line prefer-template\n        return console.log(key + ' was not supported :( !');\n      }\n  }\n});",
        "toybox/storybook-config-log/.storybook/preview.js-generated-config-entry.js": "function ownKeys(object, enumerableOnly) { var keys = Object.keys(object); if (Object.getOwnPropertySymbols) { var symbols = Object.getOwnPropertySymbols(object); if (enumerableOnly) symbols = symbols.filter(function (sym) { return Object.getOwnPropertyDescriptor(object, sym).enumerable; }); keys.push.apply(keys, symbols); } return keys; }\n\nfunction _objectSpread(target) { for (var i = 1; i < arguments.length; i++) { var source = arguments[i] != null ? arguments[i] : {}; if (i % 2) { ownKeys(Object(source), true).forEach(function (key) { _defineProperty(target, key, source[key]); }); } else if (Object.getOwnPropertyDescriptors) { Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)); } else { ownKeys(Object(source)).forEach(function (key) { Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key)); }); } } return target; }\n\nfunction _defineProperty(obj, key, value) { if (key in obj) { Object.defineProperty(obj, key, { value: value, enumerable: true, configurable: true, writable: true }); } else { obj[key] = value; } return obj; }\n\n/* eslint-disable import/no-unresolved */\nimport { addDecorator, addParameters, addLoader, addArgsEnhancer, addArgTypesEnhancer, setGlobalRender } from 'toybox/storybook-config-log/node_modules/@storybook/client-api';\nimport { logger } from 'toybox/storybook-config-log/node_modules/@storybook/client-logger';\nimport * as config from 'toybox/storybook-config-log/.storybook/preview.js';\nObject.keys(config).forEach(function (key) {\n  var value = config[key];\n\n  switch (key) {\n    case 'args':\n    case 'argTypes':\n      {\n        return logger.warn('Invalid args/argTypes in config, ignoring.', JSON.stringify(value));\n      }\n\n    case 'decorators':\n      {\n        return value.forEach(function (decorator) {\n          return addDecorator(decorator, false);\n        });\n      }\n\n    case 'loaders':\n      {\n        return value.forEach(function (loader) {\n          return addLoader(loader, false);\n        });\n      }\n\n    case 'parameters':\n      {\n        return addParameters(_objectSpread({}, value), false);\n      }\n\n    case 'argTypesEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgTypesEnhancer(enhancer);\n        });\n      }\n\n    case 'argsEnhancers':\n      {\n        return value.forEach(function (enhancer) {\n          return addArgsEnhancer(enhancer);\n        });\n      }\n\n    case 'render':\n      {\n        return setGlobalRender(value);\n      }\n\n    case 'globals':\n    case 'globalTypes':\n      {\n        var v = {};\n        v[key] = value;\n        return addParameters(v, false);\n      }\n\n    default:\n      {\n        // eslint-disable-next-line prefer-template\n        return console.log(key + ' was not supported :( !');\n      }\n  }\n});",
        "toybox/storybook-config-log/.storybook/generated-stories-entry.js": "\"use strict\";\n\nvar _frameworkImportPath = require(\"@storybook/react\");\n\n/* eslint-disable import/no-unresolved */\n(0, _frameworkImportPath.configure)([require.context('../stories', true, /^\\.(?:(?:^|\\/|(?:(?:(?!(?:^|\\/)\\.).)*?)\\/)(?!\\.)(?=.)[^/]*?\\.stories\\.mdx)$/),require.context('../stories', true, /^\\.(?:(?:^|\\/|(?:(?:(?!(?:^|\\/)\\.).)*?)\\/)(?!\\.)(?=.)[^/]*?\\.stories\\.(js|jsx|ts|tsx))$/)], module, false);"
      }
    },
    {
      "options": {
        "template": "toybox/storybook-config-log/node_modules/@storybook/core-common/dist/cjs/templates/index.ejs",
        "templateContent": false,
        "filename": "iframe.html",
        "publicPath": "auto",
        "hash": false,
        "inject": false,
        "scriptLoading": "blocking",
        "compile": true,
        "favicon": false,
        "minify": {
          "collapseWhitespace": true,
          "removeComments": true,
          "removeRedundantAttributes": true,
          "removeScriptTypeAttributes": false,
          "removeStyleLinkTypeAttributes": true,
          "useShortDoctype": true
        },
        "cache": true,
        "showErrors": true,
        "chunks": "all",
        "excludeChunks": [],
        "chunksSortMode": "none",
        "meta": {},
        "base": false,
        "title": "Webpack App",
        "xhtml": false,
        "alwaysWriteToDisk": true
      },
      "version": 4
    },
    {
      "definitions": {
        "process.env": {
          "NODE_ENV": "\"development\"",
          "NODE_PATH": "[]",
          "STORYBOOK": "\"true\"",
          "PUBLIC_URL": "\".\""
        },
        "NODE_ENV": "\"development\""
      }
    },
    {
      "nodeModulesPath": "toybox/storybook-config-log/node_modules"
    },
    { "options": {}, "fullBuildTimeout": 200, "requestTimeout": 10000 },
    {
      "options": {},
      "logger": {},
      "pathCache": {},
      "fsOperations": 0,
      "primed": false
    },
    {
      "profile": false,
      "modulesCount": 500,
      "showEntries": false,
      "showModules": true,
      "showActiveModules": true
    },
    { "definitions": {} },
    {}
  ],
  "module": {
    "rules": [
      {
        "test": {},
        "use": [
          {
            "loader": "toybox/storybook-config-log/node_modules/babel-loader/lib/index.js",
            "options": {
              "cacheDirectory": "toybox/storybook-config-log/node_modules/.cache/storybook/babel",
              "sourceType": "unambiguous",
              "presets": [
                [
                  "toybox/storybook-config-log/node_modules/@babel/preset-env/lib/index.js",
                  { "shippedProposals": true, "loose": true }
                ],
                "toybox/storybook-config-log/node_modules/@babel/preset-typescript/lib/index.js",
                [
                  "toybox/storybook-config-log/node_modules/@babel/preset-react/lib/index.js",
                  { "runtime": "automatic" }
                ],
                "toybox/storybook-config-log/node_modules/@babel/preset-flow/lib/index.js"
              ],
              "plugins": [
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-shorthand-properties/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-block-scoping/lib/index.js",
                [
                  "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-decorators/lib/index.js",
                  { "legacy": true }
                ],
                [
                  "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-class-properties/lib/index.js",
                  { "loose": true }
                ],
                [
                  "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-private-methods/lib/index.js",
                  { "loose": true }
                ],
                "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-export-default-from/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-syntax-dynamic-import/lib/index.js",
                [
                  "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-object-rest-spread/lib/index.js",
                  { "loose": true, "useBuiltIns": true }
                ],
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-classes/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-arrow-functions/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-parameters/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-destructuring/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-spread/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-for-of/lib/index.js",
                "toybox/storybook-config-log/node_modules/@storybook/core-common/node_modules/babel-plugin-macros/dist/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-optional-chaining/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-nullish-coalescing-operator/lib/index.js",
                [
                  "toybox/storybook-config-log/node_modules/@storybook/core-common/node_modules/babel-plugin-polyfill-corejs3/lib/index.js",
                  {
                    "method": "usage-global",
                    "absoluteImports": "toybox/storybook-config-log/node_modules/core-js/index.js",
                    "version": "3.17.1"
                  }
                ],
                "toybox/storybook-config-log/node_modules/babel-plugin-add-react-displayname/index.js"
              ],
              "overrides": [
                {
                  "test": {},
                  "plugins": [
                    [
                      "toybox/storybook-config-log/node_modules/babel-plugin-react-docgen/lib/index.js",
                      { "DOC_GEN_COLLECTION_NAME": "STORYBOOK_REACT_CLASSES" }
                    ]
                  ]
                }
              ]
            }
          }
        ],
        "include": [
          "toybox/storybook-config-log"
        ],
        "exclude": {}
      },
      {
        "test": {},
        "use": [
          {
            "loader": "toybox/storybook-config-log/node_modules/babel-loader/lib/index.js",
            "options": {
              "sourceType": "unambiguous",
              "presets": [
                [
                  "toybox/storybook-config-log/node_modules/@babel/preset-env/lib/index.js",
                  {
                    "shippedProposals": true,
                    "modules": false,
                    "loose": true,
                    "targets": "defaults"
                  }
                ],
                "toybox/storybook-config-log/node_modules/@babel/preset-react/lib/index.js"
              ],
              "plugins": [
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-shorthand-properties/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-block-scoping/lib/index.js",
                [
                  "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-decorators/lib/index.js",
                  { "legacy": true }
                ],
                [
                  "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-class-properties/lib/index.js",
                  { "loose": true }
                ],
                [
                  "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-private-methods/lib/index.js",
                  { "loose": true }
                ],
                "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-export-default-from/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-syntax-dynamic-import/lib/index.js",
                [
                  "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-object-rest-spread/lib/index.js",
                  { "loose": true, "useBuiltIns": true }
                ],
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-classes/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-arrow-functions/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-parameters/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-destructuring/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-spread/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-for-of/lib/index.js",
                "toybox/storybook-config-log/node_modules/@storybook/core-common/node_modules/babel-plugin-macros/dist/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-optional-chaining/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-nullish-coalescing-operator/lib/index.js",
                [
                  "toybox/storybook-config-log/node_modules/@storybook/core-common/node_modules/babel-plugin-polyfill-corejs3/lib/index.js",
                  {
                    "method": "usage-global",
                    "absoluteImports": "toybox/storybook-config-log/node_modules/core-js/index.js",
                    "version": "3.17.1"
                  }
                ]
              ]
            }
          }
        ]
      },
      {
        "test": {},
        "use": [
          {
            "loader": "toybox/storybook-config-log/node_modules/raw-loader/dist/cjs.js"
          }
        ]
      },
      {
        "test": {},
        "include": {},
        "use": [
          {
            "loader": "toybox/storybook-config-log/node_modules/babel-loader/lib/index.js",
            "options": {
              "presets": [
                [
                  "toybox/storybook-config-log/node_modules/@babel/preset-env/lib/index.js",
                  { "modules": "commonjs" }
                ]
              ]
            }
          }
        ]
      },
      {
        "test": {},
        "use": [
          {
            "loader": "toybox/storybook-config-log/node_modules/babel-loader/lib/index.js",
            "options": {
              "babelrc": false,
              "configFile": false,
              "cacheDirectory": "toybox/storybook-config-log/node_modules/.cache/storybook/babel",
              "sourceType": "unambiguous",
              "presets": [
                [
                  "toybox/storybook-config-log/node_modules/@babel/preset-env/lib/index.js",
                  { "shippedProposals": true, "loose": true }
                ],
                "toybox/storybook-config-log/node_modules/@babel/preset-typescript/lib/index.js",
                [
                  "toybox/storybook-config-log/node_modules/@babel/preset-react/lib/index.js",
                  { "runtime": "automatic" }
                ],
                "toybox/storybook-config-log/node_modules/@babel/preset-flow/lib/index.js"
              ],
              "plugins": [
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-shorthand-properties/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-block-scoping/lib/index.js",
                [
                  "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-decorators/lib/index.js",
                  { "legacy": true }
                ],
                [
                  "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-class-properties/lib/index.js",
                  { "loose": true }
                ],
                [
                  "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-private-methods/lib/index.js",
                  { "loose": true }
                ],
                "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-export-default-from/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-syntax-dynamic-import/lib/index.js",
                [
                  "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-object-rest-spread/lib/index.js",
                  { "loose": true, "useBuiltIns": true }
                ],
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-classes/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-arrow-functions/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-parameters/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-destructuring/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-spread/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-for-of/lib/index.js",
                "toybox/storybook-config-log/node_modules/@storybook/core-common/node_modules/babel-plugin-macros/dist/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-optional-chaining/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-nullish-coalescing-operator/lib/index.js",
                [
                  "toybox/storybook-config-log/node_modules/@storybook/core-common/node_modules/babel-plugin-polyfill-corejs3/lib/index.js",
                  {
                    "method": "usage-global",
                    "absoluteImports": "toybox/storybook-config-log/node_modules/core-js/index.js",
                    "version": "3.17.1"
                  }
                ],
                "toybox/storybook-config-log/node_modules/babel-plugin-add-react-displayname/index.js",
                [
                  "toybox/storybook-config-log/node_modules/@babel/plugin-transform-react-jsx/lib/index.js",
                  {
                    "pragma": "React.createElement",
                    "pragmaFrag": "React.Fragment"
                  }
                ]
              ],
              "overrides": [
                {
                  "test": {},
                  "plugins": [
                    [
                      "toybox/storybook-config-log/node_modules/babel-plugin-react-docgen/lib/index.js",
                      { "DOC_GEN_COLLECTION_NAME": "STORYBOOK_REACT_CLASSES" }
                    ]
                  ]
                }
              ]
            }
          },
          {
            "loader": "toybox/storybook-config-log/node_modules/@mdx-js/loader/index.js",
            "options": { "compilers": [null], "remarkPlugins": [null, null] }
          }
        ]
      },
      {
        "test": {},
        "exclude": {},
        "use": [
          {
            "loader": "toybox/storybook-config-log/node_modules/babel-loader/lib/index.js",
            "options": {
              "babelrc": false,
              "configFile": false,
              "cacheDirectory": "toybox/storybook-config-log/node_modules/.cache/storybook/babel",
              "sourceType": "unambiguous",
              "presets": [
                [
                  "toybox/storybook-config-log/node_modules/@babel/preset-env/lib/index.js",
                  { "shippedProposals": true, "loose": true }
                ],
                "toybox/storybook-config-log/node_modules/@babel/preset-typescript/lib/index.js",
                [
                  "toybox/storybook-config-log/node_modules/@babel/preset-react/lib/index.js",
                  { "runtime": "automatic" }
                ],
                "toybox/storybook-config-log/node_modules/@babel/preset-flow/lib/index.js"
              ],
              "plugins": [
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-shorthand-properties/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-block-scoping/lib/index.js",
                [
                  "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-decorators/lib/index.js",
                  { "legacy": true }
                ],
                [
                  "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-class-properties/lib/index.js",
                  { "loose": true }
                ],
                [
                  "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-private-methods/lib/index.js",
                  { "loose": true }
                ],
                "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-export-default-from/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-syntax-dynamic-import/lib/index.js",
                [
                  "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-object-rest-spread/lib/index.js",
                  { "loose": true, "useBuiltIns": true }
                ],
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-classes/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-arrow-functions/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-parameters/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-destructuring/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-spread/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-transform-for-of/lib/index.js",
                "toybox/storybook-config-log/node_modules/@storybook/core-common/node_modules/babel-plugin-macros/dist/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-optional-chaining/lib/index.js",
                "toybox/storybook-config-log/node_modules/@babel/plugin-proposal-nullish-coalescing-operator/lib/index.js",
                [
                  "toybox/storybook-config-log/node_modules/@storybook/core-common/node_modules/babel-plugin-polyfill-corejs3/lib/index.js",
                  {
                    "method": "usage-global",
                    "absoluteImports": "toybox/storybook-config-log/node_modules/core-js/index.js",
                    "version": "3.17.1"
                  }
                ],
                "toybox/storybook-config-log/node_modules/babel-plugin-add-react-displayname/index.js",
                [
                  "toybox/storybook-config-log/node_modules/@babel/plugin-transform-react-jsx/lib/index.js",
                  {
                    "pragma": "React.createElement",
                    "pragmaFrag": "React.Fragment"
                  }
                ]
              ],
              "overrides": [
                {
                  "test": {},
                  "plugins": [
                    [
                      "toybox/storybook-config-log/node_modules/babel-plugin-react-docgen/lib/index.js",
                      { "DOC_GEN_COLLECTION_NAME": "STORYBOOK_REACT_CLASSES" }
                    ]
                  ]
                }
              ]
            }
          },
          {
            "loader": "toybox/storybook-config-log/node_modules/@mdx-js/loader/index.js",
            "options": { "remarkPlugins": [null, null] }
          }
        ]
      },
      {
        "test": {},
        "loader": "toybox/storybook-config-log/node_modules/@storybook/source-loader/dist/cjs/index.js",
        "options": {
          "injectStoryParameters": true,
          "inspectLocalDependencies": true
        },
        "enforce": "pre"
      },
      {
        "test": {},
        "sideEffects": true,
        "use": [
          "toybox/storybook-config-log/node_modules/style-loader/dist/cjs.js",
          {
            "loader": "toybox/storybook-config-log/node_modules/css-loader/dist/cjs.js",
            "options": { "importLoaders": 1 }
          },
          {
            "loader": "toybox/storybook-config-log/node_modules/postcss-loader/dist/cjs.js",
            "options": {
              "postcssOptions": { "config": false, "plugins": [null, null] }
            }
          }
        ]
      },
      {
        "test": {},
        "loader": "toybox/storybook-config-log/node_modules/file-loader/dist/cjs.js",
        "options": {
          "esModule": false,
          "name": "static/media/[path][name].[ext]"
        }
      },
      {
        "test": {},
        "loader": "toybox/storybook-config-log/node_modules/url-loader/dist/cjs.js",
        "options": { "limit": 10000, "name": "static/media/[path][name].[ext]" }
      }
    ]
  },
  "resolve": {
    "extensions": [".mjs", ".js", ".jsx", ".ts", ".tsx", ".json", ".cjs"],
    "modules": ["node_modules"],
    "mainFields": ["browser", "module", "main"],
    "alias": {
      "@emotion/core": "toybox/storybook-config-log/node_modules/@emotion/core",
      "@emotion/styled": "toybox/storybook-config-log/node_modules/@emotion/styled",
      "emotion-theming": "toybox/storybook-config-log/node_modules/emotion-theming",
      "@storybook/addons": "toybox/storybook-config-log/node_modules/@storybook/addons",
      "@storybook/api": "toybox/storybook-config-log/node_modules/@storybook/api",
      "@storybook/channels": "toybox/storybook-config-log/node_modules/@storybook/channels",
      "@storybook/channel-postmessage": "toybox/storybook-config-log/node_modules/@storybook/channel-postmessage",
      "@storybook/components": "toybox/storybook-config-log/node_modules/@storybook/components",
      "@storybook/core-events": "toybox/storybook-config-log/node_modules/@storybook/core-events",
      "@storybook/router": "toybox/storybook-config-log/node_modules/@storybook/router",
      "@storybook/theming": "toybox/storybook-config-log/node_modules/@storybook/theming",
      "@storybook/semver": "toybox/storybook-config-log/node_modules/@storybook/semver",
      "@storybook/client-api": "toybox/storybook-config-log/node_modules/@storybook/client-api",
      "@storybook/client-logger": "toybox/storybook-config-log/node_modules/@storybook/client-logger",
      "react": "toybox/storybook-config-log/node_modules/react",
      "react-dom": "toybox/storybook-config-log/node_modules/react-dom"
    },
    "plugins": [{ "topLevelLoader": {} }]
  },
  "resolveLoader": { "plugins": [{}] },
  "optimization": {
    "splitChunks": { "chunks": "all" },
    "runtimeChunk": true,
    "sideEffects": true,
    "usedExports": true,
    "minimizer": []
  },
  "performance": { "hints": false }
}

```
