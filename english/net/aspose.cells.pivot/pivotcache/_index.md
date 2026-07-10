---
title: Class PivotCache
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotCache class. Represents the memory cache for some PivotTable reports
type: docs
url: /net/aspose.cells.pivot/pivotcache/
---
## PivotCache class

Represents the memory cache for some PivotTable reports.

```csharp
public abstract class PivotCache : IDisposable
```

## Properties

| Name | Description |
| --- | --- |
| abstract [SourceType](../../aspose.cells.pivot/pivotcache/sourcetype/) { get; } | Gets the [`PivotTableSourceType`](../pivottablesourcetype/). |

## Methods

| Name | Description |
| --- | --- |
| abstract [Dispose](../../aspose.cells.pivot/pivotcache/dispose/)() | Release all resource. |
| [GetPivotTables](../../aspose.cells.pivot/pivotcache/getpivottables/)() | Gets all pivot tables with this pivot cache. |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh)() | Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache. |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh_1)(PivotTableRefreshOption) | Refreshes data from the data source and calculates data for the view of all pivottables which data source is this pivot cache. |

### Remarks

All data will be gathered into this cache,and the pivot table only get data from this cache,not directly access data source. If data source of some [`PivotTable`](../pivottable/)s are same, they will use a pivot cache.

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


