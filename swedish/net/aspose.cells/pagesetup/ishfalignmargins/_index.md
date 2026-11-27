---
title: "PageSetup.IsHFAlignMargins"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Anger om sidhuvud- och sidfot marginaler är justerade med sidmarginalerna. Om denna egenskap är sann kommer vänster sidhuvud och sidfot att justeras med den vänstra marginalen och höger sidhuvud och sidfot att justeras med den högra marginalen. Detta alternativ är aktiverat som standard"
type: docs
url: /sv/net/aspose.cells/pagesetup/ishfalignmargins/
---
## PageSetup.IsHFAlignMargins property

Indikerar om marginalerna för sidhuvud och sidfot är justerade med sidmarginalerna. Om detta egenskap är true, kommer vänstra sidhuvudet och sidfoten att justeras med den vänstra marginalen, och högra sidhuvudet och sidfoten att justeras med den högra marginalen. Detta alternativ är aktiverat som standard.

```csharp
public bool IsHFAlignMargins { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFAlignMarginsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Få åtkomst till PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Ställ in IsHFAlignMargins till true
            pageSetup.IsHFAlignMargins = true;
            Console.WriteLine("IsHFAlignMargins set to: " + pageSetup.IsHFAlignMargins);

            // Ändra IsHFAlignMargins till false
            pageSetup.IsHFAlignMargins = false;
            Console.WriteLine("IsHFAlignMargins changed to: " + pageSetup.IsHFAlignMargins);

            // Spara arbetsboken
            workbook.Save("PageSetup_IsHFAlignMargins_Example.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


