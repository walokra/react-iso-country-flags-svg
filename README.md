# react-iso-country-flags

A list of countries with flag images.

Combines the idea and modified code from [country-flags-svg](https://github.com/ronatskiy/country-flags-svg) with images from [country-flags](https://github.com/hampusborgos/country-flags).

## Install

```bash
npm install --save iso-country-flags
```

## Usage

```jsx
import React, { Component } from 'react';
import { findFlagByIso2Code } from 'iso-country-flags';

const CountryFlagImg = ({ countryCode, dimensions }) => {
  const Flag = findFlagByIso2Code(countryCode).ReactComponent;
  return (
    <svg width={dimensions.width} height={dimensions.height}>
      <Flag />
    </svg>
  );
};

class Example extends Component {
  render() {
    return (
      <CountryFlagImg
        countryCode={'fi'}
        dimensions={{ width: '3.33vw', height: '2.5vh' }}
      />
    );
  }
}
```

## API

### `countries`

Returns all available information.


### `findFlagByCountryName(countryName)`

Returns SVG link of the official flag for a specified country (according to countryName) or empty string if is not exist

### `findFlagByNationality(nationality)`

Returns SVG link of the official flag for a specified country (according to nationality) or empty string if is not exist

### `findFlagByIso2Code(iso2Code)`

Returns SVG link of the official flag for a specified country (according to [ISO 3166-1 alpha-2](http://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) code) or empty string if is not exist

### `findFlagByIso3Code(iso3Code)`

Returns SVG link of the official flag for a specified country (according to [ISO 3166-1 alpha-3](http://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code) or empty string if is not exist

## Available Flags*

<!-- AUTO-GENERATED-CONTENT:START (LIST_OF_FLAGS) -->
<!-- AUTO-GENERATED-CONTENT:END -->

## License

Licensed under **MIT**.
