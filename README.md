# SCSS Function Round

Package for integrating `SCSS Function Round` in a web environment.

![npm](https://img.shields.io/npm/v/@bu0nq/scss-function-round?style=for-the-badge)
![npm](https://img.shields.io/npm/dt/@bu0nq/scss-function-round?style=for-the-badge)
___

## Installation

This package can be deployed automatically using NPM:

```
npm i @bu0nq/scss-function-round
```

## Usage

Import in your project depending on your setup:

```scss
@use "@bu0nq/scss-function-round" as *;

.demo {
    line-height: round(15.5px);
    font-size: round(15.4px);
}
```

Execution result:

```css
.demo {
    line-height: 16px;
    font-size: 15px;
}
```

## Namespace

You can change the namespace during import and use the rem function with a different namespace:

```scss
@use "@bu0nq/scss-function-round" as to;

.demo {
    font-size: to.round(16px);
}
```

## Changing decimals

```scss
@use "@bu0nq/scss-function-round" as * with (
  $decimals: 1
);

.demo {
    line-height: round(15.25px);
    font-size: round(15.24px);
}
```

Execution result:

```css
.demo {
    line-height: 15.3px;
    font-size: 15.2px;
}
```
