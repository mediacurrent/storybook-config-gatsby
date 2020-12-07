# storybook-config-gatsby

The webpack config for using Storybook with Gatsby on Mediacurrent projects.

## Usage 
In your `.storybook/webpack.config.js` file, put the following:

```
const sharedConfig = require('@mediacurrent/storybook-config-gatsby')
module.exports = ({ config }) => {
  const newConfig = sharedConfig(config);
  // Overrides here like:
  // newConfig.module.rules = foo
  return newConfig;
};

```