---
title: "PaginatedSaveOptions.PrintingPageType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions egenskap. Anger vilka sidor som inte kommer att skrivas ut"
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/printingpagetype/
---
## PaginatedSaveOptions.PrintingPageType property

Anger vilka sidor som inte kommer att skrivas ut.

```csharp
public PrintingPageType PrintingPageType { get; set; }
```

### Anmärkningar

Om innehållet i bladet är glest, kommer vissa sidor att vara helt tomma i den genererade pdf-filen. Om du inte vill ha dessa tomma sidor kan du använda det här alternativet för att utelämna dem.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPrintingPageTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Lägg till lite exempeldata
            ws.Cells["A1"].PutValue("Sample Data");
            ws.Cells["A2"].PutValue(123);
            ws.Cells["A3"].PutValue(456);
            
            // Skapa tomt kalkylblad
            Worksheet blankWs = wb.Worksheets.Add("BlankSheet");
            
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Spara utan att ta med tomma sidor
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
            wb.Save("output_ignore_blank_page.pdf", pdfSaveOptions);
            
            // Spara utan att ta med tomma sidor och sidor som bara innehåller format
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;
            wb.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
        }
    }
}
```

### Se även

* enum [PrintingPageType](../../printingpagetype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


