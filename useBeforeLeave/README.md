# @hooks2022/use-before-leave

React Hook to execute a function when the mouse leaves the page. Useful to show a popup or for analytics.

## Installation

#### yarn

`yarn add @hooks2022/use-before-leave`

#### npm

`npm i @hooks2022/use-before-leave`

## Usage

```js
import React from "react";
import useBeforeLeave from "@hooks2022/use-before-leave";

function App() {
  const beforeLeave = () => console.log("User is leaving...");
  useBeforeLeave(beforeLeave);
  return <h1>Hello Nooks</h1>;
}
```
