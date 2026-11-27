---
title: "HtmlSaveOptions.ExportPageFooters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions‑egenskap. Anger om sidhuvuden exporteras"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportpagefooters/
---
## HtmlSaveOptions.ExportPageFooters property

Anger om sidhuvuden ska exporteras.

```csharp
public bool ExportPageFooters { get; set; }
```

### Anmärkningar

Fungerar endast när [`SaveAsSingleFile`](../saveassinglefile/) är True.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPageFootersDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Skapa HTML-sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Ställ in ExportPageFooters till true för att inkludera sidfötter i utdata
            saveOptions.ExportPageFooters = true;
            
            // Ställ in andra nödvändiga alternativ
            saveOptions.ExportPageHeaders = true;
            
            // Spara arbetsboken till HTML
            workbook.Save("HtmlWithPageFooters.html", saveOptions);
            
            Console.WriteLine("HTML file with page footers exported successfully.");
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


