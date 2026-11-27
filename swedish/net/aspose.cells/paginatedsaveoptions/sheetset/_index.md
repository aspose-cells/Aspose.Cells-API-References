---
title: "PaginatedSaveOptions.SheetSet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions-egenskap. Hämtar eller anger de blad som ska renderas. Standard är alla synliga blad i arbetsboken Visible"
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/sheetset/
---
## PaginatedSaveOptions.SheetSet property

Hämtar eller anger vilka blad som ska renderas. Standard är alla synliga blad i arbetsboken: [`Visible`](../../../aspose.cells.rendering/sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med två kalkylblad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Ställ in exempeldata i båda bladen
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // Skapa PDF-sparalternativ
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Spara endast det andra bladet med hjälp av SheetSet
            pdfSaveOptions.SheetSet = new SheetSet(new int[] { 1 }); // 0-based index
            
            // Spara arbetsboken med de angivna bladen
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Se även

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


