---
title: "LineFormat 类"
linktitle: "LineFormat"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "LineFormat 类。封装在 Go 中表示 lineformat 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/lineformat/
---

## LineFormat class

表示线条的所有设置。

```go

type LineFormat struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewLineFormat](./newlineformat/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetHashCode](./gethashcode/) | 获取哈希码。 |
| [Equals](./equals/) | 确定此实例是否具有与另一个指定的 LineFormat 对象相同的值。 |
| [GetCompoundType](./getcompoundtype/) | 指定线的复合类型。 |
| [SetCompoundType](./setcompoundtype/) | 指定线的复合类型。 |
| [GetDashStyle](./getdashstyle/) | 指定线的虚线类型。 |
| [SetDashStyle](./setdashstyle/) | 指定线的虚线类型。 |
| [GetCapType](./getcaptype/) | 指定结束端帽。 |
| [SetCapType](./setcaptype/) | 指定结束端帽。 |
| [GetJoinType](./getjointype/) | 指定线的连接类型。 |
| [SetJoinType](./setjointype/) | 指定线的连接类型。 |
| [GetBeginArrowheadStyle](./getbeginarrowheadstyle/) | 获取并设置线的起始箭头类型。 |
| [SetBeginArrowheadStyle](./setbeginarrowheadstyle/) | 获取并设置线的起始箭头类型。 |
| [GetBeginArrowheadWidth](./getbeginarrowheadwidth/) | 获取并设置线的起始箭头宽度类型。 |
| [SetBeginArrowheadWidth](./setbeginarrowheadwidth/) | 获取并设置线的起始箭头宽度类型。 |
| [GetBeginArrowheadLength](./getbeginarrowheadlength/) | 获取并设置线的起始箭头长度类型。 |
| [SetBeginArrowheadLength](./setbeginarrowheadlength/) | 获取并设置线的起始箭头长度类型。 |
| [GetEndArrowheadStyle](./getendarrowheadstyle/) | 获取并设置线的结束箭头类型。 |
| [SetEndArrowheadStyle](./setendarrowheadstyle/) | 获取并设置线的结束箭头类型。 |
| [GetEndArrowheadWidth](./getendarrowheadwidth/) | 获取并设置线的结束箭头宽度类型。 |
| [SetEndArrowheadWidth](./setendarrowheadwidth/) | 获取并设置线的结束箭头宽度类型。 |
| [GetEndArrowheadLength](./getendarrowheadlength/) | 获取并设置线的结束箭头长度类型。 |
| [SetEndArrowheadLength](./setendarrowheadlength/) | 获取并设置线的结束箭头长度类型。 |
| [GetWeight](./getweight/) | 获取或设置线条的粗细（单位：点）。 |
| [SetWeight](./setweight/) | 获取或设置线条的粗细（单位：点）。 |
| [GetFillType](./getfilltype/) | 获取并设置填充类型 |
| [SetFillType](./setfilltype/) | 获取并设置填充类型 |
| [GetTransparency](./gettransparency/) | 返回或设置该区域的透明度，取值范围为 0.0（不透明）至 1.0（完全透明）。 |
| [SetTransparency](./settransparency/) | 返回或设置该区域的透明度，取值范围为 0.0（不透明）至 1.0（完全透明）。 |
| [GetGradientFill](./getgradientfill/) | 获取 GradientFill 对象。 |
| [GetTextureFill](./gettexturefill/) | 获取 TextureFill 对象。 |
| [GetSolidFill](./getsolidfill/) | 获取 SolidFill 对象。 |
| [GetPatternFill](./getpatternfill/) | 获取 PatternFill 对象。 |
| [GetGradientColorType](./getgradientcolortype/) | 返回指定填充的渐变颜色类型。 |
| [GetGradientStyle](./getgradientstyle/) | 返回指定填充的渐变样式。 |
| [GetGradientColor1](./getgradientcolor1/) | 返回指定填充的渐变颜色 1。 |
| [GetGradientColor2](./getgradientcolor2/) | 返回指定填充的渐变颜色 2。 |
| [GetGradientDegree](./getgradientdegree/) | 返回指定填充的渐变角度。仅适用于 Excel 2007。 |
| [GetGradientVariant](./getgradientvariant/) | 返回指定填充的渐变变体。仅适用于 Excel 2007。 |
| [GetPresetColor](./getpresetcolor/) | 返回指定填充的渐变预设颜色。 |
| [SetOneColorGradient](./setonecolorgradient/) | 将指定的填充设置为单色渐变。仅适用于 Excel 2007。 |
| [SetTwoColorGradient_Color_Color_GradientStyleType_Int](./settwocolorgradient_color_color_gradientstyletype_int/) | 将指定的填充设置为双色渐变。仅适用于 Excel 2007。 |
| [SetPresetColorGradient](./setpresetcolorgradient/) | 将指定填充设置为预设颜色渐变。仅适用于 Excel 2007。 |
| [GetTexture](./gettexture/) | 表示指定填充的纹理类型。 |
| [SetTexture](./settexture/) | 表示指定填充的纹理类型。 |
| [GetPattern](./getpattern/) | 表示区域的显示模式。 |
| [SetPattern](./setpattern/) | 表示区域的显示模式。 |
| [GetPictureFormatType](./getpictureformattype/) | 获取和设置图片格式类型。 |
| [SetPictureFormatType](./setpictureformattype/) | 获取和设置图片格式类型。 |
| [GetScale](./getscale/) | 获取和设置图片格式比例。 |
| [SetScale](./setscale/) | 获取和设置图片格式比例。 |
| [GetImageData](./getimagedata/) | 获取并设置图片图像数据。 |
| [SetImageData](./setimagedata/) | 获取并设置图片图像数据。 |
