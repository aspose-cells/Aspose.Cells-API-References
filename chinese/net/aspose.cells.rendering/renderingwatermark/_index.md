---
title: "类 RenderingWatermark"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Rendering.RenderingWatermark 类。用于渲染的水印"
type: docs
url: /zh/net/aspose.cells.rendering/renderingwatermark/
---
## RenderingWatermark class

用于渲染的水印。

```csharp
public class RenderingWatermark
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [RenderingWatermark](renderingwatermark/#constructor)(byte[]) | 创建图像水印的实例。 |
| [RenderingWatermark](renderingwatermark/#constructor_1)(string, RenderingFont) | 创建文本水印的实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Font](../../aspose.cells.rendering/renderingwatermark/font/) { get; } | 获取水印的字体。 |
| [HAlignment](../../aspose.cells.rendering/renderingwatermark/halignment/) { get; set; } | 获取或设置水印相对于页面的水平对齐方式。 |
| [Image](../../aspose.cells.rendering/renderingwatermark/image/) { get; } | 获取水印的图像。 |
| [IsBackground](../../aspose.cells.rendering/renderingwatermark/isbackground/) { get; set; } | 指示水印是否放置在页面内容后面。 |
| [OffsetX](../../aspose.cells.rendering/renderingwatermark/offsetx/) { get; set; } | 获取或设置相对于[`HAlignment`](./halignment/)的偏移值。 |
| [OffsetY](../../aspose.cells.rendering/renderingwatermark/offsety/) { get; set; } | 获取或设置相对于[`VAlignment`](./valignment/)的偏移值。 |
| [Opacity](../../aspose.cells.rendering/renderingwatermark/opacity/) { get; set; } | 获取或设置水印的不透明度，范围为[0, 1]。 |
| [Rotation](../../aspose.cells.rendering/renderingwatermark/rotation/) { get; set; } | 获取或设置水印的旋转角度（以度为单位）。 |
| [ScaleToPagePercent](../../aspose.cells.rendering/renderingwatermark/scaletopagepercent/) { get; set; } | 获取或设置相对于目标页面的缩放比例（百分比）。 |
| [Text](../../aspose.cells.rendering/renderingwatermark/text/) { get; } | 获取水印的文本。 |
| [VAlignment](../../aspose.cells.rendering/renderingwatermark/valignment/) { get; set; } | 获取或设置水印相对于页面的垂直对齐方式。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class RenderingWatermarkDemo
    {
        public static void RenderingWatermarkExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample worksheet.");

            // 为水印创建字体
            RenderingFont font = new RenderingFont("Calibri", 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // 使用文本和指定的字体创建水印
            RenderingWatermark watermark = new RenderingWatermark("Watermark", font);

            // 设置水印的属性
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.Rotation = 30;
            watermark.Opacity = 0.6f;
            watermark.ScaleToPagePercent = 50;
            watermark.IsBackground = true;

            // 指定用于渲染为 PDF 的水印
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // 将工作簿保存为带有水印的 PDF
            workbook.Save("output_watermark.pdf", options);
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


