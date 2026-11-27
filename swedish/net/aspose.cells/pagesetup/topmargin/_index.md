---
title: "PageSetup.TopMargin"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup egenskap. Representerar storleken på den övre marginalen i enheten centimeter"
type: docs
url: /sv/net/aspose.cells/pagesetup/topmargin/
---
## PageSetup.TopMargin property

Anger storleken på övermarginalen i centimeter.

```csharp
public double TopMargin { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyTopMarginDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            sheet.Cells["A1"].PutValue("Top Margin Demonstration");
            sheet.Cells["A2"].PutValue("This shows the effect of TopMargin property");

            // Ställ in sidinställningsegenskaper
            PageSetup pageSetup = sheet.PageSetup;
            pageSetup.TopMargin = 2.0; // 2 inches top margin
            pageSetup.LeftMargin = 0.5;
            pageSetup.RightMargin = 0.5;
            pageSetup.BottomMargin = 1.0;

            // Spara som PDF för att demonstrera marginalerna
            string outputPath = "TopMarginDemo.pdf";
            workbook.Save(outputPath, SaveFormat.Pdf);

            Console.WriteLine("Document with top margin of 2 inches saved to: " + outputPath);
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


