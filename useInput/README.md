# Usage

```js
import useInput from "@hooks2022/use-input";

const App = () => {
  const validator = (value) => !value.includes("@");
  const name = useInput("Mr. ", validator);
  return (
    <div className="App">
      <h1>Hello</h1>
      <input placeholder="Name" {...name.props} />
    </div>
  );
};
```
