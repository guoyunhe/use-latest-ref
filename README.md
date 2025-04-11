# use-latest-ref

React hook to provide stable reference to latest props, state, options, etc.

## Installation

```bash
npm i -S @guoyunhe/use-latest-ref
```

### Usage

```js
function Foobar(props) {
  const propsRef = useLatestRef(props);

  // you don't need to put props.foobar into dependencies and it is always the latest value
  useEffect(() => {
    propsRef.current.foobar;
  }, []);

  // ...
}
```
