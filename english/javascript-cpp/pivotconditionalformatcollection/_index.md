---
title: PivotConditionalFormatCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents all conditional formats of pivot table.
type: docs
url: /javascript-cpp/pivotconditionalformatcollection/
---

## PivotConditionalFormatCollection class

Represents all conditional formats of pivot table.

```javascript
class PivotConditionalFormatCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the pivot FormatCondition object at the specific index. |
| [add()](#add--)| Adds a pivot FormatCondition to the collection. |
| [add(number, number, PivotConditionFormatScopeType)](#add-number-number-pivotconditionformatscopetype-)| Applies the conditional format to range which must in data region. |


### get(number) {#get-number-}

Gets the pivot FormatCondition object at the specific index.

```javascript
get(index: number) : PivotConditionalFormat;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

**Returns**

pivot FormatCondition object.

### add() {#add--}

Adds a pivot FormatCondition to the collection.

```javascript
add() : number;
```


**Returns**

pivot FormatCondition object index.

**Remarks**

not supported

### add(number, number, PivotConditionFormatScopeType) {#add-number-number-pivotconditionformatscopetype-}

Applies the conditional format to range which must in data region.

```javascript
add(row: number, column: number, scope: PivotConditionFormatScopeType) : PivotConditionalFormat;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The selected row. |
| column | number | The selected column. |
| scope | [PivotConditionFormatScopeType](../pivotconditionformatscopetype/) | The scope |

**Returns**

Returens [PivotConditionalFormat](../pivotconditionalformat/).


