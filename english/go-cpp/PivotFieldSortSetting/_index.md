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
|[IsSortByLabels](./issortbylabels/) | Indicates whether to sort the field by itself or data field. | 
|[GetFieldIndex](./getfieldindex/) | Represents the index of the field sorted by.-1 means sorting the PivotField by the labels,others means sorting by the data field. | 
|[GetLineTypeSortedBy](./getlinetypesortedby/) | The pivot line type sorted by. | 
|[IsSimpleSort](./issimplesort/) | Indicates whether a simple data sort operation will be applied. | 
|[GetCell](./getcell/) | Sorts by the values in which row or column. | 
