﻿---
title: OdsCellFieldCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the fields of ODS.
type: docs
url: /nodejs-cpp/odscellfieldcollection/
---

## OdsCellFieldCollection class

Represents the fields of ODS.

```javascript
class OdsCellFieldCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the field by the index. |
| [add(number, number, OdsCellFieldType, string)](#add-number-number-odscellfieldtype-string-)| Adds a field. |
| [updateFieldsValue()](#updateFieldsValue--)| Update fields value to the cells. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### get(number) {#get-number-}

Gets the field by the index.

```javascript
get(index: number) : OdsCellField;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

[OdsCellField](../odscellfield/)

### add(number, number, OdsCellFieldType, string) {#add-number-number-odscellfieldtype-string-}

Adds a field.

```javascript
add(row: number, column: number, fieldType: OdsCellFieldType, format: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| column | number | The column index. |
| fieldType | [OdsCellFieldType](../odscellfieldtype/) | The type of the field. |
| format | string | The number format of the field. |

### updateFieldsValue() {#updateFieldsValue--}

Update fields value to the cells.

```javascript
updateFieldsValue() : void;
```


### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



