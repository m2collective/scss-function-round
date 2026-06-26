# SCSS Function Round

A package for integrating the rounding function of numeric values.

![npm](https://img.shields.io/npm/v/@m2collective/scss-function-round?style=for-the-badge)

___

## Installation

You can install the package automatically using NPM:

```
npm i @m2collective/scss-function-round
```

## Usage

To use the package, import it into your project:

```scss
@use "@m2collective/scss-function-round" as *;

.demo {
    font-size: round(16.4px);
}

// Return
.demo {
    font-size: 16px;
}
```

## Changing the namespace

You can change the namespace during function import and use the function with a different namespace:

```scss
@use "@m2collective/scss-function-round" as function;

.demo {
    font-size: function.round(16.4px);
}

// Return
.demo {
    font-size: 16px;
}
```

## Changing the variables

You can redefine the default values for the specified variables when importing the function:

```scss
@use "@m2collective/scss-function-round" as * with (
    $decimals: 1,
);

.demo {
    font-size: round(16.4px);
}

// Return
.demo {
    font-size: 16.4px;
}
```

## License

The MIT License (MIT). Please see the [License file](LICENSE.txt) for more information.
