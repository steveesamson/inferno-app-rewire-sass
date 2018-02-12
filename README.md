# Deprecated

This package has been deprecated as Create Inferno App has [documented instructions](https://github.com/facebookincubator/create-react-app/blob/master/packages/react-scripts/template/README.md#adding-a-css-preprocessor-sass-less-etc) on how to setup without ejecting.

# Rewire create-inferno-app to use SASS!

# Install

```bash
$ npm install --save inferno-app-rewire-sass
```

# Add it to your project

* [Rewire your app](https://github.com/steveesamson/inferno-app-rewired#how-to-rewire-your-create-inferno-app-project) than modify `config-overrides.js`

```javascript
const rewireSass = require('inferno-app-rewire-sass');

/* config-overrides.js */
module.exports = function override(config, env) {
  config = rewireSass(config, env);
  return config;
}
```
