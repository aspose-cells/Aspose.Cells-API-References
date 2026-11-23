---
title: "RenderingWatermark.Rotation"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "RenderingWatermark 属性。获取或设置水印的旋转角度（以度为单位）"
type: docs
url: /zh/net/aspose.cells.rendering/renderingwatermark/rotation/
---
## RenderingWatermark.Rotation property

获取或设置水印的旋转角度（以度为单位）。

```csharp
public float Rotation { get; set; }
```

### 示例

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyRotationDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data for watermark demo");

            // 为水印创建字体
            RenderingFont font = new RenderingFont("Arial", 72);
            font.Color = Color.FromArgb(128, 0, 0, 255);
            font.Bold = true;

            // 创建带旋转的水印
            RenderingWatermark watermark = new RenderingWatermark("ROTATED WATERMARK", font);
            watermark.Rotation = 45; // 45 degree rotation
            watermark.Opacity = 0.5f;
            watermark.IsBackground = true;

            // 设置带水印的 PDF 保存选项
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // 保存时使用水印
            workbook.Save("WatermarkRotationDemo.pdf", options);
        }
    }
}
```

### 另请参见

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


