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

| Name | Description |
| --- | --- |
| [constructor(DeleteOptions)](#constructor-deleteoptions-)| Constructs from a parent object convertible to this. |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getEmptyStringAsBlank()](#getEmptyStringAsBlank--)| Whether one cell will be taken as blank when its value is empty string. Default value is true. |
| [setEmptyStringAsBlank(boolean)](#setEmptyStringAsBlank-boolean-)| Whether one cell will be taken as blank when its value is empty string. Default value is true. |
| [getEmptyFormulaValueAsBlank()](#getEmptyFormulaValueAsBlank--)| Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false. |
| [setEmptyFormulaValueAsBlank(boolean)](#setEmptyFormulaValueAsBlank-boolean-)| Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false. |
| [getDrawingsAsBlank()](#getDrawingsAsBlank--)| Whether drawing related objects such as picture, shape, chart... will be taken as blank. Default value is true. |
| [setDrawingsAsBlank(boolean)](#setDrawingsAsBlank-boolean-)| Whether drawing related objects such as picture, shape, chart... will be taken as blank. Default value is true. |
| [getMergedCellsShrinkType()](#getMergedCellsShrinkType--)| Indicates how to process merged cells when deleting blank rows/columns. |
| [setMergedCellsShrinkType(MergedCellsShrinkType)](#setMergedCellsShrinkType-mergedcellsshrinktype-)| Indicates how to process merged cells when deleting blank rows/columns. |
| [getStartIndex()](#getStartIndex--)| Specifies the start row/column index of the range to check and delete blank rows/columns. |
| [setStartIndex(number)](#setStartIndex-number-)| Specifies the start row/column index of the range to check and delete blank rows/columns. |
| [getEndIndex()](#getEndIndex--)| Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked. |
| [setEndIndex(number)](#setEndIndex-number-)| Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getUpdateReference()](#getUpdateReference--)| Indicates if update references in other worksheets. |
| [setUpdateReference(boolean)](#setUpdateReference-boolean-)| Indicates if update references in other worksheets. |
| [getFormulaChangeMonitor()](#getFormulaChangeMonitor--)| Gets/sets the monitor for tracking changes caused by the deletion. |
| [setFormulaChangeMonitor(AbstractFormulaChangeMonitor)](#setFormulaChangeMonitor-abstractformulachangemonitor-)| Gets/sets the monitor for tracking changes caused by the deletion. |


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


### getEmptyStringAsBlank() {#getEmptyStringAsBlank--}

Whether one cell will be taken as blank when its value is empty string. Default value is true.

```javascript
getEmptyStringAsBlank() : boolean;
```


### setEmptyStringAsBlank(boolean) {#setEmptyStringAsBlank-boolean-}

Whether one cell will be taken as blank when its value is empty string. Default value is true.

```javascript
setEmptyStringAsBlank(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getEmptyFormulaValueAsBlank() {#getEmptyFormulaValueAsBlank--}

Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false.

```javascript
getEmptyFormulaValueAsBlank() : boolean;
```


**Remarks**

Generally user should make sure the formulas have been calculated before deleting operation with this property as true. Otherwise all newly cretaed formulas by normal apis such as [Cell.Formula](../cell.formula/) will be taken as blank and may be deleted because before calculation their calculated results are all null.

### setEmptyFormulaValueAsBlank(boolean) {#setEmptyFormulaValueAsBlank-boolean-}

Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false.

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

Whether drawing related objects such as picture, shape, chart... will be taken as blank. Default value is true.

```javascript
getDrawingsAsBlank() : boolean;
```


**Remarks**

When setting this property as false, all rows/columns covered by drawing objects will not be taken as blank and will not be deleted.

### setDrawingsAsBlank(boolean) {#setDrawingsAsBlank-boolean-}

Whether drawing related objects such as picture, shape, chart... will be taken as blank. Default value is true.

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

Indicates how to process merged cells when deleting blank rows/columns.

```javascript
getMergedCellsShrinkType() : MergedCellsShrinkType;
```


**Returns**

[MergedCellsShrinkType](../mergedcellsshrinktype/)

**Remarks**

For [MergedCellsShrinkType.KeepHeaderOnly](../mergedcellsshrinktype.keepheaderonly/), all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property.<br></br> For [MergedCellsShrinkType.None](../mergedcellsshrinktype.none/), all cells in it will be taken as non-blank.<br></br> For [MergedCellsShrinkType.ShrinkToFit](../mergedcellsshrinktype.shrinktofit/), all cells outside the content display area will be taken as blank.<br></br

### setMergedCellsShrinkType(MergedCellsShrinkType) {#setMergedCellsShrinkType-mergedcellsshrinktype-}

Indicates how to process merged cells when deleting blank rows/columns.

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

Specifies the start row/column index of the range to check and delete blank rows/columns.

```javascript
getStartIndex() : number;
```


### setStartIndex(number) {#setStartIndex-number-}

Specifies the start row/column index of the range to check and delete blank rows/columns.

```javascript
setStartIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getEndIndex() {#getEndIndex--}

Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked.

```javascript
getEndIndex() : number;
```


### setEndIndex(number) {#setEndIndex-number-}

Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked.

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

Indicates if update references in other worksheets.

```javascript
getUpdateReference() : boolean;
```


### setUpdateReference(boolean) {#setUpdateReference-boolean-}

Indicates if update references in other worksheets.

```javascript
setUpdateReference(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getFormulaChangeMonitor() {#getFormulaChangeMonitor--}

Gets/sets the monitor for tracking changes caused by the deletion.

```javascript
getFormulaChangeMonitor() : AbstractFormulaChangeMonitor;
```


**Returns**

[AbstractFormulaChangeMonitor](../abstractformulachangemonitor/)

### setFormulaChangeMonitor(AbstractFormulaChangeMonitor) {#setFormulaChangeMonitor-abstractformulachangemonitor-}

Gets/sets the monitor for tracking changes caused by the deletion.

```javascript
setFormulaChangeMonitor(value: AbstractFormulaChangeMonitor) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractFormulaChangeMonitor](../abstractformulachangemonitor/) | The value to set. |


