# ESDoc Flow Type Plugin (PoC)
**This plugin is proof of concept.**

## Install
```bash
npm install esdocs-flow-type-plugin
```

## Config
```json
{
  "source": "./src",
  "destination": "./doc",
  "plugins": [
    {"name": "esdocs-flow-type-plugin", "option": {"enable": true}}
  ]
}
```

- `enable` is default `true`

## Example
```js
export class Foo {
  // without document
  member: number;
  
  // without document
  method1(n: number): string {
  }
  
  // without @param and @return
  /**
   * this is method2.
   */
  method2(n: number): string {
  }
  
  // without type in @param and @return
  /**
   * this is method3.
   * @param n - this is param desc.
   * @return this is return desc. 
   */
  method3(n: number): string {
  }
}
```

## LICENSE
MIT

## Authors
[Muhammad-Jibril B.A. @JBA-Khalifa](https://github.com/JBA-Khalifa)
[Ryo Maruyama@h13i32maru](https://github.com/h13i32maru)