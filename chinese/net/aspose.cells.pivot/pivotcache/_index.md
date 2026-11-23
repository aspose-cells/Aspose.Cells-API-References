---
title: "类 PivotCache"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Pivot.PivotCache 类。表示某些 PivotTable 报表的内存缓存"
type: docs
url: /zh/net/aspose.cells.pivot/pivotcache/
---
## PivotCache class

表示某些 PivotTable 报表的内存缓存。

```csharp
public abstract class PivotCache : IDisposable
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [MissingItemsLimit](../../aspose.cells.pivot/pivotcache/missingitemslimit/) { get; set; } | 获取并设置在丢弃未使用项之前允许的未使用项数量。此值必须大于 -2 且小于 1048577。[`PivotCacheMissingItemsLimitConst`](../pivotcachemissingitemslimitconst/); |
| abstract [SourceType](../../aspose.cells.pivot/pivotcache/sourcetype/) { get; } | 获取 [`PivotTableSourceType`](../pivottablesourcetype/)。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| abstract [Dispose](../../aspose.cells.pivot/pivotcache/dispose/)() | 释放所有资源。 |
| [GetPivotTables](../../aspose.cells.pivot/pivotcache/getpivottables/)() | 获取使用此数据透视缓存的所有数据透视表。 |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh)() | 从数据源刷新数据，并为所有数据源为此数据透视缓存的数据透视表的视图计算数据。 |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh_1)(PivotTableRefreshOption) | 从数据源刷新数据，并为所有数据源为此数据透视缓存的数据透视表的视图计算数据。 |

### 备注

所有数据将被收集到此缓存中，数据透视表仅从该缓存获取数据，而不直接访问数据源。如果某些[`PivotTable`](../pivottable/)的数据源相同，它们将使用同一个数据透视缓存。

### 另请参见

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


