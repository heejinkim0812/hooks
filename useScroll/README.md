# @hooks2022/use-scroll

React Hook to get X/Y coordinates of current position of the scroll.

## Installation

#### yarn

`yarn add @noohooks2022ks/use-scroll`

#### npm

`npm i @hooks2022/use-scroll`

## Usage

```js
import React from "react";
import useScroll from "@hooks2022/use-scroll";

function App() {
  const { x, y } = useScroll();
  return (
    <h1>
      We are in: {x} / {y}
    </h1>
  );
}
```
