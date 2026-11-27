---
title: "PageSetup.IsAutomaticPaperSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup egenskap. Anger om papperstorleken är automatisk"
type: docs
url: /sv/net/aspose.cells/pagesetup/isautomaticpapersize/
---
## PageSetup.IsAutomaticPaperSize property

Indikerar om pappersstorleken är automatisk.

```csharp
public bool IsAutomaticPaperSize { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsAutomaticPaperSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Kom åt sidinställning
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Hämta automatiskt papperstorleksvärde
            Console.WriteLine("Automatic Paper Size: " + pageSetup.IsAutomaticPaperSize);
            
            // Skapa en annan arbetsbok med olika inställningar
            Workbook workbook2 = new Workbook("example.xlsx");
            PageSetup pageSetup2 = workbook2.Worksheets[0].PageSetup;
            Console.WriteLine("Automatic Paper Size from file: " + pageSetup2.IsAutomaticPaperSize);
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


