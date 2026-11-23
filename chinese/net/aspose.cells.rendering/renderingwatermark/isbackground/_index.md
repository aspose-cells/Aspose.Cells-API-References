---
title: "RenderingWatermark.IsBackground"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "RenderingWatermark 属性。指示水印是否放置在页面内容后面"
type: docs
url: /zh/net/aspose.cells.rendering/renderingwatermark/isbackground/
---
## RenderingWatermark.IsBackground property

指示水印是否放置在页面内容后面。

```csharp
public bool IsBackground { get; set; }
```

### 示例

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyIsBackgroundDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // 添加示例数据
            sheet.Cells["A1"].PutValue("Sample Content");

            // 创建水印并将 IsBackground 设置为 true
            RenderingFont font = new RenderingFont("Arial", 36)
            {
                Color = Color.LightGray
            };
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font)
            {
                IsBackground = true,
                Rotation = 45,
                Opacity = 0.2f
            };

            // 配置带水印的保存选项
            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // 保存带背景水印
            workbook.Save("WatermarkIsBackgroundDemo.pdf", options);
        }
    }
}
```

### 另请参见

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


