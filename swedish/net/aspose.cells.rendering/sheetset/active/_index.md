---
title: "SheetSet.Active"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SheetSet-egenskap. Hämtar en uppsättning med det aktiva bladet i arbetsboken"
type: docs
url: /sv/net/aspose.cells.rendering/sheetset/active/
---
## SheetSet.Active property

Hämtar en uppsättning med det aktiva bladet i arbetsboken.

```csharp
public static SheetSet Active { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyActiveDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med två kalkylblad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // Ställ in det andra kalkylbladet som aktivt
            workbook.Worksheets.ActiveSheetIndex = 1;

            // Lägg till data i båda kalkylbladen
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Active Sheet Data");

            // Skapa PDF-sparalternativ
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Spara endast det aktiva bladet
            pdfSaveOptions.SheetSet = SheetSet.Active;
            workbook.Save("ActiveSheetOnly.pdf", pdfSaveOptions);

            // Spara alla blad för jämförelse
            pdfSaveOptions.SheetSet = SheetSet.All;
            workbook.Save("AllSheets.pdf", pdfSaveOptions);
        }
    }
}
```

### Se även

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


