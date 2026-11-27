---
title: "PageSetup.RightMarginInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Representerar storleken på den högra marginalen i tum"
type: docs
url: /sv/net/aspose.cells/pagesetup/rightmargininch/
---
## PageSetup.RightMarginInch property

Anger storleken på högermarginalen i tum.

```csharp
public double RightMarginInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyRightMarginInchDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Få åtkomst till PageSetup och ställ in RightMarginInch
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.RightMarginInch = 0.75; // Set right margin to 0.75 inches

            // Lägg till några exempeldata för att se effekten
            worksheet.Cells["A1"].PutValue("Right Margin Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["B" + i].PutValue("Sample Data " + i);
            }

            // Spara arbetsboken
            workbook.Save("RightMarginInchDemo.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


