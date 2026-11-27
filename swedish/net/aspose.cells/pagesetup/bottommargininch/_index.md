---
title: "PageSetup.BottomMarginInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Anger storleken på den nedre marginalen i tum"
type: docs
url: /sv/net/aspose.cells/pagesetup/bottommargininch/
---
## PageSetup.BottomMarginInch property

Representerar storleken på den nedre marginalen, i enheten tum.

```csharp
public double BottomMarginInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBottomMarginInchDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt den första kalkylbladets PageSetup
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            
            // Ställ in olika marginaler i tum
            setup.HeaderMarginInch = 0.1;
            setup.FooterMarginInch = 0.2;
            setup.TopMarginInch = 0.3;
            setup.BottomMarginInch = 0.4; // Demonstrating BottomMarginInch property
            setup.LeftMarginInch = 0.5;
            setup.RightMarginInch = 0.6;
            
            // Spara arbetsboken
            workbook.Save("PageMarginsDemo.xlsx");
            
            // Visa bekräftelse
            Console.WriteLine("Workbook saved with bottom margin set to: " + setup.BottomMarginInch + " inches");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


