# minimal-lightbox
A minimal Medium.com-style lightbox for enlarging media using css transforms, scaling images from their position on a page

## Install

__No Dependencies__


__npm__
```sh
$ npm install minimal-lightbox
```

## Usage

Currently, only img tags with `data-action=zoom` will be picked up on page load and bound to be zoomable. This module is dependent on classes/styles to produce the lightbox effect, so your mileage may vary on certain older browsers.

You'll want to include the styles from the `/dist` directory as well.

```html
<!DOCTYPE html>
<html>
<head>
  <link rel='stylesheet' type='text/css' href='../dist/minimal-lightbox.css'>
</head>
<body>
  <img src='http://lorempixel.com/1000/400' data-action='zoom'/>
  
  <!-- include the package -->
  <script type="text/javascript" src="../dist/minimal-lightbox.js"></script>
</body>
</html>
```

## Contribute

Fork and PR any improvements, bug fixes you find. Feel free to open new issues.

There are a couple npm scripts to help build the dist anytime you make changes in `src`:

To compile new files in `/dist` that include your changes, use this:
```sh
$ npm run compile
```

To include source-maps for devving changes:

```sh
$ npm run debug
```
