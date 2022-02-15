# @hooks2022/use-network

React Hook to listen when the user goes online or offline.

## Installation

#### yarn

`yarn add @hooks2022/use-network`

#### npm

`npm i @hooks2022/use-network`

## Usage

```js
import React from "react";
import useNetwork from "@hooks2022/use-network";

function App() {
  const onNetworkChange = (isOnline) =>
    console.log(isOnline ? "We are back online" : "We just got offline");
  const isOnline = useNetwork(onNetworkChange);
  return <h1>{isOnline ? "We are online" : "We are offline"}</h1>;
}
```
