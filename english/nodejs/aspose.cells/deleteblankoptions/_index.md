---
title: "DeleteBlankOptions"
linktitle: "DeleteBlankOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the setting of deleting blank cells/rows/columns."
type: docs
weight: 1120
url: /nodejs/aspose.cells/deleteblankoptions/
---

## DeleteBlankOptions class

Represents the setting of deleting blank cells/rows/columns.

```js
new DeleteBlankOptions()
```

## Methods

| Name | Description |
| --- | --- |
| [getDrawingsAsBlank()](#getdrawingsasblank) |  |
| [getEmptyFormulaValueAsBlank()](#getemptyformulavalueasblank) | Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default va |
| [getEmptyStringAsBlank()](#getemptystringasblank) | Whether one cell will be taken as blank when its value is empty string. Default value is true. |
| [getEndIndex()](#getendindex) |  |
| [getFormulaChangeMonitor()](#getformulachangemonitor) |  |
| [getMergedCellsShrinkType()](#getmergedcellsshrinktype) | The value of the property is MergedCellsShrinkType integer constant. |
| [getStartIndex()](#getstartindex) |  |
| [getUpdateReference()](#getupdatereference) | Indicates if update references in other worksheets. |
| [setDrawingsAsBlank()](#setdrawingsasblank) |  |
| [setEmptyFormulaValueAsBlank()](#setemptyformulavalueasblank) | Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default va |
| [setEmptyStringAsBlank()](#setemptystringasblank) | Whether one cell will be taken as blank when its value is empty string. Default value is true. |
| [setEndIndex()](#setendindex) |  |
| [setFormulaChangeMonitor()](#setformulachangemonitor) |  |
| [setMergedCellsShrinkType()](#setmergedcellsshrinktype) | The value of the property is MergedCellsShrinkType integer constant. |
| [setStartIndex()](#setstartindex) |  |
| [setUpdateReference()](#setupdatereference) | Indicates if update references in other worksheets. |

### getDrawingsAsBlank() {#getdrawingsasblank}

### getEmptyFormulaValueAsBlank() {#getemptyformulavalueasblank}

Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false. Generally user should make sure the formulas have been calculated before deleting operation with this property as true. Otherwise all newly cretaed formulas by normal apis such as Cell.Formula will be taken as blank and may be deleted because before calculation their calculated results are all null.

### getEmptyStringAsBlank() {#getemptystringasblank}

Whether one cell will be taken as blank when its value is empty string. Default value is true.

### getEndIndex() {#getendindex}

### getFormulaChangeMonitor() {#getformulachangemonitor}

### getMergedCellsShrinkType() {#getmergedcellsshrinktype}

The value of the property is MergedCellsShrinkType integer constant.

### getStartIndex() {#getstartindex}

### getUpdateReference() {#getupdatereference}

Indicates if update references in other worksheets.

### setDrawingsAsBlank() {#setdrawingsasblank}

### setEmptyFormulaValueAsBlank() {#setemptyformulavalueasblank}

Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false. Generally user should make sure the formulas have been calculated before deleting operation with this property as true. Otherwise all newly cretaed formulas by normal apis such as Cell.Formula will be taken as blank and may be deleted because before calculation their calculated results are all null.

### setEmptyStringAsBlank() {#setemptystringasblank}

Whether one cell will be taken as blank when its value is empty string. Default value is true.

### setEndIndex() {#setendindex}

### setFormulaChangeMonitor() {#setformulachangemonitor}

### setMergedCellsShrinkType() {#setmergedcellsshrinktype}

The value of the property is MergedCellsShrinkType integer constant.

### setStartIndex() {#setstartindex}

### setUpdateReference() {#setupdatereference}

Indicates if update references in other worksheets.
