---
title: PivotAreaCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents a list of pivot area.
type: docs
url: /javascript-cpp/pivotareacollection/
---

## PivotAreaCollection class

Represents a list of pivot area.

```javascript
class PivotAreaCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets a [PivotArea](../pivotarea/) object; |
| [add(PivotArea)](#add-pivotarea-)| Adds pivot area. |
| [add(CellArea)](#add-cellarea-)| Adds an area based on pivot table view. |
| [addPivotArea(PivotArea)](#addPivotArea-pivotarea-)| Adds pivot area into this collection. |
| [removeAt(number)](#removeAt-number-)| Remove one pivot conditional formatted area setting. |


### get(number) {#get-number-}

Gets a [PivotArea](../pivotarea/) object;

```javascript
get(index: number) : PivotArea;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

**Returns**

[PivotArea](../pivotarea/)

### add(PivotArea) {#add-pivotarea-}

Adds pivot area.

```javascript
add(pivotArea: PivotArea) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotArea | [PivotArea](../pivotarea/) | The pivot area. |

**Remarks**

NOTE: This member is now obsolete. Instead, please use AddPivotArea() method. This method will be removed 6 months later since December 2025. Aspose apologizes for any inconvenience you may have experienced.

### add(CellArea) {#add-cellarea-}

Adds an area based on pivot table view.

```javascript
add(cellArea: CellArea) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../cellarea/) | The area based on pivot table view. |

### addPivotArea(PivotArea) {#addPivotArea-pivotarea-}

Adds pivot area into this collection.

```javascript
addPivotArea(pivotArea: PivotArea) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotArea | [PivotArea](../pivotarea/) |  |

**Returns**

index of the added pivot area in this collection

### removeAt(number) {#removeAt-number-}

Remove one pivot conditional formatted area setting.

```javascript
removeAt(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index |


