---
title: PasteOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the paste special options.
type: docs
url: /nodejs-cpp/pasteoptions/
---

## PasteOptions class

Represents the paste special options.

```javascript
class PasteOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getPasteType()](#getPasteType--)| The paste special type. |
| [setPasteType(PasteType)](#setPasteType-pastetype-)| The paste special type. |
| [getSkipBlanks()](#getSkipBlanks--)| Indicates whether skips blank cells. |
| [setSkipBlanks(boolean)](#setSkipBlanks-boolean-)| Indicates whether skips blank cells. |
| [getOnlyVisibleCells()](#getOnlyVisibleCells--)| True means only copying visible cells. |
| [setOnlyVisibleCells(boolean)](#setOnlyVisibleCells-boolean-)| True means only copying visible cells. |
| [getTranspose()](#getTranspose--)| True to transpose rows and columns when the range is pasted. The default value is False. |
| [setTranspose(boolean)](#setTranspose-boolean-)| True to transpose rows and columns when the range is pasted. The default value is False. |
| [getOperationType()](#getOperationType--)| Gets and sets the operation type when pasting range. |
| [setOperationType(PasteOperationType)](#setOperationType-pasteoperationtype-)| Gets and sets the operation type when pasting range. |
| [getIgnoreLinksToOriginalFile()](#getIgnoreLinksToOriginalFile--)| Ingore links to the original file. |
| [setIgnoreLinksToOriginalFile(boolean)](#setIgnoreLinksToOriginalFile-boolean-)| Ingore links to the original file. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getPasteType() {#getPasteType--}

The paste special type.

```javascript
getPasteType() : PasteType;
```


**Returns**

[PasteType](../pastetype/)

### setPasteType(PasteType) {#setPasteType-pastetype-}

The paste special type.

```javascript
setPasteType(value: PasteType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PasteType](../pastetype/) | The value to set. |

### getSkipBlanks() {#getSkipBlanks--}

Indicates whether skips blank cells.

```javascript
getSkipBlanks() : boolean;
```


### setSkipBlanks(boolean) {#setSkipBlanks-boolean-}

Indicates whether skips blank cells.

```javascript
setSkipBlanks(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getOnlyVisibleCells() {#getOnlyVisibleCells--}

True means only copying visible cells.

```javascript
getOnlyVisibleCells() : boolean;
```


### setOnlyVisibleCells(boolean) {#setOnlyVisibleCells-boolean-}

True means only copying visible cells.

```javascript
setOnlyVisibleCells(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getTranspose() {#getTranspose--}

True to transpose rows and columns when the range is pasted. The default value is False.

```javascript
getTranspose() : boolean;
```


### setTranspose(boolean) {#setTranspose-boolean-}

True to transpose rows and columns when the range is pasted. The default value is False.

```javascript
setTranspose(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getOperationType() {#getOperationType--}

Gets and sets the operation type when pasting range.

```javascript
getOperationType() : PasteOperationType;
```


**Returns**

[PasteOperationType](../pasteoperationtype/)

### setOperationType(PasteOperationType) {#setOperationType-pasteoperationtype-}

Gets and sets the operation type when pasting range.

```javascript
setOperationType(value: PasteOperationType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PasteOperationType](../pasteoperationtype/) | The value to set. |

### getIgnoreLinksToOriginalFile() {#getIgnoreLinksToOriginalFile--}

Ingore links to the original file.

```javascript
getIgnoreLinksToOriginalFile() : boolean;
```


### setIgnoreLinksToOriginalFile(boolean) {#setIgnoreLinksToOriginalFile-boolean-}

Ingore links to the original file.

```javascript
setIgnoreLinksToOriginalFile(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



