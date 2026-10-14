---
title: PivotFieldSortSetting Class 
linktitle: PivotFieldSortSetting
second_title: Aspose.Cells for Go via C++ API Reference
description: 'PivotFieldSortSetting class. Encapsulates the object that represents pivotfieldsortsetting in Go.'
type: docs
weight: 200
url: /go-cpp/pivotfieldsortsetting/
---

## PivotFieldSortSetting class

Represents the setting for sorting pivot fields.

```go

type PivotFieldSortSetting struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetSortType](./getsorttype/) | Represents the SortOrder. | 
|[SetSortType](./setsorttype/) | Represents the SortOrder. | 
|[IsSortByLabels](./issortbylabels/) | Indicates whether to sort the field by itself or data field. | 
|[GetSortBy](./getsortby/) | Represents the index of the field sorted by.A value of -1 indicates sorting by the pivot item's own values.When greater than or equal to zero, it represents the index of data field in the data region. | 
|[SetSortBy](./setsortby/) | Represents the index of the field sorted by.A value of -1 indicates sorting by the pivot item's own values.When greater than or equal to zero, it represents the index of data field in the data region. | 
|[GetLineTypeSortedBy](./getlinetypesortedby/) | The pivot line type sorted by. | 
|[IsSimpleSort](./issimplesort/) | Indicates whether a simple data sort operation will be applied. | 
|[SetIsSimpleSort](./setissimplesort/) | Indicates whether a simple data sort operation will be applied. | 
|[GetCell](./getcell/) | Sorts by the values in which row or column. | 
