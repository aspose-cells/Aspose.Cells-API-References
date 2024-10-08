﻿---
title: ErrorCheckOption
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Error check setting applied on certain ranges.
type: docs
url: /nodejs-cpp/errorcheckoption/
---

## ErrorCheckOption class

Error check setting applied on certain ranges.

```javascript
class ErrorCheckOption;
```


## Methods

| Method | Description |
| --- | --- |
| [isErrorCheck(ErrorCheckType)](#isErrorCheck-errorchecktype-)| Checks whether given error type will be checked. |
| [setErrorCheck(ErrorCheckType, boolean)](#setErrorCheck-errorchecktype-boolean-)| Sets whether given error type will be checked. |
| [getCountOfRange()](#getCountOfRange--)| Gets the count of ranges that influenced by this setting. |
| [addRange(CellArea)](#addRange-cellarea-)| Adds one influenced range by this setting. |
| [getRange(number)](#getRange-number-)| Gets the influenced range of this setting by given index. |
| [removeRange(number)](#removeRange-number-)| Removes one range by given index. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### isErrorCheck(ErrorCheckType) {#isErrorCheck-errorchecktype-}

Checks whether given error type will be checked.

```javascript
isErrorCheck(errorCheckType: ErrorCheckType) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| errorCheckType | [ErrorCheckType](../errorchecktype/) | error type can be checked |

**Returns**

return true if given error type will be checked(green triangle will be shown for cell if the check failed).

### setErrorCheck(ErrorCheckType, boolean) {#setErrorCheck-errorchecktype-boolean-}

Sets whether given error type will be checked.

```javascript
setErrorCheck(errorCheckType: ErrorCheckType, isCheck: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| errorCheckType | [ErrorCheckType](../errorchecktype/) | error type can be checked. |
| isCheck | boolean | true if given error type needs to be checked(green triangle will be shown for cell if the check failed). |

### getCountOfRange() {#getCountOfRange--}

Gets the count of ranges that influenced by this setting.

```javascript
getCountOfRange() : number;
```


**Returns**

the count of ranges that influenced by this setting.

### addRange(CellArea) {#addRange-cellarea-}

Adds one influenced range by this setting.

```javascript
addRange(ca: CellArea) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../cellarea/) | the range to be added. |

**Returns**

the index of the added range in the range list of this setting.

### getRange(number) {#getRange-number-}

Gets the influenced range of this setting by given index.

```javascript
getRange(index: number) : CellArea;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | the index of range |

**Returns**

return influenced range at given index.

### removeRange(number) {#removeRange-number-}

Removes one range by given index.

```javascript
removeRange(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | the index of the range to be removed. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



