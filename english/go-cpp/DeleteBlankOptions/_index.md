---
title: DeleteBlankOptions Class 
linktitle: DeleteBlankOptions
second_title: Aspose.Cells for Go via C++ API Reference
description: 'DeleteBlankOptions class. Encapsulates the object that represents deleteblankoptions in Go.'
type: docs
weight: 200
url: /go-cpp/deleteblankoptions/
---

## DeleteBlankOptions class

Represents the setting of deleting blank cells/rows/columns.

```go

type DeleteBlankOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewDeleteBlankOptions](./newdeleteblankoptions/) | Default constructor. | 
|[NewDeleteBlankOptions_DeleteOptions](./newdeleteblankoptions_deleteoptions/) | Constructs from a parent object. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetEmptyStringAsBlank](./getemptystringasblank/) | Indicates whether one cell will be taken as blank when its value is an empty string.Default value is true. | 
|[SetEmptyStringAsBlank](./setemptystringasblank/) | Indicates whether one cell will be taken as blank when its value is an empty string.Default value is true. | 
|[GetEmptyFormulaValueAsBlank](./getemptyformulavalueasblank/) | Whether one cell will be taken as blank when it is a formula and the calculated result is null or empty string.Default value is false. | 
|[SetEmptyFormulaValueAsBlank](./setemptyformulavalueasblank/) | Whether one cell will be taken as blank when it is a formula and the calculated result is null or empty string.Default value is false. | 
|[GetDrawingsAsBlank](./getdrawingsasblank/) | Indicates whether drawing related objects such as picture, shape, chart... will be taken as blank.Default value is true. | 
|[SetDrawingsAsBlank](./setdrawingsasblank/) | Indicates whether drawing related objects such as picture, shape, chart... will be taken as blank.Default value is true. | 
|[GetMergedCellsShrinkType](./getmergedcellsshrinktype/) | Indicates how to process merged cells when deleting blank rows/columns. | 
|[SetMergedCellsShrinkType](./setmergedcellsshrinktype/) | Indicates how to process merged cells when deleting blank rows/columns. | 
|[GetStartIndex](./getstartindex/) | Specifies the start row/column index of the range to check and delete blank row/column. | 
|[SetStartIndex](./setstartindex/) | Specifies the start row/column index of the range to check and delete blank row/column. | 
|[GetEndIndex](./getendindex/) | Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns.Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked. | 
|[SetEndIndex](./setendindex/) | Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns.Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked. | 
|[GetUpdateReference](./getupdatereference/) | Indicates if update references in other worksheets. | 
|[SetUpdateReference](./setupdatereference/) | Indicates if update references in other worksheets. | 
|[GetFormulaChangeMonitor](./getformulachangemonitor/) | Gets/sets the monitor for tracking changes caused by the deletion. | 
|[SetFormulaChangeMonitor](./setformulachangemonitor/) | Gets/sets the monitor for tracking changes caused by the deletion. | 
