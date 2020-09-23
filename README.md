# webpack-boilerplate

Webpack boilerplate

#### Tools

- Pug
- Sass
- ES6 Transpile

## File Structure

```
.
+-- public/ (Deploy this directory)
    +-- index.html
    +-- second.html
        +-- assets/
            +-- images/
            +-- javascripts/
            +-- stylesheets/
        +-- posts/
            1.html
+-- src/
    +-- main.js (Import js and css you want to pick up)
    +-- assets/
        +-- images
        +-- javascripts
        +-- stylesheets
    +-- pages/ (Picked up by HtmlWebpackPlugin)
        +-- index.pug
        +-- second.pug
        +-- posts/
            +-- 1.html
+-- tsconfig.json
+-- webpack.config.js
```

## Let's Get Started

```bash
# Start development
$ npm start

# To Emit files into /public
# Use this as a build command
$ npm run build

# Use this as a build command(mode=development)
$ npm run build:dev
```

## Add New HTML Page

- Add a `.pug` file in `pages/`.
- Add `'your/path/to/page.html'` as `htmlPlugin`'s argument.
- Restart webpack (npm start).

## Add New CSS / JS

- Add a `.js` or `.scss/.sass` file in `/src/assets`.
- Import them in /`src/main.js` file.
- Restart webpack (npm start).

`/src/main.js` is an entry point to pick everything up in this project.
You can see the setting in webpack.config.js.

## Update Packages

https://github.com/tjunnone/npm-check-updates

```
$ npm install -g npm-check-updates

# To check latest versions
$ ncu

# To Upgrade everything to the latest version
$ ncu -u
```
