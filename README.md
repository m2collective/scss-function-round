# SCSS Function Round

A package for integrating the rounding function of numeric values.

![npm](https://img.shields.io/npm/v/@bu0nq/scss-function-round?style=for-the-badge)
![npm](https://img.shields.io/npm/dt/@bu0nq/scss-function-round?style=for-the-badge)

Documentation: [EN](README.md) | [RU](README.RU.md)

___

## Installation

You can install the package automatically using NPM:

```
npm i @bu0nq/scss-function-round
```

## Usage

To use the package, import it into your project:

```scss
@use "@bu0nq/scss-function-round" as *;

.demo {
    font-size: round(16.4px);
}
```

## Changing the namespace

You can change the namespace during function import and use the function with a different namespace:

```scss
@use "@bu0nq/scss-function-round" as function;

.demo {
    font-size: function.round(16.4px);
}
```

## Changing the variables

You can redefine the default values for the specified variables when importing the function:

```scss
@use "@bu0nq/scss-function-round" as * with (
    $decimals: 0,
);
```
