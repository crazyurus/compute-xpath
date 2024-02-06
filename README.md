# Compute xPath

![publish](https://github.com/crazyurus/xpath/actions/workflows/publish.yaml/badge.svg)
[![BSD-3-Clause License](https://img.shields.io/badge/license-BSD-blue.svg)](LICENSE)
[![npm](https://badgen.net/npm/v/compute-xpath)](https://www.npmjs.com/package/compute-xpath)
[![npm dependents](https://badgen.net/npm/dependents/compute-xpath)](https://www.npmjs.com/package/compute-xpath?activeTab=dependents)
[![npm downloads](https://badgen.net/npm/dt/compute-xpath)](https://www.npmjs.com/package/compute-xpath)

This is a library that generates xPath based on DOM elements. The implementation is extracted from [Chrome DevTools Frontend](https://github.com/ChromeDevTools/devtools-frontend)

## Introduction

You can generate xPath based on DOM elements. For example:

```js
import { computeXPath } from 'compute-xpath';

const xPath = computeXPath(element)[0];
```

If you need to query the corresponding element or text based on xPath, you can call the browser API `document.evalute`. For example:

```js
const result = document.evaluate(xPath, document.documentElement);
const element = result.iterateNext();
```

## Parameters

- **node**: The node to compute
- **optimized**: Whether to optimize the XPath for the node. Does not imply the XPath is shorter; implies the XPath will be highly-scoped to the node.

## License

[BSD-3-Clause](./LICENSE)
