---
title: "PageSetup.LeftMarginInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup egenskap. Representerar storleken på den vänstra marginalen i enheten tum"
type: docs
url: /sv/net/aspose.cells/pagesetup/leftmargininch/
---
## PageSetup.LeftMarginInch property

Representerar storleken på den vänstra marginalen, i enheten tum.

```csharp
public double LeftMarginInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyLeftMarginInchDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Kom åt PageSetup.
            PageSetup pageSetup = worksheet.PageSetup;

            // Ställ in vänster marginal i tum (0,39 tum = ~1 cm)
            pageSetup.LeftMarginInch = 0.39;

            // Lägg till lite data för att demonstrera marginalen
            worksheet.Cells["A1"].PutValue("Left Margin Demonstration");
            worksheet.Cells["A2"].PutValue("Left margin set to 0.39 inches");

            // Spara arbetsboken
            workbook.Save("LeftMarginInchDemo.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


