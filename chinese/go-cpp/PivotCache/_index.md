---
title: "PivotCache 类"
linktitle: "PivotCache"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PivotCache 类。封装在 Go 中表示 pivotcache 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pivotcache/
---

## PivotCache class

表示某些 PivotTable 报表的内存缓存。

```go

type PivotCache struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetMissingItemsLimit](./getmissingitemslimit/) | 获取和设置在丢弃未使用项之前允许的未使用项数量。该值必须大于 -2 且小于 1048577。PivotCacheMissingItemsLimitConst； |
| [SetMissingItemsLimit](./setmissingitemslimit/) | 获取和设置在丢弃未使用项之前允许的未使用项数量。该值必须大于 -2 且小于 1048577。PivotCacheMissingItemsLimitConst； |
| [Refresh_PivotTableRefreshOption](./refresh_pivottablerefreshoption/) | 从数据源刷新数据，并计算所有数据源为此 pivot 缓存的透视表的视图数据。 |
| [Refresh](./refresh/) | 从数据源刷新数据，并计算所有数据源为此 pivot 缓存的透视表的视图数据。 |
| [GetPivotTables](./getpivottables/) | 获取使用此 pivot 缓存的所有透视表。 |
| [Dispose](./dispose/) | 释放所有资源。 |
| [GetSourceType](./getsourcetype/) | 获取 PivotTableSourceType。 |
