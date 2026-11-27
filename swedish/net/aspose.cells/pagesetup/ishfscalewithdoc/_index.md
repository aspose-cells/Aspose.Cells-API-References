---
title: "PageSetup.IsHFScaleWithDoc"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Anger om sidhuvud och sidfot skalas med dokumentets skalning. Gäller endast för Excel 2007."
type: docs
url: /sv/net/aspose.cells/pagesetup/ishfscalewithdoc/
---
## PageSetup.IsHFScaleWithDoc property

Indikerar om sidhuvud och sidfot skalas med dokumentets skalning. Gäller endast för Excel 2007.

```csharp
public bool IsHFScaleWithDoc { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFScaleWithDocDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Kom åt PageSetup.
            PageSetup pageSetup = worksheet.PageSetup;

            // Ställ in grundläggande sidinställning.
            pageSetup.Orientation = PageOrientationType.Landscape;
            pageSetup.PaperSize = PaperSizeType.PaperA4;

            // Demonstrera IsHFScaleWithDoc-egenskapen.
            pageSetup.IsHFScaleWithDoc = true;
            Console.WriteLine("Header/Footer scaling with document is set to: " + pageSetup.IsHFScaleWithDoc);

            // Spara arbetsboken
            workbook.Save("PageSetup_IsHFScaleWithDoc_Demo.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


