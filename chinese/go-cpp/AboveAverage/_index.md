---
title: "AboveAverage 类"
linktitle: "AboveAverage"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "AboveAverage 类。封装在 Go 中表示 aboveaverage 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/aboveaverage/
---

## AboveAverage class

描述 AboveAverage 条件格式规则。此条件格式规则突出显示范围内所有值的高于或低于平均值的单元格。

```go

type AboveAverage struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewAboveAverage](./newaboveaverage/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [IsAboveAverage](./isaboveaverage/) | 获取或设置指示规则是否为\"above average\"规则的标志。'true' 表示 \"above average\"。默认值为 true。 |
| [SetIsAboveAverage](./setisaboveaverage/) | 获取或设置指示规则是否为\"above average\"规则的标志。'true' 表示 \"above average\"。默认值为 true。 |
| [IsEqualAverage](./isequalaverage/) | 获取或设置指示 'aboveAverage' 和 'belowAverage' 条件是包含平均值本身还是排除该值的标志。'true' 表示在条件中包含平均值。默认值为 false。 |
| [SetIsEqualAverage](./setisequalaverage/) | 获取或设置指示 'aboveAverage' 和 'belowAverage' 条件是包含平均值本身还是排除该值的标志。'true' 表示在条件中包含平均值。默认值为 false。 |
| [GetStdDev](./getstddev/) | 获取或设置在条件格式规则中包含在平均值上方或下方的标准差数量。输入值必须在 0 到 3 之间（包括 0 和 3）。将此值设为 0 表示未设置 stdDev。默认值为 0。 |
| [SetStdDev](./setstddev/) | 获取或设置在条件格式规则中包含在平均值上方或下方的标准差数量。输入值必须在 0 到 3 之间（包括 0 和 3）。将此值设为 0 表示未设置 stdDev。默认值为 0。 |
