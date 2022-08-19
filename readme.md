# @esm2cjs/aggregate-error

This is a fork of https://github.com/sindresorhus/aggregate-error, but automatically patched to support ESM **and** CommonJS, unlike the original repository.

## Install

You can use an npm alias to install this package under the original name:

```
npm i aggregate-error@npm:@esm2cjs/aggregate-error
```

```jsonc
// package.json
"dependencies": {
    "aggregate-error": "npm:@esm2cjs/aggregate-error"
}
```

but `npm` might dedupe this incorrectly when other packages depend on the replaced package. If you can, prefer using the scoped package directly:

```
npm i @esm2cjs/aggregate-error
```

```jsonc
// package.json
"dependencies": {
    "@esm2cjs/aggregate-error": "^ver.si.on"
}
```

## Usage

```js
// Using ESM import syntax
import AggregateError from "@esm2cjs/aggregate-error";

// Using CommonJS require()
const AggregateError = require("@esm2cjs/aggregate-error").default;
```

> **Note:**
> Because the original module uses `export default`, you need to append `.default` to the `require()` call.

For more details, please see the original [repository](https://github.com/sindresorhus/aggregate-error).

## Sponsoring

To support my efforts in maintaining the ESM/CommonJS hybrid, please sponsor [here](https://github.com/sponsors/AlCalzone).

To support the original author of the module, please sponsor [here](https://github.com/sindresorhus/aggregate-error).
