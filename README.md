# xPath

![publish](https://github.com/crazyurus/xpath/actions/workflows/publish.yaml/badge.svg)
[![BSD-3-Clause License](https://img.shields.io/badge/license-BSD-blue.svg)](LICENSE)
[![npm](https://badgen.net/npm/v/craco-css-modules)](https://www.npmjs.com/package/craco-css-modules)
[![npm dependents](https://badgen.net/npm/dependents/xPath)](https://www.npmjs.com/package/xPath?activeTab=dependents)
[![npm downloads](https://badgen.net/npm/dt/xPath)](https://www.npmjs.com/package/xPath)

This is a library that generates xPath based on DOM elements. The implementation is extracted from [Chrome DevTools Frontend](https://github.com/ChromeDevTools/devtools-frontend)

## Introduction

You can generate xPath based on DOM elements. For example:

```js
import { computeXPath } from 'xPath';

const xPath = computeXPath(element)[0];
```

## Parameters

- **node**: The node to compute
- **optimized**: Whether to optimize the XPath for the node. Does not imply the XPath is shorter; implies the XPath will be highly-scoped to the node.

## License

[BSD-3-Clause](./LICENSE)
