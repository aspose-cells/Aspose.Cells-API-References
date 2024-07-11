---
title: FindOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents find options.
type: docs
url: /nodejs-cpp/findoptions/
---

## FindOptions class

Represents find options.

```javascript
class FindOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getCaseSensitive()](#getCaseSensitive--)| Indicates if the searched string is case sensitive. |
| [setCaseSensitive(boolean)](#setCaseSensitive-boolean-)| Indicates if the searched string is case sensitive. |
| [getLookAtType()](#getLookAtType--)| Look at type. |
| [setLookAtType(LookAtType)](#setLookAtType-lookattype-)| Look at type. |
| [isRangeSet()](#isRangeSet--)| Indicates whether the searched range is set. |
| [getSearchBackward()](#getSearchBackward--)| Whether search backward for cells. |
| [setSearchBackward(boolean)](#setSearchBackward-boolean-)| Whether search backward for cells. |
| [getSeachOrderByRows()](#getSeachOrderByRows--)| Indicates whether search order by rows or columns. |
| [setSeachOrderByRows(boolean)](#setSeachOrderByRows-boolean-)| Indicates whether search order by rows or columns. |
| [getLookInType()](#getLookInType--)| Look in type. |
| [setLookInType(LookInType)](#setLookInType-lookintype-)| Look in type. |
| [getRegexKey()](#getRegexKey--)| Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel. |
| [setRegexKey(boolean)](#setRegexKey-boolean-)| Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel. |
| [getValueTypeSensitive()](#getValueTypeSensitive--)| Indicates whether searched cell value type should be same with the searched key. |
| [setValueTypeSensitive(boolean)](#setValueTypeSensitive-boolean-)| Indicates whether searched cell value type should be same with the searched key. |
| [getStyle()](#getStyle--)| The format to search for. |
| [setStyle(Style)](#setStyle-style-)| The format to search for. |
| [getConvertNumericData()](#getConvertNumericData--)| Gets or sets a value that indicates whether converting the searched string value to numeric data. |
| [setConvertNumericData(boolean)](#setConvertNumericData-boolean-)| Gets or sets a value that indicates whether converting the searched string value to numeric data. |
| [getRange()](#getRange--)| Gets and sets the searched range. |
| [setRange(CellArea)](#setRange-cellarea-)| Sets the searched range. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getCaseSensitive() {#getCaseSensitive--}

Indicates if the searched string is case sensitive.

```javascript
getCaseSensitive() : boolean;
```


### setCaseSensitive(boolean) {#setCaseSensitive-boolean-}

Indicates if the searched string is case sensitive.

```javascript
setCaseSensitive(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getLookAtType() {#getLookAtType--}

Look at type.

```javascript
getLookAtType() : LookAtType;
```


**Returns**

[LookAtType](./lookattype/)

### setLookAtType(LookAtType) {#setLookAtType-lookattype-}

Look at type.

```javascript
setLookAtType(value: LookAtType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LookAtType](./lookattype/) | The value to set. |

### isRangeSet() {#isRangeSet--}

Indicates whether the searched range is set.

```javascript
isRangeSet() : boolean;
```


### getSearchBackward() {#getSearchBackward--}

Whether search backward for cells.

```javascript
getSearchBackward() : boolean;
```


### setSearchBackward(boolean) {#setSearchBackward-boolean-}

Whether search backward for cells.

```javascript
setSearchBackward(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSeachOrderByRows() {#getSeachOrderByRows--}

Indicates whether search order by rows or columns.

```javascript
getSeachOrderByRows() : boolean;
```


### setSeachOrderByRows(boolean) {#setSeachOrderByRows-boolean-}

Indicates whether search order by rows or columns.

```javascript
setSeachOrderByRows(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getLookInType() {#getLookInType--}

Look in type.

```javascript
getLookInType() : LookInType;
```


**Returns**

[LookInType](./lookintype/)

### setLookInType(LookInType) {#setLookInType-lookintype-}

Look in type.

```javascript
setLookInType(value: LookInType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LookInType](./lookintype/) | The value to set. |

### getRegexKey() {#getRegexKey--}

Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel.

```javascript
getRegexKey() : boolean;
```


### setRegexKey(boolean) {#setRegexKey-boolean-}

Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel.

```javascript
setRegexKey(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getValueTypeSensitive() {#getValueTypeSensitive--}

Indicates whether searched cell value type should be same with the searched key.

```javascript
getValueTypeSensitive() : boolean;
```


### setValueTypeSensitive(boolean) {#setValueTypeSensitive-boolean-}

Indicates whether searched cell value type should be same with the searched key.

```javascript
setValueTypeSensitive(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getStyle() {#getStyle--}

The format to search for.

```javascript
getStyle() : Style;
```


**Returns**

[Style](./style/)

### setStyle(Style) {#setStyle-style-}

The format to search for.

```javascript
setStyle(value: Style) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Style](./style/) | The value to set. |

### getConvertNumericData() {#getConvertNumericData--}

Gets or sets a value that indicates whether converting the searched string value to numeric data.

```javascript
getConvertNumericData() : boolean;
```


### setConvertNumericData(boolean) {#setConvertNumericData-boolean-}

Gets or sets a value that indicates whether converting the searched string value to numeric data.

```javascript
setConvertNumericData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRange() {#getRange--}

Gets and sets the searched range.

```javascript
getRange() : CellArea;
```


**Returns**

Returns the searched range.

### setRange(CellArea) {#setRange-cellarea-}

Sets the searched range.

```javascript
setRange(ca: CellArea) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](./cellarea/) | the searched range. |


