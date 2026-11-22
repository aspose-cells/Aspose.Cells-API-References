---
title: "RenderingFont.Color"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RenderingFont. يحصل أو يعيّن اللون للخط"
type: docs
url: /ar/net/aspose.cells.rendering/renderingfont/color/
---
## RenderingFont.Color property

يحصل أو يعيّن اللون للخط.

```csharp
public Color Color { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Testing font color property");

            RenderingFont font = new RenderingFont("Arial", 16);
            font.Color = System.Drawing.Color.Red;
            font.Bold = true;

            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = new RenderingWatermark("COLOR DEMO", font)
            {
                Opacity = 0.5f,
                IsBackground = true
            };

            workbook.Save("FontColorDemo.pdf", options);
        }
    }
}
```

### انظر أيضًا

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


