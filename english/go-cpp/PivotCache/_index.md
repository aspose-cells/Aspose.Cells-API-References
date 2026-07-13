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
|[Refresh_PivotTableRefreshOption](./refresh_pivottablerefreshoption/) | Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache. | 
|[Refresh](./refresh/) | Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache. | 
|[GetPivotTables](./getpivottables/) | Gets all pivot tables with this pivot cache. | 
|[Dispose](./dispose/) | Release all resource. | 
|[GetSourceType](./getsourcetype/) | Gets the PivotTableSourceType. | 
