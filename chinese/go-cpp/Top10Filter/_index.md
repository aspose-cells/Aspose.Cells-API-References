---
title: "Top10Filter 类"
linktitle: "Top10Filter"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Top10Filter 类。封装了在 Go 中表示 top10filter 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/top10filter/
---

## Top10Filter class

表示要过滤的前 N（百分比或项目数量）。

```go

type Top10Filter struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewTop10Filter](./newtop10filter/) | 从可转换为此对象的 Object 构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [ToObject](./toobject/) | 获取对象。 |
| [IsTop](./istop/) | 指示是否按顶部顺序进行过滤 |
| [SetIsTop](./setistop/) | 指示是否按顶部顺序进行过滤 |
| [IsPercent](./ispercent/) | 指示是否按列的百分比值进行过滤 |
| [SetIsPercent](./setispercent/) | 指示是否按列的百分比值进行过滤 |
| [GetItems](./getitems/) | 获取并设置用作过滤条件的顶部或底部值。 |
| [SetItems](./setitems/) | 获取并设置用作过滤条件的顶部或底部值。 |
