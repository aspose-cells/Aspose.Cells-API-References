---
title: "RenderingWatermark 类"
linktitle: "RenderingWatermark"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "RenderingWatermark 类。封装在 Go 中表示 renderingwatermark 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/renderingwatermark/
---

## RenderingWatermark class

渲染使用的水印。

```go

type RenderingWatermark struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewRenderingWatermark_String_RenderingFont](./newrenderingwatermark_string_renderingfont/) | 创建文本水印的实例。 |
| [NewRenderingWatermark_Stream](./newrenderingwatermark_stream/) | 创建图像水印的实例。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetRotation](./getrotation/) | 获取或设置水印的 roation（以度为单位）。 |
| [SetRotation](./setrotation/) | 获取或设置水印的 roation（以度为单位）。 |
| [GetScaleToPagePercent](./getscaletopagepercent/) | 获取或设置相对于目标页面的缩放比例（百分比）。 |
| [SetScaleToPagePercent](./setscaletopagepercent/) | 获取或设置相对于目标页面的缩放比例（百分比）。 |
| [GetOpacity](./getopacity/) | 获取或设置水印的不透明度，范围为 [0, 1]。 |
| [SetOpacity](./setopacity/) | 获取或设置水印的不透明度，范围为 [0, 1]。 |
| [IsBackground](./isbackground/) | 指示水印是否放置在页面内容后面。 |
| [SetIsBackground](./setisbackground/) | 指示水印是否放置在页面内容后面。 |
| [GetText](./gettext/) | 获取水印的文本。 |
| [GetFont](./getfont/) | 获取水印的字体。 |
| [GetImage](./getimage/) | 获取水印的图像。 |
| [GetHAlignment](./gethalignment/) | 获取或设置水印相对于页面的水平对齐方式。 |
| [SetHAlignment](./sethalignment/) | 获取或设置水印相对于页面的水平对齐方式。 |
| [GetVAlignment](./getvalignment/) | 获取或设置水印相对于页面的垂直对齐方式。 |
| [SetVAlignment](./setvalignment/) | 获取或设置水印相对于页面的垂直对齐方式。 |
| [GetOffsetX](./getoffsetx/) | 获取或设置 HAlignment 的偏移值。 |
| [SetOffsetX](./setoffsetx/) | 获取或设置 HAlignment 的偏移值。 |
| [GetOffsetY](./getoffsety/) | 获取或设置 VAlignment 的偏移值。 |
| [SetOffsetY](./setoffsety/) | 获取或设置 VAlignment 的偏移值。 |
