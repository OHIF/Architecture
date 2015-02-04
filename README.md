# Architecture

Introduction
------------
The formation of OHIF was heavily inspired by the work done in the [cornerstone platform](https://github.com/chafey/cornerstone).  The cornerstone project demonstrated the viability of a 100% HTML5/JavaScript based medical image viewer using client side rendering without the use of any plugins.  The OHIF seeks to take the work done in cornerstone as a foundation, modernize it to the latest web technologies (specifically ES6 and Web Components) and expand the scope to include all functionality found in medical imaging systems (e.g. archiving, 3D rendering, etc).


Languages
---------
The entire platform should be cross platform and cross browser.  JavaScript ES6 is our primary language for both client and server development.  Third Party JavaScript ES5 modules can be used when needed.  C/C++ is an option only if we cannot accomplish what we need in JavaScript for some reason.

* [JavaScript ES6](https://github.com/lukehoban/es6features) - as much as possible
* JavaScript ES5 - when using third party libraries 
* C/C++ - only if absolutely necessary

Technologies
------------

* [Meteor](https://www.meteor.com/) - as much as possible
* [6to5](https://6to5.org/) - for running ES6 code in NodeJS via 6to5Node (when meteor isn't appropriate)
* [6to5](https://6to5.org/) - ES6 transpiling
* [Web Components](http://webcomponents.org/) - as much as possible
* [Bootstrap 3](http://getbootstrap.com/) - base css/components
* [Polymer](https://www.polymer-project.org/) - baseline web components
* [JSPM](http://jspm.io/) - browser package registry
* [NPM](https://www.npmjs.com/) - npm package registry

Tools
-----

* [Mocha](http://unitjs.com/guide/mocha.html) - unit testing
* [6to5](https://6to5.org/) - ES6 transpiling
* [JetBrains WebStorm](https://www.jetbrains.com/webstorm/) - IDE
* [NPM](https://www.npmjs.com/) - build tool for NPM modules
* [github](https://github.com/) - source control

Modules
-------
* Modules should be as fine grained as possible
* Each module shall be hosted in its own github repository
* Client side modules should be published to the JSPM registry
* Server side modules should be published to the NPM registry
* Meteor only modules should be published to the Atmosphere
* TBD: Whether or not we publish as ES5 code
* 
