# @hooks2022/use-prevent-leave

React Hook to prompt the user for confirmation before leaving the page. Useful when changes haven't been saved.

## Installation

#### yarn

`yarn add @hooks2022/use-prevent-leave`

#### npm

`npm i @hooks2022/use-prevent-leave`

## Usage

```js
import React from "react";
import usePreventLeave from "@hooks2022/use-prevent-leave";

function App() {
  const { enablePrevent, disablePrevent } = usePreventLeave();
  const saveChanges = async () => {
    enablePrevent();
    await sendToApi();
    disablePrevent();
  };
  return <button onClick={saveChanges}>Save changes</button>;
}
```
