---
title: "RenderingWatermark Class"
linktitle: "RenderingWatermark"
articleTitle: "RenderingWatermark"
second_title: "Aspose.Cells for PHP via Java"
description: "Watermark for rendering."
type: docs
weight: 5380
url: /php/aspose.cells/renderingwatermark/
---

## RenderingWatermark class

Watermark for rendering.

## Constructors

| Name | Description |
| --- | --- |
| [RenderingWatermark](#constructor) | Creates instance of text watermark. |
| [RenderingWatermark](#constructor) | Creates instance of image watermark. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Rotation](#rotation) | Number | Gets or sets roation of the watermark in degrees. |
| [ScaleToPagePercent](#scaletopagepercent) | Number | Gets or sets scale relative to target page in percent. |
| [Opacity](#opacity) | Number | Gets or sets opacity of the watermark in range [0, 1]. |
| [IsBackground](#isbackground) | boolean | Indicates whether the watermark is placed behind page contents. |
| [Text](#text) | String | Gets text of the watermark. |
| [Font](#font) | RenderingFont | Gets font of the watermark. |
| [Image](#image) | byte[] | Gets image of the watermark. |
| [HAlignment](#halignment) | Number | Gets or sets horizontal alignment of the watermark to the page. The value of the property is TextAlignmentType integer c |
| [VAlignment](#valignment) | Number | Gets or sets vertical alignment of the watermark to the page. The value of the property is TextAlignmentType integer con |
| [OffsetX](#offsetx) | Number | Gets or sets offset value to HAlignment |
| [OffsetY](#offsety) | Number | Gets or sets offset value to VAlignment |

### RenderingWatermark(text, renderingFont) (1 of 2) {#constructor}

Creates instance of text watermark.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | watermark text |
| renderingFont | RenderingFont | watermark font |

---

### RenderingWatermark(imageData) (2 of 2) {#constructor-1}

Creates instance of image watermark.

| Parameter | Type | Description |
| --- | --- | --- |
| imageData | byte[] |  |

### RenderingWatermark.Rotation property {#rotation}

Gets or sets roation of the watermark in degrees.

**Type:** Number

### RenderingWatermark.ScaleToPagePercent property {#scaletopagepercent}

Gets or sets scale relative to target page in percent.

**Type:** Number

### RenderingWatermark.Opacity property {#opacity}

Gets or sets opacity of the watermark in range [0, 1].

**Type:** Number

### RenderingWatermark.IsBackground property {#isbackground}

Indicates whether the watermark is placed behind page contents.

**Type:** boolean

### RenderingWatermark.Text property {#text}

Gets text of the watermark.

**Type:** String

### RenderingWatermark.Font property {#font}

Gets font of the watermark.

**Type:** RenderingFont

### RenderingWatermark.Image property {#image}

Gets image of the watermark.

**Type:** byte[]

### RenderingWatermark.HAlignment property {#halignment}

Gets or sets horizontal alignment of the watermark to the page. The value of the property is TextAlignmentType integer constant. Only Left, Center, Right is valid. Default is Left.

**Type:** Number

### RenderingWatermark.VAlignment property {#valignment}

Gets or sets vertical alignment of the watermark to the page. The value of the property is TextAlignmentType integer constant. Only Top, Center, Bottom is valid. Default is Top.

**Type:** Number

### RenderingWatermark.OffsetX property {#offsetx}

Gets or sets offset value to HAlignment

**Type:** Number

### RenderingWatermark.OffsetY property {#offsety}

Gets or sets offset value to VAlignment

**Type:** Number
