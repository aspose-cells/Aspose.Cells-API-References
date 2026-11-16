---
title: "ErrorBar 类"
linktitle: "ErrorBar"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ErrorBar 类。封装在 Go 中表示 errorbar 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/errorbar/
---

## ErrorBar class

表示数据系列的误差线。

```go

type ErrorBar struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewErrorBar](./newerrorbar/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetType](./gettype/) | 表示误差线的数值类型。 |
| [SetType](./settype/) | 表示误差线的数值类型。 |
| [GetDisplayType](./getdisplaytype/) | 表示误差线的显示类型。 |
| [SetDisplayType](./setdisplaytype/) | 表示误差线的显示类型。 |
| [GetAmount](./getamount/) | 表示误差线的量值。 |
| [SetAmount](./setamount/) | 表示误差线的量值。 |
| [GetShowMarkerTTop](./getshowmarkerttop/) | 指示误差线是否使用 T 顶格式。 |
| [SetShowMarkerTTop](./setshowmarkerttop/) | 指示误差线是否使用 T 顶格式。 |
| [GetPlusValue](./getplusvalue/) | 当误差线类型为自定义时，表示正误差量。 |
| [SetPlusValue](./setplusvalue/) | 当误差线类型为自定义时，表示正误差量。 |
| [GetMinusValue](./getminusvalue/) | 当误差线类型为自定义时，表示负误差量。 |
| [SetMinusValue](./setminusvalue/) | 当误差线类型为自定义时，表示负误差量。 |
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
