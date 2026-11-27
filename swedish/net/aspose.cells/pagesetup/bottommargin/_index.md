---
title: "PageSetup.BottomMargin"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskapen. Representerar storleken på den nedre marginalen i enheten centimeter"
type: docs
url: /sv/net/aspose.cells/pagesetup/bottommargin/
---
## PageSetup.BottomMargin property

Representerar storleken på den nedre marginalen, i enheten centimeter.

```csharp
public double BottomMargin { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBottomMarginDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange några exempeldata
            worksheet.Cells["A1"].PutValue("Sample Text for Margin Demonstration");
            
            // Konfigurera sidinställning med BottomMargin
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.BottomMargin = 0.5; // 0.5 inch bottom margin
            pageSetup.TopMargin = 1.0;    // 1 inch top margin
            pageSetup.LeftMargin = 0.75;  // 0.75 inch left margin
            pageSetup.RightMargin = 0.75; // 0.75 inch right margin

            // Spara till PDF för att demonstrera marginalerna
            workbook.Save("PageMarginsDemo.pdf", SaveFormat.Pdf);

            Console.WriteLine("Document with bottom margin of 0.5 inches created successfully.");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


