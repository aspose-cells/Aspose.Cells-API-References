---
title: "PdfSaveOptions.Watermark"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PdfSaveOptions 属性。获取或设置要输出的水印"
type: docs
url: /zh/net/aspose.cells/pdfsaveoptions/watermark/
---
## PdfSaveOptions.Watermark property

获取或设置要输出的水印。

```csharp
public RenderingWatermark Watermark { get; set; }
```

### 示例

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyWatermarkDemo
    {
        public static void Run()
        {
            // 创建一个包含 3 个工作表的工作簿
            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells["A1"].PutValue("Page1");
            int index = wb.Worksheets.Add();
            wb.Worksheets[index].Cells["A1"].PutValue("Page2");
            index = wb.Worksheets.Add();
            wb.Worksheets[index].Cells["A1"].PutValue("Page3");

            // 创建水印字体
            RenderingFont font = new RenderingFont("Calibri", 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // 使用文本和字体创建水印
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.Rotation = 45;
            watermark.Opacity = 0.3f;
            watermark.ScaleToPagePercent = 75;

            // 在 PDF 保存选项中设置水印
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // 保存带有水印的工作簿
            wb.Save("output_watermark.pdf", options);
        }
    }
}
```

### 另请参见

* class [RenderingWatermark](../../../aspose.cells.rendering/renderingwatermark/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


