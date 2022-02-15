# @hooks2022/use-fade-in

React Hook to fade in any element.

## Installation

#### yarn

`yarn add @hooks2022/use-fade-in`

#### npm

`npm i @hooks2022/use-fade-in`

## Usage

```js
import React from "react";
import useFadeIn from "@hooks2022/use-fade-in";

function App() {
  const fadeIn = useFadeIn(5, 10);
  return <h1 {...fadeIn}>This will fade in.</h1>;
}
```
