# @hooks2022/use-axios

React Hook to execute a function using Axios, an HTTP asynchronous communication library.

## Installation

#### yarn

`yarn add @hooks2022/use-axios`

#### npm

`npm i @hooks2022/use-axios`

## Usage

```js
import React from "react";
import useBeforeLeave from "@hooks2022/use-axios";

function App() {
  const {loading, data, error, refetch}=useAxios(){
      url:"https://..."
  }
  console.log(`Loading: ${loading}\n Error: ${error}\n Data: ${JSON.stringfy(data)}`)
  return (
      <h1>{data && data.status}</h1>
      <h2>{loading && "Loading"}</h2>
      <button onClick={refetch}>Refetch</button>
  );

}
```
