<p align="center"><img src="https://laravel.com/assets/img/components/logo-laravel.svg"></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/license.svg" alt="License"></a>
</p>

## Instalation

Laravel Mix
The only remaining step is to install Laravel Mix. Within a fresh installation of Laravel, you'll find a  package.json file in the root of your directory structure. The default package.json file includes everything you need to get started. Think of this like your composer.json file, except it defines Node dependencies instead of PHP. You may install the dependencies it references by running:
```js
npm install
```

If you are developing on a Windows system or you are running your VM on a Windows host system, you may need to run the npm install command with the --no-bin-links switch enabled:
```js
npm install --no-bin-links
```
# BrowserSync

```js
mix.browserSync('my-site.dev');
```

BrowserSync will automatically monitor your files for changes, and insert your changes into the browser - all without requiring a manual refresh. You may enable support by calling the `mix.browserSync()` method, like so:

```js
mix.browserSync('my-domain.dev');

// Or:

// https://browsersync.io/docs/options/
mix.browserSync({
    proxy: 'my-domain.dev'
})
```

You may pass either a string (proxy) or object (BrowserSync settings) to this method. The domain name you declare as your proxy is vital. This will proxy output from webpack Dev Server through BrowserSync.

Now, boot up the dev server (`npm run watch`), and you're all set go!

# Watching Assets For Changes

The npm run watch command will continue running in your terminal and watch all relevant files for changes. Webpack will then automatically recompile your assets when it detects a change:
```js
npm run watch
```

