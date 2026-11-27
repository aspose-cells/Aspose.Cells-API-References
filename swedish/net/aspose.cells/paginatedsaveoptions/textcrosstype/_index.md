---
title: "PaginatedSaveOptions.TextCrossType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions egenskap. Hämtar eller anger visningstyp för text när textbredden är större än cellbredden"
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/textcrosstype/
---
## PaginatedSaveOptions.TextCrossType property

Hämtar eller anger visningstyp för text när textbredden är större än cellbredden.

```csharp
public TextCrossType TextCrossType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyTextCrossTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange lång text som kommer att gå över cellgränser
            worksheet.Cells["A1"].PutValue("This is a long text that will cross cell boundaries");
            worksheet.Cells["B1"].PutValue("Another cell content");
            
            // Ange kolumnbredd för att låta text gå över celler
            worksheet.Cells.SetColumnWidth(0, 5);
            
            // Skapa PDF-sparalternativ
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Demonstrera TextCrossType genom att sätta den till CrossKeep
            options.TextCrossType = TextCrossType.CrossKeep;
            
            // Spara arbetsboken som PDF
            workbook.Save("TextCrossTypeDemo.pdf", options);
            
            Console.WriteLine("PDF saved with TextCrossType.CrossKeep setting");
        }
    }
}
```

### Se även

* enum [TextCrossType](../../textcrosstype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


