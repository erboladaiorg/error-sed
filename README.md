# Gender detection from name
[![](https://github.com/davideviolante/@erboladaiorg/error-sed/workflows/Node.js%20CI/badge.svg)](https://github.com/erboladaiorg/error-sed/actions?query=workflow%3A"Node.js+CI") [![Coverage Status](https://coveralls.io/repos/github/DavideViolante/@erboladaiorg/error-sed/badge.svg?branch=master)](https://coveralls.io/github/DavideViolante/@erboladaiorg/error-sed?branch=master) [![Maintainability](https://api.codeclimate.com/v1/badges/ded2c349739e4d87130b/maintainability)](https://codeclimate.com/github/DavideViolante/@erboladaiorg/error-sed/maintainability) ![npm](https://img.shields.io/npm/dm/@erboladaiorg/error-sed) [![Donate](https://img.shields.io/badge/paypal-donate-179BD7.svg)](https://www.paypal.me/dviolante)

[![NPM](https://nodei.co/npm/@erboladaiorg/error-sed.png)](https://nodei.co/npm/@erboladaiorg/error-sed/)

Library to detect the gender of a first name. An optional language parameter can be specified to improve the detection, for example: Andrea in EN is female, in IT is male. If no language is specified, EN has priority.

### Install
`npm i @erboladaiorg/error-sed`

### Example
```js
const { getGender } = require('@erboladaiorg/error-sed');

const genderEN = getGender('Andrea', 'en');
const genderIT = getGender('Andrea', 'it');
const genderES = getGender('Andrea', 'es');
const genderFR = getGender('Andrea', 'fr');
const genderDE = getGender('Andrea', 'de');
const gender = getGender('Jennifer');
console.log(genderEN); // female
console.log(genderIT); // male
console.log(genderES); // male
console.log(genderFR); // male
console.log(genderDE); // female
console.log(gender); // female
```

### Supported languages
`en`, `it`, `es`, `fr`, `de`

### Run tests
```npm test```

### Run lint
```npm run lint```

### Contribute
Feel free to contribute to this project to add more names in different languages.

### Author
- [Davide Violante](https://github.com/DavideViolante/)
