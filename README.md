# angular-translate-loader-static-files [![Build Status](https://travis-ci.org/PascalPrecht/angular-translate-loader-static-files.png?branch=master)](https://travis-ci.org/PascalPrecht/angular-translate-loader-static-files) [![Build Status](https://travis-ci.org/PascalPrecht/angular-translate-loader-static-files.png?branch=canary)](https://travis-ci.org/PascalPrecht/angular-translate-loader-static-files) [![Dependency Status](https://gemnasium.com/PascalPrecht/angular-translate-loader-static-files.png)](https://gemnasium.com/PascalPrecht/angular-translate-loader-static-files)



> Static files loader extension for angular-translate

Use this extension to use the asynchronous static-files loader for `angular-translate`.

## Quick Start

Install extension via Bower:

```
$ bower install angular-translate-loader-static-files
```

Embed the package file **after** `angular-translate` and **before** your app:

```html
<script src="path/to/angular-translate.js"></script>
<script src="path/to/angular-translate-loader-static-files.js"></script>
<script src="path/to/app.js"></script>
```

And within module config, simply do:

```js
angular.module('myApp', ['pascalprecht.translate']);

angular.module('myApp').config(['$translateProvider', function ($translateProvider) {

  // use static-files loader with options object
  $translateProvider.useStaticFilesLoader({
    prefix: 'lang_',
    suffix: '.json'
  });
}]);
```

More information in the [angular-translate wiki](https://github.com/PascalPrecht/angular-translate/wiki).

### Contributing
Any idea to make this thing better? Read the [Contributing Guide](CONTRIBUTING.md),
I'd **<3** to get some PR's from you!


[![WTFPL](http://www.wtfpl.net/wp-content/uploads/2012/12/wtfpl-badge-4.png)](http://wtfpl.net)
