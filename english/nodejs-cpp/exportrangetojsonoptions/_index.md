---
title: ExportRangeToJsonOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Indicates the options that exporting range to json.
type: docs
url: /nodejs-cpp/exportrangetojsonoptions/
---

## ExportRangeToJsonOptions class

Indicates the options that exporting range to json.

```javascript
class ExportRangeToJsonOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getHasHeaderRow()](#getHasHeaderRow--)| Indicates whether the range contains header row. |
| [setHasHeaderRow(boolean)](#setHasHeaderRow-boolean-)| Indicates whether the range contains header row. |
| [getExportAsString()](#getExportAsString--)| Exports the string value of the cells to json. |
| [setExportAsString(boolean)](#setExportAsString-boolean-)| Exports the string value of the cells to json. |
| [getExportEmptyCells()](#getExportEmptyCells--)| Indicates whether exporting empty cells as null. |
| [setExportEmptyCells(boolean)](#setExportEmptyCells-boolean-)| Indicates whether exporting empty cells as null. |
| [getIndent()](#getIndent--)| Indicates the indent. |
| [setIndent(string)](#setIndent-string-)| Indicates the indent. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getHasHeaderRow() {#getHasHeaderRow--}

Indicates whether the range contains header row.

```javascript
getHasHeaderRow() : boolean;
```


### setHasHeaderRow(boolean) {#setHasHeaderRow-boolean-}

Indicates whether the range contains header row.

```javascript
setHasHeaderRow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportAsString() {#getExportAsString--}

Exports the string value of the cells to json.

```javascript
getExportAsString() : boolean;
```


### setExportAsString(boolean) {#setExportAsString-boolean-}

Exports the string value of the cells to json.

```javascript
setExportAsString(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportEmptyCells() {#getExportEmptyCells--}

Indicates whether exporting empty cells as null.

```javascript
getExportEmptyCells() : boolean;
```


### setExportEmptyCells(boolean) {#setExportEmptyCells-boolean-}

Indicates whether exporting empty cells as null.

```javascript
setExportEmptyCells(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getIndent() {#getIndent--}

Indicates the indent.

```javascript
getIndent() : string;
```


**Remarks**

If the indent is null or empty, the exported json is not formatted.

### setIndent(string) {#setIndent-string-}

Indicates the indent.

```javascript
setIndent(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

If the indent is null or empty, the exported json is not formatted.


