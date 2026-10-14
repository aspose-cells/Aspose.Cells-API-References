---
title: PivotCache Class 
linktitle: PivotCache
second_title: Aspose.Cells for Go via C++ API Reference
description: 'PivotCache class. Encapsulates the object that represents pivotcache in Go.'
type: docs
weight: 200
url: /go-cpp/pivotcache/
---

## PivotCache class

Represents the memory cache for some PivotTable reports.

```go

type PivotCache struct  {
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
|[GetMissingItemsLimit](./getmissingitemslimit/) | Gets and sets the number of unused items to allow before discarding unused items.This value MUST be greater than -2 and less than 1048577.PivotCacheMissingItemsLimitConst; | 
|[SetMissingItemsLimit](./setmissingitemslimit/) | Gets and sets the number of unused items to allow before discarding unused items.This value MUST be greater than -2 and less than 1048577.PivotCacheMissingItemsLimitConst; | 
|[Refresh_PivotTableRefreshOption](./refresh_pivottablerefreshoption/) | Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache. | 
|[Refresh](./refresh/) | Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache. | 
|[GetPivotTables](./getpivottables/) | Gets all pivot tables with this pivot cache. | 
|[Dispose](./dispose/) | Release all resource. | 
|[GetSourceType](./getsourcetype/) | Gets the PivotTableSourceType. | 
