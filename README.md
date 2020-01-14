# rollup-plugin-react-compat

<a href="https://www.npmjs.com/package/rollup-plugin-react-compat" target="_blank"><img src="https://img.shields.io/npm/v/rollup-plugin-react-compat.svg?style=flat-square&color=007acc&label=version" alt="npm version" /></a>
<img src="https://img.shields.io/badge/language-typescript-blue.svg?style=flat-square"/>
<a href="https://github.com/daybrush/rollup-plugin-react-compat/blob/master/LICENSE" target="_blank"><img src="https://img.shields.io/github/license/daybrush/rollup-plugin-react-compat.svg?style=flat-square&label=license&color=08CE5D"/></a>


## 🚀 How to use
* See Options: https://github.com/rollup/rollup-plugin-node-resolve

```js
const preact = require("rollup-plugin-react-compat");


{
    external: ["preact", "preact-compat"],
    plugins: [
        preact({
            ...nodeResolveOptions,
            useReactCompat: false,
            usePreactCompat: false,
            usePreactX: false, // usePreactX is auto resolvePreactCompat: true.
            noPropTypes: false,
            noReactIs: false,
            noEnv: false,
            resolvePreactCompat: false,
            aliasModules: {
                "react-css-styled": "preact-css-styled",
            },
        }),
    ],
}
```

## 👏 Contributing

If you have any questions or requests or want to contribute to `rollup-plugin-react-compat` or other packages, please write the [issue](https://github.com/daybrush/rollup-plugin-react-compat/issues) or give me a Pull Request freely.

## 🐞 Bug Report

If you find a bug, please report to us opening a new [Issue](https://github.com/daybrush/rollup-plugin-react-compat/issues) on GitHub.


## 📝 License

This project is [MIT](https://github.com/daybrush/rollup-plugin-react-compat/blob/master/LICENSE) licensed.

```
MIT License

Copyright (c) 2019 Daybrush

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```