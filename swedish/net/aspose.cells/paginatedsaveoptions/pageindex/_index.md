---
title: "PaginatedSaveOptions.PageIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions-egenskap. Hämtar eller anger det 0-baserade indexet för den första sidan som ska sparas"
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/pageindex/
---
## PaginatedSaveOptions.PageIndex property

Hämtar eller anger det 0‑baserade indexet för den första sidan som ska sparas.

```csharp
public int PageIndex { get; set; }
```

### Anmärkningar

Standard är 0.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Lägg till exempeldata över flera sidor
            for (int i = 0; i < 100; i++)
            {
                sheet.Cells[i, 0].Value = "Data " + (i + 1);
            }

            // Ställ in PDF-sparalternativ
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Ställ in för att skriva ut sidor 3-4 (0-baserat index)
            options.PageIndex = 2;  // Third page (index 2)
            options.PageCount = 2; // Print 2 pages
            
            // Spara PDF-filen med valda sidor
            wb.Save("SelectedPages.pdf", options);
            
            Console.WriteLine("PDF with pages 3-4 created successfully.");
        }
    }
}
```

### Se även

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


