---
title: "HtmlSaveOptions.AddTooltipText"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions egenskap. Anger om verktygstippstext ska läggas till när data inte kan visas helt. Standardvärdet är falskt"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/addtooltiptext/
---
## HtmlSaveOptions.AddTooltipText property

Anger om tooltip‑text ska läggas till när data inte kan visas helt. Standardvärdet är false.

```csharp
public bool AddTooltipText { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAddTooltipTextDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange en lång text som kommer att överskrida cellens bredd
            worksheet.Cells["A1"].PutValue("This is a long text that will exceed cell width and need tooltip");
            worksheet.Cells.SetColumnWidth(0, 10); // Set narrow column width
            
            // Konfigurera HTML-sparalternativ med verktygstipp
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.AddTooltipText = true;
            
            // Spara arbetsboken
            string outputPath = "output_with_tooltip.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved with tooltips: " + outputPath);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


