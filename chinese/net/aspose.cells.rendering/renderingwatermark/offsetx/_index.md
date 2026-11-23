---
title: "RenderingWatermark.OffsetX"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "RenderingWatermark 属性。获取或设置相对于 HAlignment 的偏移值"
type: docs
url: /zh/net/aspose.cells.rendering/renderingwatermark/offsetx/
---
## RenderingWatermark.OffsetX property

获取或设置相对于 [`HAlignment`](../halignment/) 的偏移值

```csharp
public float OffsetX { get; set; }
```

### 示例

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyOffsetXDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Sample Data");

            RenderingFont font = new RenderingFont("Arial", 24)
            {
                Color = Color.Red,
                Bold = true
            };

            RenderingWatermark watermark = new RenderingWatermark("DEMO WATERMARK", font)
            {
                Rotation = 45,
                Opacity = 0.3f,
                IsBackground = true,
                OffsetX = 100,  // Demonstrating OffsetX property
                OffsetY = 50
            };

            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            workbook.Save("WatermarkWithOffsetX.pdf", options);
        }
    }
}
```

### 另请参见

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


