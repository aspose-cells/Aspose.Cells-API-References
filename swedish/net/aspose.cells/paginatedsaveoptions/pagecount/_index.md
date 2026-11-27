---
title: "PaginatedSaveOptions.PageCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions egenskap. Hämtar eller anger antalet sidor att spara"
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/pagecount/
---
## PaginatedSaveOptions.PageCount property

Hämtar eller anger antalet sidor som ska sparas.

```csharp
public int PageCount { get; set; }
```

### Anmärkningar

Standard är System.Int32.MaxValue vilket betyder att alla sidor kommer att renderas..

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageCountDemo
    {
        public static void Run()
        {
            // Öppna en Excel‑fil
            Workbook wb = new Workbook("Book1.xlsx");
            
            // Initiera PDF-sparalternativ
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Ställ in för att skriva ut endast 2 sidor med start från sida 4 (0-baserat index 3)
            options.PageIndex = 3;
            options.PageCount = 2;
            
            // Spara PDF‑filen
            wb.Save("output.pdf", options);
            
            Console.WriteLine("PDF saved with selected pages.");
        }
    }
}
```

### Se även

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


