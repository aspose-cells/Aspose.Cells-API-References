---
title: "PageSetup.FitToPagesWide"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Representerar antalet sidor i bredd som kalkylbladet skalas till när det skrivs ut. Standardvärdet är 1"
type: docs
url: /sv/net/aspose.cells/pagesetup/fittopageswide/
---
## PageSetup.FitToPagesWide property

Representerar antalet sidor i bredd som arbetsbladet skalas till när det skrivs ut. Standardvärdet är 1.

```csharp
public int FitToPagesWide { get; set; }
```

### Anmärkningar

Du måste sätta FitToPagesTall till noll om du vill passa alla kolumner på en sida.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFitToPagesWideDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Sample Data 1");
            worksheet.Cells["A2"].PutValue("Sample Data 2");
            worksheet.Cells["B1"].PutValue("Sample Data 3");
            worksheet.Cells["B2"].PutValue("Sample Data 4");

            // Ställ in sidinställningsegenskaper
            worksheet.PageSetup.FitToPagesWide = 1;  // Fit to 1 page wide
            worksheet.PageSetup.FitToPagesTall = 0; // Let height adjust automatically

            // Spara arbetsboken
            workbook.Save("FitToPagesWideDemo.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


