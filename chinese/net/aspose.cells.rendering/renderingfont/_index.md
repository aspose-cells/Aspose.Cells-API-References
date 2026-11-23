---
title: "类 RenderingFont"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Rendering.RenderingFont 类。用于渲染的字体"
type: docs
url: /zh/net/aspose.cells.rendering/renderingfont/
---
## RenderingFont class

用于渲染的字体。

```csharp
public class RenderingFont
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [RenderingFont](renderingfont/)(string, float) | 初始化 `RenderingFont` 的新实例 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Bold](../../aspose.cells.rendering/renderingfont/bold/) { get; set; } | 获取或设置字体的粗体。 |
| [Color](../../aspose.cells.rendering/renderingfont/color/) { get; set; } | 获取或设置字体的颜色。 |
| [Italic](../../aspose.cells.rendering/renderingfont/italic/) { get; set; } | 获取或设置字体的斜体。 |
| [Name](../../aspose.cells.rendering/renderingfont/name/) { get; } | 获取字体名称。 |
| [Size](../../aspose.cells.rendering/renderingfont/size/) { get; } | 获取字体的点大小。 |

### 示例

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontDemo
    {
        public static void RenderingFontExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // 添加一些示例数据
            sheet.Cells["A1"].PutValue("Hello World!");

            // 创建 RenderingFont 对象
            RenderingFont renderingFont = new RenderingFont("Arial", 12)
            {
                Bold = true,
                Italic = true,
                Color = Color.Blue
            };

            // 使用 RenderingFont 创建 RenderingWatermark 对象
            RenderingWatermark watermark = new RenderingWatermark("Sample Watermark", renderingFont)
            {
                Rotation = 45,
                ScaleToPagePercent = 100,
                Opacity = 0.5f,
                IsBackground = true,
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                OffsetX = 0,
                OffsetY = 0
            };

            // 创建 PdfSaveOptions 并设置水印
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions
            {
                Watermark = watermark,
                EmbedStandardWindowsFonts = true,
                CalculateFormula = true,
                ExportDocumentStructure = true,
                DisplayDocTitle = true
            };

            // 将工作簿保存为带水印的 PDF
            workbook.Save("RenderingFontExample.pdf", pdfSaveOptions);
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


