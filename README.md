This is a private fork of fine-uploader to make it work with [FileJet](https://github.com/everlutionsk/FileJetBundle)

Difference with original fork in source files is 2 LOC

### Installation
1. download via npm
```
./ops npm install git://github.com/everlutionsk/fine-uploader.git#filejet
```

2. include in encore webpack config
```diff
--- project/webpack.config.js
+++ project/webpack.config.js
Encore
   .createSharedEntry('js/vendor', [
      'jquery',
      'tether',
      'popper.js',
+     'fine-uploader/_build/fine-uploader.js',
      './assets/js/ajax.js',
      './assets/js/modal.js',
      './assets/js/rooms.js',
      './assets/js/modified_fine_uploader.js',
      './assets/js/autocomplete.js',
```
