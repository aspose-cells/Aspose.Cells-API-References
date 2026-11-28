---
title: "RenderingFont.Italic"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RenderingFont özelliği. Yazı tipi için italik alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.rendering/renderingfont/italic/
---
## RenderingFont.Italic property

Yazı tipinin italik özelliğini alır veya ayarlar.

```csharp
public bool Italic { get; set; }
```

### Örnekler

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

            // İtalik özelliği ayarlanmış bir RenderingFont oluştur
            RenderingFont renderingFont = new RenderingFont("Arial", 16)
            {
                Italic = true,
                Color = Color.Red
            };

            // Yazı tipini A1 hücresine uygula
            sheet.Cells["A1"].PutValue("Italic Text Example");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";  // Directly use the font name
            style.Font.Size = (int)renderingFont.Size;  // Explicit cast to int
            style.Font.IsItalic = renderingFont.Italic;
            style.Font.Color = renderingFont.Color;
            sheet.Cells["A1"].SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("ItalicFontExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


