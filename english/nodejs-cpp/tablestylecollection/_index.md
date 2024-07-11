---
title: TableStyleCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents all custom table styles.
type: docs
url: /nodejs-cpp/tablestylecollection/
---

## TableStyleCollection class

Represents all custom table styles.

```javascript
class TableStyleCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the table style by the index. |
| [getDefaultTableStyleName()](#getDefaultTableStyleName--)| Gets and sets the default style name of the table. |
| [setDefaultTableStyleName(string)](#setDefaultTableStyleName-string-)| Gets and sets the default style name of the table. |
| [getDefaultPivotStyleName()](#getDefaultPivotStyleName--)| Gets and sets the  default style name of pivot table . |
| [setDefaultPivotStyleName(string)](#setDefaultPivotStyleName-string-)| Gets and sets the  default style name of pivot table . |
| [addTableStyle(string)](#addTableStyle-string-)| Adds a custom table style. |
| [addPivotTableStyle(string)](#addPivotTableStyle-string-)| Adds a custom pivot table style. |
| [getBuiltinTableStyle(TableStyleType)](#getBuiltinTableStyle-tablestyletype-)| Gets the builtin table style |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### get(number) {#get-number-}

Gets the table style by the index.

```javascript
get(index: number) : TableStyle;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The position of the table style in the list. |

**Returns**

The table style object.

### getDefaultTableStyleName() {#getDefaultTableStyleName--}

Gets and sets the default style name of the table.

```javascript
getDefaultTableStyleName() : string;
```


### setDefaultTableStyleName(string) {#setDefaultTableStyleName-string-}

Gets and sets the default style name of the table.

```javascript
setDefaultTableStyleName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getDefaultPivotStyleName() {#getDefaultPivotStyleName--}

Gets and sets the  default style name of pivot table .

```javascript
getDefaultPivotStyleName() : string;
```


### setDefaultPivotStyleName(string) {#setDefaultPivotStyleName-string-}

Gets and sets the  default style name of pivot table .

```javascript
setDefaultPivotStyleName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### addTableStyle(string) {#addTableStyle-string-}

Adds a custom table style.

```javascript
addTableStyle(name: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The table style name. |

**Returns**

The index of the table style.

### addPivotTableStyle(string) {#addPivotTableStyle-string-}

Adds a custom pivot table style.

```javascript
addPivotTableStyle(name: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The pivot table style name. |

**Returns**

The index of the pivot table style.

### getBuiltinTableStyle(TableStyleType) {#getBuiltinTableStyle-tablestyletype-}

Gets the builtin table style

```javascript
getBuiltinTableStyle(type: TableStyleType) : TableStyle;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [TableStyleType](./tablestyletype/) | The builtin table style type. |

**Returns**

[TableStyle](./tablestyle/)

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



