---
title: License
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Provides methods to license the component.
type: docs
url: /nodejs-cpp/license/
---

## License class
Provides methods to license the component.

## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Initializes a new instance of this class. |


## Methods

| Method | Description |
| --- | --- |
| [setLicense(string)](#setLicense-string-)| Licenses the component. |
| [setLicense(Uint8Array)](#setLicense-uint8array-)| Licenses the component. |


### constructor() {#constructor--}

Initializes a new instance of this class.

```javascript
constructor();
```

### setLicense(string) {#setLicense-string-}

Licenses the component.

```javascript
setLicense(licenseName: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| licenseName | string | The license file path. |

### setLicense(Uint8Array) {setLicense-uint8array-}

Licenses the component.

```javascript
setLicense(stream: Uint8Array): void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Uint8Array | A stream that contains the license. |
