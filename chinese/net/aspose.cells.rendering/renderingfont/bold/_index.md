---
title: "RenderingFont.Bold"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "RenderingFont 属性。获取或设置字体的粗体"
type: docs
url: /zh/net/aspose.cells.rendering/renderingfont/bold/
---
## RenderingFont.Bold property

获取或设置字体的粗体。

```csharp
public bool Bold { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontPropertyBoldDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Bold Font Example");

            // 为单元格创建样式
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            worksheet.Cells["A1"].SetStyle(style);

            // 创建带有演示粗体字体的水印的 PDF 保存选项
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // 创建带有粗体属性的渲染字体
            RenderingFont font = new RenderingFont("Arial", 36)
            {
                Bold = true,
                Color = System.Drawing.Color.Red
            };
            
            // 使用粗体字体创建水印
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Opacity = 0.3f
            };
            pdfSaveOptions.Watermark = watermark;

            // 保存工作簿
            workbook.Save("BoldFontExample.pdf", pdfSaveOptions);
        }
    }
}
```

### 另请参见

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


