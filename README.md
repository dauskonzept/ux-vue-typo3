TYPO3 Extension "typo3-ux-vue"
=================================

## What does it do?
Render Vue components directly in Fluid template

This Extensions enables you to render Vue Components directly in Fluid templates.
It acts as an integration for symfony/ux-vue into TYPO3.

## Prerequsites
To use this extension you have to use Webpack Encore for bundling for frontend assets.

Before you start, make sure you have [Symfony UX configured in your project](https://symfony.com/doc/current/frontend/ux.html).

## Installation
The recommended way to install the extension is by
using [Composer](https://getcomposer.org/). In your Composer based TYPO3 project
root, just run:
<pre>composer require svenpetersen/typo3-ux-vue</pre>

## Setup
Follow the [Symfony UX Vue.js official documentation](https://symfony.com/bundles/ux-vue/current/index.html)

## Compatibility
@todo

## Usage
In any fluid template: Just register the Namespace and use the provided ViewHelper to render your component:

    <html xmlns:ux="http://typo3.org/ns/SvenPetersen/UX/Vue/ViewHelpers">
        <div {ux:vueComponent(name:'MyComponent',props:"{'name':'John Doe'}")}></div>
    </html>

## Contributing

Please refer to the [contributing](CONTRIBUTING.md) document included in this
repository.
