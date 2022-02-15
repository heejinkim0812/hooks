# @hooks2022/use-confirm

React Hook to ask the user for a confirmation before executing a function.

## Installation

#### yarn

`yarn add @hooks2022/use-confirm`

#### npm

`npm i @hooks2022/use-confirm`

## Usage

```js
import React from "react";
import useConfirm from "@hooks2022/use-confirm";

function App() {
  const deleteWorld = () => console.log("Deleting world...");
  const confirmDelete = useConfirm("Are you sure?", deleteWorld);
  return <button onClick={confirmDelete}>Delete the world</button>;
}
```
