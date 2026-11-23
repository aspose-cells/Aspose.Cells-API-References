---
title: "RenderingWatermark.OffsetY"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "RenderingWatermark 属性。获取或设置相对于 VAlignment 的偏移值"
type: docs
url: /zh/net/aspose.cells.rendering/renderingwatermark/offsety/
---
## RenderingWatermark.OffsetY property

获取或设置偏移值到 [`VAlignment`](../valignment/)

```csharp
public float OffsetY { get; set; }
```

### 示例

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyOffsetYDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // 添加示例数据
            sheet.Cells["A1"].PutValue("OffsetY Demo");

            // 创建水印字体
            RenderingFont font = new RenderingFont("Arial", 24)
            {
                Color = Color.Red,
                Bold = true
            };

            // 使用不同的 OffsetY 值创建水印
            RenderingWatermark watermark = new RenderingWatermark("VERTICAL OFFSET", font)
            {
                Rotation = 0,
                Opacity = 0.3f,
                IsBackground = true,
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                OffsetX = 0,
                OffsetY = 100 // Demonstrating OffsetY property
            };

            // 设置带有水印的保存选项
            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // 使用水印偏移保存
            workbook.Save("WatermarkOffsetYDemo.pdf", options);
        }
    }
}
```

### 另请参见

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


