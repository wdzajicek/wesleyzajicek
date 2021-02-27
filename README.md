# wesleyzajicek.com

#### Jekyll + Webpack + Babel + Gulp + Sass + Autoprefixer + imagemin + BrowserSync + ...

-----

<br>

## Requirements

 - Jekyll & Bundler:
```shell
$ gem install jekyll
$ gem install bundler
```
 - Nodejs/npm - We use NVM (Node Version Manager): https://github.com/creationix/nvm
   - .nvmrc file in this repo will make NVM use Node v8.9.4 (to avoid compatibility issues)
   - Or, if you must - Use the Nodejs installer: https://nodejs.org/

 - Gulp:
```shell
$ npm install --global gulp-cli # mac users may need sudo
```

-----

<br>

## Installation

```bash
git clone git@github.com:wdzajicek/wesleyzajicek.git
cd wesleyzajicek
npm i && bundle i
```

-----

<br>

## Development

```shell
$ npm run dev

# This alias in your dotfiles is convenient:
alias npm-d="npm run dev"
```

Dev builds run quicker on your machine. They make un-minified CSS, JS, & images.

Dev builds also create a sourcemap in the stylesheets. This allows tools like Chrome's inspect to display the Sass module a particular style is located in.

-----

<br>

## Production

***Only production builds should be pushed to the GitHub repo.***

```shell
$ npm run production

# Another convenient alias:
alias npm-p="npm run production"
```

Production build minifies CSS and JavaScript and compresses image files.

<br>

-----