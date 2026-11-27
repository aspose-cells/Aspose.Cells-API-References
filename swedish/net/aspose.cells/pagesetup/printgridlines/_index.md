---
title: "PageSetup.PrintGridlines"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Anger om cellrutnät skrivs ut på sidan"
type: docs
url: /sv/net/aspose.cells/pagesetup/printgridlines/
---
## PageSetup.PrintGridlines property

Anger om cellrutnät skrivs ut på sidan.

```csharp
public bool PrintGridlines { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintGridlinesDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Placera exempeldata i cell
            worksheet.Cells["A1"].PutValue("PrintGridlines Property Demo");
            worksheet.Cells["A3"].PutValue("Gridlines will ");
            worksheet.Cells["B3"].PutValue(worksheet.PageSetup.PrintGridlines ? "appear" : "not appear");
            worksheet.Cells["A4"].PutValue("when printing this sheet.");

            // Växla PrintGridlines-egenskap
            worksheet.PageSetup.PrintGridlines = true;
            
            // Spara arbetsboken
            workbook.Save("PrintGridlinesDemo.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


