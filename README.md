# pointcss
A flexible CSS Framework for building modern responsive web apps.

- Built with Flexbox
- Mobile-First
- BEM, Namespaces, Modular, Beautiful code
- 10KB minified and gzipped

## Setup
There are 3 ways to start

### Install with Yarn
```sh
yarn add point-sass
```

### Install with NPM
```sh
npm install point-sass --save
```

### Direct `<script>` Include
`<link rel="stylesheet" href="dist/point.min.css" />`

## Documentation
- [Documentation](http://point.moyu.io/getting-started/)
- [Style Guide](http://point.moyu.io/getting-started/style-guide.html)

## Customize
Point is coded in [SASS](http://sass-lang.com/), If you're familiar with it, You can continue.

### 1. Install the dependence
```sh
yarn add point-sass --dev
```

### 2. Set your variables
you can reference all initial variables in `scss/_vars.scss`
```scss
$master-palette: (
  primary: #e74c3c
);

$link-color: #e74c3c;
```

### 3. Import Point at the end of your code
```scss
$master-palette: (
  primary: #e74c3c
);

$link-color: #e74c3c;

// Your code

@import "node_modules/point-sass/point"
```

## Browser Support
Point uses [Normalize.css](https://necolas.github.io/normalize.css/) for CSS
reset and [Autoprefixer](https://github.com/postcss/autoprefixer) to make styles
compatible with earlier browser versions. For best user experience, these
browsers are recommended:

- Chrome
- Firefox
- Safari
- Opera
- Microsoft Edge
- Internet Explorer 10+

## Copyright and license
Code copyright 2017 moyu. Code released under [the MIT license](https://github.com/moyus/point/blob/master/LICENSE).
