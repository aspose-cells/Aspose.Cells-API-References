---
title: PivotFieldCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents a collection of all the PivotField objects in the different regions of the pivot table.
type: docs
url: /javascript-cpp/pivotfieldcollection/
---

## PivotFieldCollection class

Represents a collection of all the PivotField objects in the different regions of the pivot table.

```javascript
class PivotFieldCollection;
```


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [type](#type--)| PivotFieldType | Readonly. Gets the PivotFields type. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the PivotField Object at the specific index. |
| [get(string)](#get-string-)| Gets the PivotField Object of the specific name. |
| [removeAt(number)](#removeAt-number-)| Removes field by the index. Only for filter,row,column,data region. |
| [addByBaseIndex(number)](#addByBaseIndex-number-)| Adds a PivotField Object to the specific type PivotFields. |
| [add(PivotField)](#add-pivotfield-)| Adds a PivotField Object to the specific type PivotFields. |
| [insert(number, PivotField)](#insert-number-pivotfield-)| Insert a pivot field at specific index. |
| [clear()](#clear--)| clear all fields of PivotFieldCollection |
| [remove(PivotField)](#remove-pivotfield-)| Removes field from the current region. |
| [move(number, number)](#move-number-number-)| Moves the PivotField from current position to destination position |


### type {#type--}

Readonly. Gets the PivotFields type.

```javascript
type : PivotFieldType;
```


### get(number) {#get-number-}

Gets the PivotField Object at the specific index.

```javascript
get(index: number) : PivotField;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

**Returns**

[PivotField](../pivotfield/)

### get(string) {#get-string-}

Gets the PivotField Object of the specific name.

```javascript
get(name: string) : PivotField;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string |  |

**Returns**

[PivotField](../pivotfield/)

### removeAt(number) {#removeAt-number-}

Removes field by the index. Only for filter,row,column,data region.

```javascript
removeAt(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

### addByBaseIndex(number) {#addByBaseIndex-number-}

Adds a PivotField Object to the specific type PivotFields.

```javascript
addByBaseIndex(baseFieldIndex: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | number | field index in the base PivotFields. |

**Returns**

the index of  the PivotField Object in this PivotFields.

### add(PivotField) {#add-pivotfield-}

Adds a PivotField Object to the specific type PivotFields.

```javascript
add(pivotField: PivotField) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | [PivotField](../pivotfield/) | a PivotField Object. |

**Returns**

the index of  the PivotField Object in this PivotFields.

### insert(number, PivotField) {#insert-number-pivotfield-}

Insert a pivot field at specific index.

```javascript
insert(index: number, pivotField: PivotField) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
| pivotField | [PivotField](../pivotfield/) | The field. |

### clear() {#clear--}

clear all fields of PivotFieldCollection

```javascript
clear() : void;
```


### remove(PivotField) {#remove-pivotfield-}

Removes field from the current region.

```javascript
remove(pivotField: PivotField) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | [PivotField](../pivotfield/) |  |

### move(number, number) {#move-number-number-}

Moves the PivotField from current position to destination position

```javascript
move(currPos: number, destPos: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| currPos | number | Current position of PivotField based on zero |
| destPos | number | Destination position of PivotField based on zero |


