---
title: "ImageOrPrintOptions.VerticalResolution"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Hämtar eller anger den vertikala upplösningen för genererade bilder i punkter per tum"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/verticalresolution/
---
## ImageOrPrintOptions.VerticalResolution property

Hämtar eller anger vertikal upplösning för genererade bilder, i punkter per tum.

```csharp
public int VerticalResolution { get; set; }
```

### Anmärkningar

Standardvärdet är 96.

Att ställa in [`HorizontalResolution`](../horizontalresolution/) och `VerticalResolution` påverkar bredden och höjden på den genererade bilden i pixlar.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyVerticalResolutionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata och skapa ett diagram
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue(200);
            
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Skapa bildalternativ med specifik vertikal upplösning
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            options.VerticalResolution = 300; // Setting vertical resolution to 300 DPI
            options.HorizontalResolution = 300; // For consistency, setting horizontal resolution too

            // Spara diagram som bild med angiven upplösning
            chart.ToImage("output_chart.png", options);
            
            Console.WriteLine("Chart saved as image with vertical resolution of 300 DPI.");
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


