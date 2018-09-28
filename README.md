# [Yayoi-js](https://panepo.github.io/Yayoi-js/)

[![Build Status](https://travis-ci.org/Panepo/Uzuki.svg?branch=master)](https://travis-ci.org/Panepo/Yayoi-js.svg) [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)

React implementation of image super-resolution using deep convolutional neural network (SRCNN)

## Requirements

* Browser (Chrome is perfered)
* Image for super-resolution

## Usage

First visit this [page](https://panepo.github.io/Yayoi-js/) and follow these steps:

![usage](https://github.com/Panepo/Yayoi-js/blob/master/doc/usage.png)

1. Upload the images
2. Click enlarge

## Results

Here are two result. From left to right, the first column is the input image, the second one is what you would get from a standard bicubic interpolation, and on the right is the the output generated by the neural net.

Butterfly

<img src="https://github.com/Panepo/Yayoi-js/blob/master/doc/butterfly_GT.bmp" alt="Butterfly" height="100" width="100"> <img src="https://github.com/Panepo/Yayoi-js/blob/master/doc/butterfly_opencv.png" alt="Butterfly" height="200" width="200"> <img src="https://github.com/Panepo/Yayoi-js/blob/master/doc/butterfly_srcnn.png" alt="Butterfly" height="200" width="200">

Shaman

<img src="https://github.com/Panepo/Yayoi-js/blob/master/doc/comic.png" alt="Shaman" height="144" width="100"> <img src="https://github.com/Panepo/Yayoi-js/blob/master/doc/comic_opencv.png" alt="Shaman" height="288" width="200"> <img src="https://github.com/Panepo/Yayoi-js/blob/master/doc/comic_srcnn.png" alt="Shaman" height="288" width="200">

## Library used

* [Tensorflow.js](https://js.tensorflow.org/)
* [React](https://facebook.github.io/react/)
* [Redux](http://redux.js.org/)
* [Create React App ](https://github.com/facebook/create-react-app)
* [Material Design Lite](https://getmdl.io/)
* [FlipMove](https://github.com/joshwcomeau/react-flip-move)

## Develop

### Development Requirements
* node `^8.11.0`
* yarn `^1.7.0`

### Getting Start

1. Clone source code
```
$ git clone https://github.com/Panepo/Yayoi-js.git
```
2. Install dependencies
```
$ cd Yayoi-js
$ yarn
```
3. Start development server and visit [http://localhost:3000/](http://localhost:3000/)
```
$ yarn start
```
### Scripts

|`yarn <script>`       |Description|
|-------------------|-----------|
|`start`            |Serves your app at `localhost:3000`|
|`test`             |Run test code in ./src|
|`lint`             |Lint code in ./src|
|`prettier`         |Prettier code in ./src|
|`build`            |Builds the production application to ./build|
|`deploy`           |Deploy the production application to github pages|

### Testing

Jest is used for test runner. Jest will look for test files with any of the following naming conventions:

* Files with `.js` suffix in `__tests__` folders.
* Files with `.test.js` suffix.
* Files with `.spec.js` suffix.

Jest has an integrated coverage reporter that works well with ES6 and requires no configuration.
Run `npm test -- --coverage` (note extra `--` in the middle) to include a coverage report.

### Production

Build code before deployment by running `yarn build`.

## Author

[Panepo](https://github.com/Panepo)
