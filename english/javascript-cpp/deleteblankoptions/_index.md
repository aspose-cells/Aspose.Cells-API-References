---
title: DeleteBlankOptions
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the setting of deleting blank cellsrowscolumns.
type: docs
url: /javascript-cpp/deleteblankoptions/
---

## DeleteBlankOptions class

Represents the setting of deleting blank cells/rows/columns.

```javascript
class DeleteBlankOptions extends DeleteOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(DeleteOptions)](#constructor-deleteoptions-)| Constructs from a parent object convertible to this. |
| [constructor()](#constructor--)| Default Constructor. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [emptyStringAsBlank](#emptyStringAsBlank--)| boolean | Indicates whether one cell will be taken as blank when its value is an empty string. Default value is true. |
| [emptyFormulaValueAsBlank](#emptyFormulaValueAsBlank--)| boolean | Whether one cell will be taken as blank when it is a formula and the calculated result is null or empty string. Default value is false. |
| [drawingsAsBlank](#drawingsAsBlank--)| boolean | Indicates whether drawing related objects such as picture, shape, chart... will be taken as blank. Default value is true. |
| [mergedCellsShrinkType](#mergedCellsShrinkType--)| MergedCellsShrinkType | Indicates how to process merged cells when deleting blank rows/columns. |
| [startIndex](#startIndex--)| number | Specifies the start row/column index of the range to check and delete blank row/column. |
| [endIndex](#endIndex--)| number | Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked. |
| [updateReference](#updateReference--)| boolean | Indicates if update references in other worksheets. |
| [formulaChangeMonitor](#formulaChangeMonitor--)| AbstractFormulaChangeMonitor | Gets/sets the monitor for tracking changes caused by the deletion. |


### constructor(DeleteOptions) {#constructor-deleteoptions-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: DeleteOptions);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | DeleteOptions | The parent object. |

### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### emptyStringAsBlank {#emptyStringAsBlank--}

Indicates whether one cell will be taken as blank when its value is an empty string. Default value is true.

```javascript
emptyStringAsBlank : boolean;
```


### emptyFormulaValueAsBlank {#emptyFormulaValueAsBlank--}

Whether one cell will be taken as blank when it is a formula and the calculated result is null or empty string. Default value is false.

```javascript
emptyFormulaValueAsBlank : boolean;
```


**Remarks**

Generally user should make sure the formulas have been calculated before deleting operation with this property as true. Otherwise all newly cretaed formulas by normal apis such as [Cell.Formula](../cell.formula/) will be taken as blank and may be deleted because before calculation their calculated results are all null.

### drawingsAsBlank {#drawingsAsBlank--}

Indicates whether drawing related objects such as picture, shape, chart... will be taken as blank. Default value is true.

```javascript
drawingsAsBlank : boolean;
```


**Remarks**

When setting this property as false, all rows/columns covered by drawing objects will not be taken as blank and will not be deleted.

### mergedCellsShrinkType {#mergedCellsShrinkType--}

Indicates how to process merged cells when deleting blank rows/columns.

```javascript
mergedCellsShrinkType : MergedCellsShrinkType;
```


**Remarks**

For [MergedCellsShrinkType.KeepHeaderOnly](../mergedcellsshrinktype.keepheaderonly/), all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property.<br></br> For [MergedCellsShrinkType.None](../mergedcellsshrinktype.none/), all cells in it will be taken as non-blank.<br></br> For [MergedCellsShrinkType.ShrinkToFit](../mergedcellsshrinktype.shrinktofit/), all cells outside the content display area will be taken as blank.<br></br

### startIndex {#startIndex--}

Specifies the start row/column index of the range to check and delete blank row/column.

```javascript
startIndex : number;
```


### endIndex {#endIndex--}

Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked.

```javascript
endIndex : number;
```


### updateReference {#updateReference--}

Indicates if update references in other worksheets.

```javascript
updateReference : boolean;
```


### formulaChangeMonitor {#formulaChangeMonitor--}

Gets/sets the monitor for tracking changes caused by the deletion.

```javascript
formulaChangeMonitor : AbstractFormulaChangeMonitor;
```



