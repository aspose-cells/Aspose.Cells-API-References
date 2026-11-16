---
title: "ChartSplitType 枚举"
linktitle: "ChartSplitType"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ChartSplitType 枚举。封装在 Go 中表示 chartsplittype 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/chartsplittype/
---

## ChartSplitType Enum

表示饼中饼图或条形饼图的两个部分的分割方式。

```go

type ChartSplitType int32


```

## 字段

| 字段 | 描述 |
| --- | --- |
| [Position](./position/) | 表示数据点。数据点应通过将数据点的最后拆分位置放入第二个图表来在饼图和第二个图表之间拆分。 |
| [Value](./value/) | 表示数据点应通过将值小于拆分位置的数据点放入第二个图表，在饼图和第二个图表之间拆分。 |
| [PercentValue](./percentvalue/) | 表示应通过将百分比低于拆分位置百分比的点放入第二个图表，在饼图和第二个图表之间拆分的数据点。 |
| [Custom](./custom/) | 表示应根据自定义拆分值在饼图和第二个图表之间拆分的数据点。 |
| [Auto](./auto/) | 表示应使用此图表类型的默认机制拆分的数据点。 |
