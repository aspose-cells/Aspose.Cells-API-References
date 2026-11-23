---
title: "RenderingFont.Italic"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "RenderingFont 属性。获取或设置字体的斜体"
type: docs
url: /zh/net/aspose.cells.rendering/renderingfont/italic/
---
## RenderingFont.Italic property

获取或设置字体的斜体。

```csharp
public bool Italic { get; set; }
```

### 示例

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingFontPropertyItalicDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // 创建一个已设置 Italic 属性的 RenderingFont
            RenderingFont renderingFont = new RenderingFont("Arial", 16)
            {
                Italic = true,
                Color = Color.Red
            };

            // 将字体应用于单元格 A1
            sheet.Cells["A1"].PutValue("Italic Text Example");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";  // Directly use the font name
            style.Font.Size = (int)renderingFont.Size;  // Explicit cast to int
            style.Font.IsItalic = renderingFont.Italic;
            style.Font.Color = renderingFont.Color;
            sheet.Cells["A1"].SetStyle(style);

            // 保存工作簿
            workbook.Save("ItalicFontExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### 另请参见

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


