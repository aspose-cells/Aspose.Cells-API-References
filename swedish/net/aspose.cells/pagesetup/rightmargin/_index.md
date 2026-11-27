---
title: "PageSetup.RightMargin"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Anger storleken på den högra marginalen i centimeter"
type: docs
url: /sv/net/aspose.cells/pagesetup/rightmargin/
---
## PageSetup.RightMargin property

Anger storleken på högermarginalen i centimeter.

```csharp
public double RightMargin { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyRightMarginDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in olika högermarginaler och spara för att demonstrera effekten
            worksheet.PageSetup.RightMargin = 0;
            workbook.Save("RightMargin_0.xlsx");

            worksheet.PageSetup.RightMargin = 1.0;
            workbook.Save("RightMargin_1.xlsx");

            worksheet.PageSetup.RightMargin = 2.5;
            workbook.Save("RightMargin_2.5.xlsx");

            // Skriv ut det aktuella värdet för högermarginalen
            Console.WriteLine("Current Right Margin: " + worksheet.PageSetup.RightMargin);
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


