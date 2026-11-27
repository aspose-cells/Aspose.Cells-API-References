---
title: "PageSetup.TopMarginInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Representerar storleken på den övre marginalen i tum"
type: docs
url: /sv/net/aspose.cells/pagesetup/topmargininch/
---
## PageSetup.TopMarginInch property

Anger storleken på övermarginalen i tum.

```csharp
public double TopMarginInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyTopMarginInchDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ställ in övre marginal till 1,5 tum
            sheet.PageSetup.TopMarginInch = 1.5;

            // Hämta och skriv ut värdet för den övre marginalen
            Console.WriteLine("Top Margin (inches): " + sheet.PageSetup.TopMarginInch);

            // Spara arbetsboken
            workbook.Save("PageSetup_TopMarginInch_Example.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


