---
title: "Trendline 类"
linktitle: "Trendline"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Trendline 类。封装在 Go 中表示 trendline 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/trendline/
---

## Trendline class

表示图表中的趋势线。

```go

type Trendline struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewTrendline](./newtrendline/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [IsNameAuto](./isnameauto/) | 返回 Microsoft Excel 是否自动确定趋势线的名称。 |
| [SetIsNameAuto](./setisnameauto/) | 返回 Microsoft Excel 是否自动确定趋势线的名称。 |
| [GetType](./gettype/) | 返回趋势线类型。 |
| [GetName](./getname/) | 返回趋势线的名称。 |
| [SetName](./setname/) | 返回趋势线的名称。 |
| [GetOrder](./getorder/) | 获取或设置趋势线的阶数（大于 1 的整数），当趋势线类型为 Polynomial 时。阶数必须在 2 到 6 之间。 |
| [SetOrder](./setorder/) | 获取或设置趋势线的阶数（大于 1 的整数），当趋势线类型为 Polynomial 时。阶数必须在 2 到 6 之间。 |
| [GetPeriod](./getperiod/) | 获取或设置移动平均趋势线的周期。 |
| [SetPeriod](./setperiod/) | 获取或设置移动平均趋势线的周期。 |
| [GetForward](./getforward/) | 获取或设置趋势线向前延伸的周期数（或散点图上的单位）。周期数必须大于或等于零。 |
| [SetForward](./setforward/) | 获取或设置趋势线向前延伸的周期数（或散点图上的单位）。周期数必须大于或等于零。 |
| [GetBackward](./getbackward/) | 获取或设置趋势线向后延伸的周期数（或散点图上的单位）。周期数必须大于或等于零。如果图表类型为 column，周期数必须在 0 到 0.5 之间。 |
| [SetBackward](./setbackward/) | 获取或设置趋势线向后延伸的周期数（或散点图上的单位）。周期数必须大于或等于零。如果图表类型为 column，周期数必须在 0 到 0.5 之间。 |
| [GetDisplayEquation](./getdisplayequation/) | 表示是否在图表上显示趋势线方程（与 R-squared 值在同一数据标签中）。将此属性设置为 True 会自动打开数据标签。 |
| [SetDisplayEquation](./setdisplayequation/) | 表示是否在图表上显示趋势线方程（与 R-squared 值在同一数据标签中）。将此属性设置为 True 会自动打开数据标签。 |
| [GetDisplayRSquared](./getdisplayrsquared/) | 表示是否在图表上显示趋势线的 R-squared 值（与方程在同一数据标签中）。将此属性设置为 True 会自动打开数据标签。 |
| [SetDisplayRSquared](./setdisplayrsquared/) | 表示是否在图表上显示趋势线的 R-squared 值（与方程在同一数据标签中）。将此属性设置为 True 会自动打开数据标签。 |
| [GetIntercept](./getintercept/) | 获取或设置趋势线与数值轴相交的点。 |
| [SetIntercept](./setintercept/) | 获取或设置趋势线与数值轴相交的点。 |
| [GetDataLabels](./getdatalabels/) | 表示指定系列的 DataLabels 对象。 |
| [GetLegendEntry](./getlegendentry/) | 获取此趋势线对应的图例项。 |
| [GetCompoundType](./getcompoundtype/) | 指定复合线类型 |
| [SetCompoundType](./setcompoundtype/) | 指定复合线类型 |
| [GetDashType](./getdashtype/) | 指定虚线类型 |
| [SetDashType](./setdashtype/) | 指定虚线类型 |
| [GetCapType](./getcaptype/) | 指定结束端帽。 |
| [SetCapType](./setcaptype/) | 指定结束端帽。 |
| [GetJoinType](./getjointype/) | 指定连接端帽。 |
| [SetJoinType](./setjointype/) | 指定连接端帽。 |
| [GetBeginType](./getbegintype/) | 指定线段起点的箭头。 |
| [SetBeginType](./setbegintype/) | 指定线段起点的箭头。 |
| [GetEndType](./getendtype/) | 指定线段终点的箭头。 |
| [SetEndType](./setendtype/) | 指定线段终点的箭头。 |
| [GetBeginArrowLength](./getbeginarrowlength/) | 指定线段起点箭头的长度。 |
| [SetBeginArrowLength](./setbeginarrowlength/) | 指定线段起点箭头的长度。 |
| [GetEndArrowLength](./getendarrowlength/) | 指定线段终点箭头的长度。 |
| [SetEndArrowLength](./setendarrowlength/) | 指定线段终点箭头的长度。 |
| [GetBeginArrowWidth](./getbeginarrowwidth/) | 指定线段起点箭头的宽度。 |
| [SetBeginArrowWidth](./setbeginarrowwidth/) | 指定线段起点箭头的宽度。 |
| [GetEndArrowWidth](./getendarrowwidth/) | 指定线段终点箭头的宽度。 |
| [SetEndArrowWidth](./setendarrowwidth/) | 指定线段终点箭头的宽度。 |
| [GetThemeColor](./getthemecolor/) | 获取和设置主题颜色。 |
| [SetThemeColor](./setthemecolor/) | 获取和设置主题颜色。 |
| [GetColor](./getcolor/) | 表示线条的颜色。 |
| [SetColor](./setcolor/) | 表示线条的颜色。 |
| [GetTransparency](./gettransparency/) | 返回或设置线条的透明度，取值范围从 0.0（不透明）到 1.0（完全透明）。 |
| [SetTransparency](./settransparency/) | 返回或设置线条的透明度，取值范围从 0.0（不透明）到 1.0（完全透明）。 |
| [GetStyle](./getstyle/) | 表示线条的样式。 |
| [SetStyle](./setstyle/) | 表示线条的样式。 |
| [GetWeight](./getweight/) | 获取或设置线条的 WeightType。 |
| [SetWeight](./setweight/) | 获取或设置线条的 WeightType。 |
| [GetWeightPt](./getweightpt/) | 获取或设置线条的粗细（单位：点）。 |
| [SetWeightPt](./setweightpt/) | 获取或设置线条的粗细（单位：点）。 |
| [GetWeightPx](./getweightpx/) | 获取或设置线条的粗细（单位：像素）。 |
| [SetWeightPx](./setweightpx/) | 获取或设置线条的粗细（单位：像素）。 |
| [GetFormattingType](./getformattingtype/) | 获取或设置格式类型。 |
| [SetFormattingType](./setformattingtype/) | 获取或设置格式类型。 |
| [IsAutomaticColor](./isautomaticcolor/) | 指示线条颜色是否自动分配。 |
| [IsVisible](./isvisible/) | 表示线条是否可见。 |
| [SetIsVisible](./setisvisible/) | 表示线条是否可见。 |
| [IsAuto](./isauto/) | 指示此线条样式是否自动分配。 |
| [SetIsAuto](./setisauto/) | 指示此线条样式是否自动分配。 |
| [GetGradientFill](./getgradientfill/) | 表示渐变填充。 |
