---
title: "PaginatedSaveOptions.IgnoreError"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions‑egenskap. Anger om du behöver dölja felet vid rendering. Felet kan vara ett fel i form, bild, diagramrendering osv."
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/ignoreerror/
---
## PaginatedSaveOptions.IgnoreError property

Anger om du behöver dölja felet vid rendering. Felet kan vara ett fel i form, bild, diagramrendering osv.

```csharp
public bool IgnoreError { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyIgnoreErrorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite exempeldata med potentiella formateringsfel
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);
            
            // Skapa PDF-sparalternativ
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Ange IgnoreError till true för att hoppa över eventuella konverteringsfel
            options.IgnoreError = true;
            
            // Spara arbetsboken som PDF
            workbook.Save("PaginatedSaveWithIgnoreError.pdf", options);
            
            Console.WriteLine("PDF saved with IgnoreError enabled.");
        }
    }
}
```

### Se även

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


