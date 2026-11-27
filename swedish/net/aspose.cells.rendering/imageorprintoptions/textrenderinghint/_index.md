---
title: "ImageOrPrintOptions.TextRenderingHint"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Anger kvaliteten på textrendering. Standardvärdet är TextRenderingHint.SystemDefault"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/textrenderinghint/
---
## ImageOrPrintOptions.TextRenderingHint property

Anger kvaliteten på textåtergivning. Standardvärdet är TextRenderingHint.SystemDefault

```csharp
public TextRenderingHint TextRenderingHint { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyTextRenderingHintDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeltext för att demonstrera textrendering
            worksheet.Cells["A1"].PutValue("Text Rendering Hint Demo");
            
            HtmlSaveOptions options = new HtmlSaveOptions();
#if !NETCOREAPP3_1_OR_GREATER
            options.ImageOptions.TextRenderingHint = TextRenderingHint.AntiAlias;
#endif
            workbook.Save("output.html", options);
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


