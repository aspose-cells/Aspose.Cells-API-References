---
title: "DeleteBlankOptions Class"
linktitle: "DeleteBlankOptions"
articleTitle: "DeleteBlankOptions"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the setting of deleting blank cells/rows/columns."
type: docs
weight: 1710
url: /python-java/asposecells.api/deleteblankoptions/
---

## DeleteBlankOptions class

Represents the setting of deleting blank cells/rows/columns.

## Constructors

| Name | Description |
| --- | --- |
| [DeleteBlankOptions](#constructor) |  |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [EmptyStringAsBlank](#emptystringasblank) | boolean | Whether one cell will be taken as blank when its value is empty string. Default value is true. |
| [EmptyFormulaValueAsBlank](#emptyformulavalueasblank) | boolean | Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default va |
| [DrawingsAsBlank](#drawingsasblank) | boolean |  |
| [MergedCellsShrinkType](#mergedcellsshrinktype) | int | The value of the property is MergedCellsShrinkType integer constant. |
| [StartIndex](#startindex) | int |  |
| [EndIndex](#endindex) | int |  |
| [UpdateReference](#updatereference) | boolean | Indicates if update references in other worksheets. |
| [FormulaChangeMonitor](#formulachangemonitor) | AbstractFormulaChangeMonitor |  |

### DeleteBlankOptions() {#constructor}

### DeleteBlankOptions.EmptyStringAsBlank property {#emptystringasblank}

Whether one cell will be taken as blank when its value is empty string. Default value is true.

**Type:** boolean

### DeleteBlankOptions.EmptyFormulaValueAsBlank property {#emptyformulavalueasblank}

Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false. Generally user should make sure the formulas have been calculated before deleting operation with this property as true. Otherwise all newly cretaed formulas by normal apis such as Cell.Formula will be taken as blank and may be deleted because before calculation their calculated results are all null.

**Type:** boolean

### DeleteBlankOptions.DrawingsAsBlank property {#drawingsasblank}

**Type:** boolean

### DeleteBlankOptions.MergedCellsShrinkType property {#mergedcellsshrinktype}

The value of the property is MergedCellsShrinkType integer constant.

**Type:** int

### DeleteBlankOptions.StartIndex property {#startindex}

**Type:** int

### DeleteBlankOptions.EndIndex property {#endindex}

**Type:** int

### DeleteBlankOptions.UpdateReference property {#updatereference}

Indicates if update references in other worksheets.

**Type:** boolean

### DeleteBlankOptions.FormulaChangeMonitor property {#formulachangemonitor}

**Type:** AbstractFormulaChangeMonitor
