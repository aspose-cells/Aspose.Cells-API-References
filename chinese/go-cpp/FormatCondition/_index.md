---
title: "FormatCondition 类"
linktitle: "FormatCondition"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "FormatCondition 类。封装在 Go 中表示 formatcondition 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/formatcondition/
---

## FormatCondition class

表示条件格式化条件。

```go

type FormatCondition struct  {
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
| [GetFormula1_Bool_Bool](./getformula1_bool_bool/) | 获取与此格式条件关联的值或表达式。 |
| [GetFormula2_Bool_Bool](./getformula2_bool_bool/) | 获取与此格式条件关联的值或表达式。 |
| [GetFormula1_Bool_Bool_Int_Int](./getformula1_bool_bool_int_int/) | 获取单元格条件格式的值或表达式。 |
| [GetFormula2_Bool_Bool_Int_Int](./getformula2_bool_bool_int_int/) | 获取单元格条件格式的值或表达式。 |
| [SetFormulas](./setformulas/) | 设置与此格式条件关联的值或表达式。 |
| [SetFormula1_String_Bool_Bool](./setformula1_string_bool_bool/) | 设置与此格式条件关联的值或表达式。 |
| [SetFormula2_String_Bool_Bool](./setformula2_string_bool_bool/) | 设置与此格式条件关联的值或表达式。 |
| [GetFormula1](./getformula1/) | 获取并设置条件格式关联的值或表达式。 |
| [SetFormula1_String](./setformula1_string/) | 获取并设置条件格式关联的值或表达式。 |
| [GetFormula1_Int_Int](./getformula1_int_int/) | 获取单元格条件格式的公式。 |
| [GetFormula2](./getformula2/) | 获取并设置条件格式关联的值或表达式。 |
| [SetFormula2_String](./setformula2_string/) | 获取并设置条件格式关联的值或表达式。 |
| [GetFormula2_Int_Int](./getformula2_int_int/) | 获取单元格条件格式的公式。 |
| [GetOperator](./getoperator/) | 获取并设置条件格式运算符类型。 |
| [SetOperator](./setoperator/) | 获取并设置条件格式运算符类型。 |
| [GetStopIfTrue](./getstopiftrue/) | 为真时，优先级更低的规则不能覆盖此规则，仅在 Excel 2007 中适用； |
| [SetStopIfTrue](./setstopiftrue/) | 为真时，优先级更低的规则不能覆盖此规则，仅在 Excel 2007 中适用； |
| [GetPriority](./getpriority/) | 此条件格式规则的优先级。该值用于确定应评估和呈现的格式。数值越低优先级越高，而数值越高优先级越低，其中 '1' 为最高优先级。 |
| [SetPriority](./setpriority/) | 此条件格式规则的优先级。该值用于确定应评估和呈现的格式。数值越低优先级越高，而数值越高优先级越低，其中 '1' 为最高优先级。 |
| [GetStyle](./getstyle/) | 获取或设置条件格式化单元格范围的样式。 |
| [SetStyle](./setstyle/) | 获取或设置条件格式化单元格范围的样式。 |
| [GetType](./gettype/) | 获取并设置条件格式类型。 |
| [SetType](./settype/) | 获取并设置条件格式类型。 |
| [GetIconSet](./geticonset/) | 获取条件格式的 "IconSet" 实例。默认实例的 IconSetType 为 TrafficLights31。仅在 type = IconSet 时有效。 |
| [GetDataBar](./getdatabar/) | 获取条件格式的 "DataBar" 实例。默认实例的颜色为蓝色。仅在 type 为 DataBar 时有效。 |
| [GetColorScale](./getcolorscale/) | 获取条件格式的 "ColorScale" 实例。默认实例是一个 "green-yellow-red" 3ColorScale。仅在 type = ColorScale 时有效。 |
| [GetTop10](./gettop10/) | 获取条件格式的 "Top10" 实例。默认实例的规则突出显示值位于前 10% 区间的单元格。仅在 type 为 Top10 时有效。 |
| [GetAboveAverage](./getaboveaverage/) | 获取条件格式的 "AboveAverage" 实例。默认实例的规则突出显示范围内所有值高于平均值的单元格。仅在 type = AboveAverage 时有效。 |
| [GetText](./gettext/) | 在 "text contains" 条件格式规则中的文本值。仅在 type = containsText、notContainsText、beginsWith 和 endsWith 时有效。默认值为 null。 |
| [SetText](./settext/) | 在 "text contains" 条件格式规则中的文本值。仅在 type = containsText、notContainsText、beginsWith 和 endsWith 时有效。默认值为 null。 |
| [GetTimePeriod](./gettimeperiod/) | 在 "date occurrin" 条件格式规则中的适用时间段。仅在 type 为 timePeriod 时有效。默认值为 TimePeriodType.Today。 |
| [SetTimePeriod](./settimeperiod/) | 在 "date occurrin" 条件格式规则中的适用时间段。仅在 type 为 timePeriod 时有效。默认值为 TimePeriodType.Today。 |
