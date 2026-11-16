---
title: "ColorScale 类"
linktitle: "ColorScale"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ColorScale 类。封装在 Go 中表示 colorscale 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/colorscale/
---

## ColorScale class

描述 ColorScale 条件格式规则。此条件格式规则在单元格上创建渐变颜色比例。

```go

type ColorScale struct  {
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
| [GetIs3ColorScale](./getis3colorscale/) | 指示条件格式是否为三色刻度。 |
| [SetIs3ColorScale](./setis3colorscale/) | 指示条件格式是否为三色刻度。 |
| [GetMinCfvo](./getmincfvo/) | 获取或设置此 ColorScale 的最小值对象。不能将 null 或类型为 FormatConditionValueType.Max 的 CFValueObject 设置为它。 |
| [GetMidCfvo](./getmidcfvo/) | 获取或设置此 ColorScale 的中间值对象。不能将类型为 FormatConditionValueType.Max 或 FormatConditionValueType.Min 的 CFValueObject 设置为它。 |
| [GetMaxCfvo](./getmaxcfvo/) | 获取或设置此 ColorScale 的最大值对象。不能将 null 或类型为 FormatConditionValueType.Min 的 CFValueObject 设置为它。 |
| [GetMinColor](./getmincolor/) | 获取或设置范围内最小值的渐变颜色。 |
| [SetMinColor](./setmincolor/) | 获取或设置范围内最小值的渐变颜色。 |
| [GetMidColor](./getmidcolor/) | 获取或设置范围内中间值的渐变颜色。 |
| [SetMidColor](./setmidcolor/) | 获取或设置范围内中间值的渐变颜色。 |
| [GetMaxColor](./getmaxcolor/) | 获取或设置范围内最大值的渐变颜色。 |
| [SetMaxColor](./setmaxcolor/) | 获取或设置范围内最大值的渐变颜色。 |
