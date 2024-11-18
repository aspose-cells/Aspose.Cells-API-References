---
title: DeleteBlankOptions Class 
linktitle: DeleteBlankOptions
second_title: Aspose.Cells for Go API Reference
description: 'DeleteBlankOptions class. Encapsulates the object that represents deleteblankoptions in Go.'
type: docs
weight: 200
url: /go/aspose.cells/deleteblankoptions/
---

## DeleteBlankOptions class

Represents the setting of deleting blank cells/rows/columns.

```go

type DeleteBlankOptions struct 

deleteblankoptions, _ := asposecells.NewDeleteBlankOptions()

```

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetEmptyStringAsBlank](./getemptystringasblank/) | Whether one cell will be taken as blank when its value is empty string. Default value is true. | 
|[SetEmptyStringAsBlank](./setemptystringasblank/) | Whether one cell will be taken as blank when its value is empty string. Default value is true. | 
|[GetEmptyFormulaValueAsBlank](./getemptyformulavalueasblank/) | Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false. | 
|[SetEmptyFormulaValueAsBlank](./setemptyformulavalueasblank/) | Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false. | 
|[GetMergedCellsShrinkType](./getmergedcellsshrinktype/) | Indicates how to process merged cells when deleting blank rows/columns.<br></br>For <see cref="MergedCellsShrinkType.KeepHeaderOnly"/>, all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property.<br></br>For <see cref="MergedCellsShrinkType.None"/>, all cells in it will be taken as non-blank.<br></br>For <see cref="MergedCellsShrinkType.ShrinkToFit"/>, all cells outside the content display area will be taken as blank.<br></br> | 
|[SetMergedCellsShrinkType](./setmergedcellsshrinktype/) | Indicates how to process merged cells when deleting blank rows/columns.<br></br>For <see cref="MergedCellsShrinkType.KeepHeaderOnly"/>, all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property.<br></br>For <see cref="MergedCellsShrinkType.None"/>, all cells in it will be taken as non-blank.<br></br>For <see cref="MergedCellsShrinkType.ShrinkToFit"/>, all cells outside the content display area will be taken as blank.<br></br> | 
|[GetUpdateReference](./getupdatereference/) | Indicates if update references in other worksheets. | 
|[SetUpdateReference](./setupdatereference/) | Indicates if update references in other worksheets. | 
