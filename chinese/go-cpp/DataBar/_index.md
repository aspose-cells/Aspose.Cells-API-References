---
title: "DataBar 类"
linktitle: "DataBar"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "DataBar 类。封装了在 Go 中表示 databar 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/databar/
---

## DataBar class

描述 DataBar 条件格式规则。此条件格式规则在单元格范围内显示渐变数据条。

```go

type DataBar struct  {
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
| [GetAxisColor](./getaxiscolor/) | 获取条件格式为数据条的单元格的轴颜色。 |
| [SetAxisColor](./setaxiscolor/) | 获取条件格式为数据条的单元格的轴颜色。 |
| [GetAxisPosition](./getaxisposition/) | 获取或设置由条件格式规则指定的数据条轴的位置。 |
| [SetAxisPosition](./setaxisposition/) | 获取或设置由条件格式规则指定的数据条轴的位置。 |
| [GetBarFillType](./getbarfilltype/) | 获取或设置数据条的填充颜色方式。 |
| [SetBarFillType](./setbarfilltype/) | 获取或设置数据条的填充颜色方式。 |
| [GetDirection](./getdirection/) | 获取或设置数据条的显示方向。 |
| [SetDirection](./setdirection/) | 获取或设置数据条的显示方向。 |
| [GetBarBorder](./getbarborder/) | 获取指定数据条边框的对象。 |
| [GetNegativeBarFormat](./getnegativebarformat/) | 获取与数据条条件格式规则关联的 NegativeBarFormat 对象。 |
| [GetMinCfvo](./getmincfvo/) | 获取或设置此 DataBar 的最小值对象。不能将 null 或类型为 FormatConditionValueType.Max 的 CFValueObject 设置给它。 |
| [GetMaxCfvo](./getmaxcfvo/) | 获取或设置此 DataBar 的最大值对象。不能将 null 或类型为 FormatConditionValueType.Min 的 CFValueObject 设置给它。 |
| [GetColor](./getcolor/) | 获取或设置此 DataBar 的颜色。 |
| [SetColor](./setcolor/) | 获取或设置此 DataBar 的颜色。 |
| [GetMinLength](./getminlength/) | 表示数据条的最小长度。 |
| [SetMinLength](./setminlength/) | 表示数据条的最小长度。 |
| [GetMaxLength](./getmaxlength/) | 表示数据条的最大长度。 |
| [SetMaxLength](./setmaxlength/) | 表示数据条的最大长度。 |
| [GetShowValue](./getshowvalue/) | 获取或设置指示是否显示此数据条所应用单元格值的标志。默认值为 true。 |
| [SetShowValue](./setshowvalue/) | 获取或设置指示是否显示此数据条所应用单元格值的标志。默认值为 true。 |
| [ToImage](./toimage/) | 将单元格中的数据条渲染为图像字节数组。 |
