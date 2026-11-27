---
title: "PageSetup.HeaderMarginInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Representerar avståndet från sidans topp till rubriken i tum"
type: docs
url: /sv/net/aspose.cells/pagesetup/headermargininch/
---
## PageSetup.HeaderMarginInch property

Representerar avståndet från sidans topp till sidhuvudet, i enheten tum.

```csharp
public double HeaderMarginInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyHeaderMarginInchDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Få åtkomst till det första kalkylbladet och dess PageSetup
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Ställ in rubrikmarginal i tum
            pageSetup.HeaderMarginInch = 0.5;
            
            // Ställ in övriga marginaler för demonstration
            pageSetup.FooterMarginInch = 0.25;
            pageSetup.TopMarginInch = 1.0;
            pageSetup.BottomMarginInch = 1.0;
            pageSetup.LeftMarginInch = 0.75;
            pageSetup.RightMarginInch = 0.75;

            // Spara arbetsboken
            workbook.Save("PageSetupMargins.xlsx");

            // Visa rubrikmarginalens värde
            Console.WriteLine("Header Margin (inches): " + pageSetup.HeaderMarginInch);
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


