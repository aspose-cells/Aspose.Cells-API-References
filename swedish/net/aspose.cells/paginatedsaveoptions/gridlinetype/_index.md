---
title: "PaginatedSaveOptions.GridlineType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions egenskap. Hämtar eller anger rutnätslinjetyp"
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/gridlinetype/
---
## PaginatedSaveOptions.GridlineType property

Hämtar eller anger typ av rutnätslinje.

```csharp
public GridlineType GridlineType { get; set; }
```

### Anmärkningar

Standard är prickad typ.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyGridlineTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata och aktivera rutnätslinjer
            worksheet.Cells["A1"].PutValue("GridlineType Demo");
            worksheet.Cells["B2"].PutValue(1);
            worksheet.Cells["C3"].PutValue(2);
            worksheet.Cells["D4"].PutValue(3);
            worksheet.IsGridlinesVisible = true;

            // Skapa PDF-sparalternativ
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Demonstrera GridlineType-egenskapen
            pdfSaveOptions.GridlineType = GridlineType.Dotted;

            // Spara arbetsboken med rutnätslinjer
            workbook.Save("GridlineTypeDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Se även

* enum [GridlineType](../../gridlinetype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


