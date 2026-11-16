---
title: "ChartCalculateOptions 类"
linktitle: "ChartCalculateOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ChartCalculateOptions 类。封装在 Go 中表示 chartcalculateoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/chartcalculateoptions/
---

## ChartCalculateOptions class

表示图表计算的选项。

```go

type ChartCalculateOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewChartCalculateOptions](./newchartcalculateoptions/) | 创建用于计算图表的选项。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetUpdateAllPoints](./getupdateallpoints/) | 在执行图表计算时是否更新所有数据点。默认：False。当您想要专门获取图表中每个数据点的值时，请将其设为 true。如果此参数设为 True，计算图表时可能会生成新的数据点。这可能会使 Excel 文件变大。 |
| [SetUpdateAllPoints](./setupdateallpoints/) | 在执行图表计算时是否更新所有数据点。默认：False。当您想要专门获取图表中每个数据点的值时，请将其设为 true。如果此参数设为 True，计算图表时可能会生成新的数据点。这可能会使 Excel 文件变大。 |
