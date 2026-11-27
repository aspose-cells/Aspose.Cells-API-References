---
title: "PageSetup.IsPercentScale"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Om denna egenskap är falsk styr FitToPagesWide- och FitToPagesTall-egenskaperna hur kalkylbladet skalas"
type: docs
url: /sv/net/aspose.cells/pagesetup/ispercentscale/
---
## PageSetup.IsPercentScale property

Om detta egenskap är False, styr egenskaperna FitToPagesWide och FitToPagesTall hur arbetsbladet skalas.

```csharp
public bool IsPercentScale { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsPercentScaleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Öppna PageSetup och ställ in skalning till 80% (procentskala)
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.Zoom = 80;
            pageSetup.IsPercentScale = true;

            // Visa inställningarna för att demonstrera IsPercentScale
            Console.WriteLine("Zoom: " + pageSetup.Zoom);
            Console.WriteLine("IsPercentScale: " + pageSetup.IsPercentScale);

            // Spara arbetsboken
            workbook.Save("PageSetup_IsPercentScale_Output.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


