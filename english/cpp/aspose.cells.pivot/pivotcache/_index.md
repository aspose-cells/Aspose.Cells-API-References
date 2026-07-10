---
title: Aspose::Cells::Pivot::PivotCache class
linktitle: PivotCache
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotCache class. Represents the memory cache for some PivotTable reports in C++.'
type: docs
weight: 600
url: /cpp/aspose.cells.pivot/pivotcache/
---
## PivotCache class


Represents the memory cache for some [PivotTable](../pivottable/) reports.

```cpp
class PivotCache
```

## Methods

| Method | Description |
| --- | --- |
| virtual [Dispose()](./dispose/) | Release all resource. |
| [GetPivotTables()](./getpivottables/) | Gets all pivot tables with this pivot cache. |
| virtual [GetSourceType()](./getsourcetype/) | Gets the [PivotTableSourceType](../pivottablesourcetype/). |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotCache\& src)](./operator_asm/) | operator= |
| [PivotCache(PivotCache_Impl* impl)](./pivotcache/) | Constructs from an implementation object. |
| [PivotCache(const PivotCache\& src)](./pivotcache/) | Copy constructor. |
| [Refresh(const PivotTableRefreshOption\& option)](./refresh/) | Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache. |
| [Refresh()](./refresh/) | Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache. |
| [~PivotCache()](./~pivotcache/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Remarks


All data will be gathered into this cache,and the pivot table only get data from this cache,not directly access data source. If data source of some [PivotTable](../pivottable/)s are same, they will use a pivot cache. 
## See Also

* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
