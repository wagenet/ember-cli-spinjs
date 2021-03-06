# Ember-cli Spinjs


[![CircleCI](https://circleci.com/gh/kiwiupover/ember-cli-spinjs.svg?style=shield)](https://circleci.com/gh/kiwiupover/ember-cli-spinjs/tree/master)
[![Ember Observer Score](http://emberobserver.com/badges/ember-cli-spinjs.svg)](http://emberobserver.com/addons/ember-cli-spinjs)
[![Code Climate](https://codeclimate.com/github/kiwiupover/ember-cli-spinjs/badges/gpa.svg)](https://codeclimate.com/github/kiwiupover/ember-cli-spinjs)
[![npm version](https://badge.fury.io/js/ember-cli-spinjs.svg)](http://badge.fury.io/js/ember-cli-spinjs)
[![Greenkeeper badge](https://badges.greenkeeper.io/kiwiupover/ember-cli-spinjs.svg)](https://greenkeeper.io/)

## Install
In the root of your ember-cli project directory, run:

```bash
  ember install ember-cli-spinjs
```

## Usage
Now you in your templates you can use `{{ember-spinner}}` to add a spinner to your page.

[View Demo](http://ember-cli-spinjs.surge.sh/)

```handlebars
{{ember-spinner}}
```
Default

### With a config file
```handlebars
{{ember-spinner config='standard'}}
```
Add two folders to your app the first called `config` and in that folder
another called `ember-spinner` with a file called `standard.js`

```javascript
export default {
  color:  'blue',
  lines:  10,
  length: 30,
  zIndex: 200000
}
```

```handlebars
{{ember-spinner lines=11 length=16 radius=30 width=8 rotate=10 speed='1.1' color="#ffc52e"}}
```
Spinning Lines

```handlebars
{{ember-spinner lines=18 radius=10 width=5 rotate=0 speed="3.4" color='blue'}}
```
Fast spinning blue dots.

### Dependencies

##### Spin.js
The [Spin.js docs](http://fgnass.github.io/spin.js/)
jQuery is no longer a dependency

### Linting

* `npm run lint:js`
* `npm run lint:js -- --fix`

### Running tests

* `ember test` – Runs the test suite on the current Ember version
* `ember test --server` – Runs the test suite in "watch mode"
* `ember try:each` – Runs the test suite against multiple Ember versions

### Running the dummy application

* `ember serve`
* Visit the dummy application at [http://localhost:4200](http://localhost:4200).

For more information on using ember-cli, visit [https://ember-cli.com/](https://ember-cli.com/).

License
------------------------------------------------------------------------------

This project is licensed under the [MIT License](LICENSE.md).
