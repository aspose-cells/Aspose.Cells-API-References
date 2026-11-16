---
title: "PivotTableRefreshOption 类"
linktitle: "PivotTableRefreshOption"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PivotTableRefreshOption 类。封装了在 Go 中表示 pivottablerefreshoption 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pivottablerefreshoption/
---

## PivotTableRefreshOption class

表示刷新数据透视表数据源的选项。

```go

type PivotTableRefreshOption struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewPivotTableRefreshOption](./newpivottablerefreshoption/) | 表示刷新数据透视表数据源的选项。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetReserveMissingPivotItemType](./getreservemissingpivotitemtype/) | 表示如何保留缺失的透视项。 |
| [SetReserveMissingPivotItemType](./setreservemissingpivotitemtype/) | 表示如何保留缺失的透视项。 |
| [IsKeepOriginalOrder](./iskeeporiginalorder/) | 指示是否保持透视表项的原始顺序（与旧数据源相同）。 |
| [SetIsKeepOriginalOrder](./setiskeeporiginalorder/) | 指示是否保持透视表项的原始顺序（与旧数据源相同）。 |
| [GetKeepCachedLocalGroupData](./getkeepcachedlocalgroupdata/) | 指示在最大值和最小值保持不变的情况下是否保留缓存的本地分组数据。默认值为 false，表示使用本地设置刷新分组。 |
| [SetKeepCachedLocalGroupData](./setkeepcachedlocalgroupdata/) | 指示在最大值和最小值保持不变的情况下是否保留缓存的本地分组数据。默认值为 false，表示使用本地设置刷新分组。 |
