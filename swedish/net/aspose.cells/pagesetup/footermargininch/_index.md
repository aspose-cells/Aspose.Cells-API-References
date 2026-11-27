---
title: "PageSetup.FooterMarginInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup egenskap. Representerar avståndet från sidans botten till sidfoten i enheten tum"
type: docs
url: /sv/net/aspose.cells/pagesetup/footermargininch/
---
## PageSetup.FooterMarginInch property

Representerar avståndet från sidans botten till sidfoten, i enheten tum.

```csharp
public double FooterMarginInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFooterMarginInchDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Öppna det första kalkylbladet och dess PageSetup
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Ställ in sidfotens marginal i tum
            pageSetup.FooterMarginInch = 0.5;
            
            // Ställ in övriga marginaler för demonstration
            pageSetup.HeaderMarginInch = 0.3;
            pageSetup.TopMarginInch = 1.0;
            pageSetup.BottomMarginInch = 1.0;
            pageSetup.LeftMarginInch = 0.75;
            pageSetup.RightMarginInch = 0.75;
            
            // Spara arbetsboken
            workbook.Save("PageSetupMargins.xlsx");
            
            // Skriv ut bekräftelse
            Console.WriteLine("Footer margin set to: " + pageSetup.FooterMarginInch + " inches");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


