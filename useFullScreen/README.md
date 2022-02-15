# @hooks2022/use-fullscreen

React Hook to make any element go Fullscreen

## Installation

#### yarn

`yarn add @hooks2022/use-fullscreen`

#### npm

`npm i @hooks2022/use-fullscreen`

## Usage

```js
import React from "react";
import useFullscreen from "@hooks2022/use-fullscreen";

function App() {
  const onChange = (isFull) =>
    console.log(isFull ? "We are in Fullscreen" : "We are not in Fullscreen");
  const { element, triggerFull, exitFull } = useFullscreen(onChange);
  return (
    <div ref={element}>
      <h1>Hello</h1>
      <button onClick={triggerFull}>Make this Fullscreen</button>
      <button onClick={exitFull}>Exit Fullscreen</button>
    </div>
  );
}
```
