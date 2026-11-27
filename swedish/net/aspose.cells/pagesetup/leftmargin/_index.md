---
title: "PageSetup.LeftMargin"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Representerar storleken på den vänstra marginalen i centimeter"
type: docs
url: /sv/net/aspose.cells/pagesetup/leftmargin/
---
## PageSetup.LeftMargin property

Representerar storleken på den vänstra marginalen, i enheten centimeter.

```csharp
public double LeftMargin { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyLeftMarginDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ange några exempeldata
            sheet.Cells["A1"].PutValue("Left Margin Demonstration");
            sheet.Cells["A2"].PutValue("This shows how to set page margins");

            // Ställ in vänster marginal (i tum)
            sheet.PageSetup.LeftMargin = 1.5;

            // Skriv ut värdet för vänster marginal till konsolen
            Console.WriteLine("Left Margin set to: " + sheet.PageSetup.LeftMargin + " inches");

            // Spara till PDF för att demonstrera marginalen
            string outputPath = "LeftMarginDemo.pdf";
            workbook.Save(outputPath, SaveFormat.Pdf);

            Console.WriteLine("File saved with left margin: " + outputPath);
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


