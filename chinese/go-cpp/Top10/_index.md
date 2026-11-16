---
title: "Top10 类"
linktitle: "Top10"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Top10 类。封装在 Go 中表示 top10 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/top10/
---

## Top10 class

描述 Top10 条件格式规则。此条件格式规则突出显示其值落在指定的前 N 或后 N 区间的单元格。

```go

type Top10 struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewTop10](./newtop10/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [IsPercent](./ispercent/) | 获取或设置 "top/bottom n" 规则是否为 "top/bottom n percent" 规则。默认值为 false。 |
| [SetIsPercent](./setispercent/) | 获取或设置 "top/bottom n" 规则是否为 "top/bottom n percent" 规则。默认值为 false。 |
| [IsBottom](./isbottom/) | 获取或设置 "top/bottom n" 规则是否为 "bottom n" 规则。默认值为 false。 |
| [SetIsBottom](./setisbottom/) | 获取或设置 "top/bottom n" 规则是否为 "bottom n" 规则。默认值为 false。 |
| [GetRank](./getrank/) | 获取或设置 "top/bottom n" 条件格式规则中 "n" 的值。如果 IsPercent 为 true，则该值必须在 0 到 100 之间。否则必须在 0 到 1000 之间。默认值为 10。 |
| [SetRank](./setrank/) | 获取或设置 "top/bottom n" 条件格式规则中 "n" 的值。如果 IsPercent 为 true，则该值必须在 0 到 100 之间。否则必须在 0 到 1000 之间。默认值为 10。 |
