# storybook-config-gatsby

The webpack config for using Storybook with Gatsby on Mediacurrent projects.

## Install
`npm install --save-dev @mediacurrent/storybook-config-gatsby`

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