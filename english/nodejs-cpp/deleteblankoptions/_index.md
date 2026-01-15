---
title: DeleteBlankOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the setting of deleting blank cellsrowscolumns.
type: docs
url: /nodejs-cpp/deleteblankoptions/
---

## DeleteBlankOptions class

Represents the setting of deleting blank cells/rows/columns.

```javascript
class DeleteBlankOptions extends DeleteOptions;
```


## Constructors

| Constructor | Description |
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

## Methods

| Method | Description |
| --- | --- |
| [getEmptyStringAsBlank()](#getEmptyStringAsBlank--)| <b>@deprecated.</b> Please use the 'emptyStringAsBlank' property instead. Indicates whether one cell will be taken as blank when its value is an empty string. Default value is true. |
| [setEmptyStringAsBlank(boolean)](#setEmptyStringAsBlank-boolean-)| <b>@deprecated.</b> Please use the 'emptyStringAsBlank' property instead. Indicates whether one cell will be taken as blank when its value is an empty string. Default value is true. |
| [getEmptyFormulaValueAsBlank()](#getEmptyFormulaValueAsBlank--)| <b>@deprecated.</b> Please use the 'emptyFormulaValueAsBlank' property instead. Whether one cell will be taken as blank when it is a formula and the calculated result is null or empty string. Default value is false. |
| [setEmptyFormulaValueAsBlank(boolean)](#setEmptyFormulaValueAsBlank-boolean-)| <b>@deprecated.</b> Please use the 'emptyFormulaValueAsBlank' property instead. Whether one cell will be taken as blank when it is a formula and the calculated result is null or empty string. Default value is false. |
| [getDrawingsAsBlank()](#getDrawingsAsBlank--)| <b>@deprecated.</b> Please use the 'drawingsAsBlank' property instead. Indicates whether drawing related objects such as picture, shape, chart... will be taken as blank. Default value is true. |
| [setDrawingsAsBlank(boolean)](#setDrawingsAsBlank-boolean-)| <b>@deprecated.</b> Please use the 'drawingsAsBlank' property instead. Indicates whether drawing related objects such as picture, shape, chart... will be taken as blank. Default value is true. |
| [getMergedCellsShrinkType()](#getMergedCellsShrinkType--)| <b>@deprecated.</b> Please use the 'mergedCellsShrinkType' property instead. Indicates how to process merged cells when deleting blank rows/columns. |
| [setMergedCellsShrinkType(MergedCellsShrinkType)](#setMergedCellsShrinkType-mergedcellsshrinktype-)| <b>@deprecated.</b> Please use the 'mergedCellsShrinkType' property instead. Indicates how to process merged cells when deleting blank rows/columns. |
| [getStartIndex()](#getStartIndex--)| <b>@deprecated.</b> Please use the 'startIndex' property instead. Specifies the start row/column index of the range to check and delete blank row/column. |
| [setStartIndex(number)](#setStartIndex-number-)| <b>@deprecated.</b> Please use the 'startIndex' property instead. Specifies the start row/column index of the range to check and delete blank row/column. |
| [getEndIndex()](#getEndIndex--)| <b>@deprecated.</b> Please use the 'endIndex' property instead. Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked. |
| [setEndIndex(number)](#setEndIndex-number-)| <b>@deprecated.</b> Please use the 'endIndex' property instead. Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getUpdateReference()](#getUpdateReference--)| <b>@deprecated.</b> Please use the 'updateReference' property instead. Indicates if update references in other worksheets. |
| [setUpdateReference(boolean)](#setUpdateReference-boolean-)| <b>@deprecated.</b> Please use the 'updateReference' property instead. Indicates if update references in other worksheets. |
| [getFormulaChangeMonitor()](#getFormulaChangeMonitor--)| <b>@deprecated.</b> Please use the 'formulaChangeMonitor' property instead. Gets/sets the monitor for tracking changes caused by the deletion. |
| [setFormulaChangeMonitor(AbstractFormulaChangeMonitor)](#setFormulaChangeMonitor-abstractformulachangemonitor-)| <b>@deprecated.</b> Please use the 'formulaChangeMonitor' property instead. Gets/sets the monitor for tracking changes caused by the deletion. |


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


### getEmptyStringAsBlank() {#getEmptyStringAsBlank--}

<b>@deprecated.</b> Please use the 'emptyStringAsBlank' property instead. Indicates whether one cell will be taken as blank when its value is an empty string. Default value is true.

```javascript
getEmptyStringAsBlank() : boolean;
```


### setEmptyStringAsBlank(boolean) {#setEmptyStringAsBlank-boolean-}

<b>@deprecated.</b> Please use the 'emptyStringAsBlank' property instead. Indicates whether one cell will be taken as blank when its value is an empty string. Default value is true.

```javascript
setEmptyStringAsBlank(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getEmptyFormulaValueAsBlank() {#getEmptyFormulaValueAsBlank--}

<b>@deprecated.</b> Please use the 'emptyFormulaValueAsBlank' property instead. Whether one cell will be taken as blank when it is a formula and the calculated result is null or empty string. Default value is false.

```javascript
getEmptyFormulaValueAsBlank() : boolean;
```


**Remarks**

Generally user should make sure the formulas have been calculated before deleting operation with this property as true. Otherwise all newly cretaed formulas by normal apis such as [Cell.Formula](../cell.formula/) will be taken as blank and may be deleted because before calculation their calculated results are all null.

### setEmptyFormulaValueAsBlank(boolean) {#setEmptyFormulaValueAsBlank-boolean-}

<b>@deprecated.</b> Please use the 'emptyFormulaValueAsBlank' property instead. Whether one cell will be taken as blank when it is a formula and the calculated result is null or empty string. Default value is false.

```javascript
setEmptyFormulaValueAsBlank(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Generally user should make sure the formulas have been calculated before deleting operation with this property as true. Otherwise all newly cretaed formulas by normal apis such as [Cell.Formula](../cell.formula/) will be taken as blank and may be deleted because before calculation their calculated results are all null.

### getDrawingsAsBlank() {#getDrawingsAsBlank--}

<b>@deprecated.</b> Please use the 'drawingsAsBlank' property instead. Indicates whether drawing related objects such as picture, shape, chart... will be taken as blank. Default value is true.

```javascript
getDrawingsAsBlank() : boolean;
```


**Remarks**

When setting this property as false, all rows/columns covered by drawing objects will not be taken as blank and will not be deleted.

### setDrawingsAsBlank(boolean) {#setDrawingsAsBlank-boolean-}

<b>@deprecated.</b> Please use the 'drawingsAsBlank' property instead. Indicates whether drawing related objects such as picture, shape, chart... will be taken as blank. Default value is true.

```javascript
setDrawingsAsBlank(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

When setting this property as false, all rows/columns covered by drawing objects will not be taken as blank and will not be deleted.

### getMergedCellsShrinkType() {#getMergedCellsShrinkType--}

<b>@deprecated.</b> Please use the 'mergedCellsShrinkType' property instead. Indicates how to process merged cells when deleting blank rows/columns.

```javascript
getMergedCellsShrinkType() : MergedCellsShrinkType;
```


**Returns**

[MergedCellsShrinkType](../mergedcellsshrinktype/)

**Remarks**

For [MergedCellsShrinkType.KeepHeaderOnly](../mergedcellsshrinktype.keepheaderonly/), all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property.<br></br> For [MergedCellsShrinkType.None](../mergedcellsshrinktype.none/), all cells in it will be taken as non-blank.<br></br> For [MergedCellsShrinkType.ShrinkToFit](../mergedcellsshrinktype.shrinktofit/), all cells outside the content display area will be taken as blank.<br></br

### setMergedCellsShrinkType(MergedCellsShrinkType) {#setMergedCellsShrinkType-mergedcellsshrinktype-}

<b>@deprecated.</b> Please use the 'mergedCellsShrinkType' property instead. Indicates how to process merged cells when deleting blank rows/columns.

```javascript
setMergedCellsShrinkType(value: MergedCellsShrinkType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MergedCellsShrinkType](../mergedcellsshrinktype/) | The value to set. |

**Remarks**

For [MergedCellsShrinkType.KeepHeaderOnly](../mergedcellsshrinktype.keepheaderonly/), all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property.<br></br> For [MergedCellsShrinkType.None](../mergedcellsshrinktype.none/), all cells in it will be taken as non-blank.<br></br> For [MergedCellsShrinkType.ShrinkToFit](../mergedcellsshrinktype.shrinktofit/), all cells outside the content display area will be taken as blank.<br></br

### getStartIndex() {#getStartIndex--}

<b>@deprecated.</b> Please use the 'startIndex' property instead. Specifies the start row/column index of the range to check and delete blank row/column.

```javascript
getStartIndex() : number;
```


### setStartIndex(number) {#setStartIndex-number-}

<b>@deprecated.</b> Please use the 'startIndex' property instead. Specifies the start row/column index of the range to check and delete blank row/column.

```javascript
setStartIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getEndIndex() {#getEndIndex--}

<b>@deprecated.</b> Please use the 'endIndex' property instead. Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked.

```javascript
getEndIndex() : number;
```


### setEndIndex(number) {#setEndIndex-number-}

<b>@deprecated.</b> Please use the 'endIndex' property instead. Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked.

```javascript
setEndIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getUpdateReference() {#getUpdateReference--}

<b>@deprecated.</b> Please use the 'updateReference' property instead. Indicates if update references in other worksheets.

```javascript
getUpdateReference() : boolean;
```


### setUpdateReference(boolean) {#setUpdateReference-boolean-}

<b>@deprecated.</b> Please use the 'updateReference' property instead. Indicates if update references in other worksheets.

```javascript
setUpdateReference(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFormulaChangeMonitor() {#getFormulaChangeMonitor--}

<b>@deprecated.</b> Please use the 'formulaChangeMonitor' property instead. Gets/sets the monitor for tracking changes caused by the deletion.

```javascript
getFormulaChangeMonitor() : AbstractFormulaChangeMonitor;
```


**Returns**

[AbstractFormulaChangeMonitor](../abstractformulachangemonitor/)

### setFormulaChangeMonitor(AbstractFormulaChangeMonitor) {#setFormulaChangeMonitor-abstractformulachangemonitor-}

<b>@deprecated.</b> Please use the 'formulaChangeMonitor' property instead. Gets/sets the monitor for tracking changes caused by the deletion.

```javascript
setFormulaChangeMonitor(value: AbstractFormulaChangeMonitor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractFormulaChangeMonitor](../abstractformulachangemonitor/) | The value to set. |


