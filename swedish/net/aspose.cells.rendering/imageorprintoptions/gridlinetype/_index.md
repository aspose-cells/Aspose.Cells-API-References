---
title: "ImageOrPrintOptions.GridlineType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Hämtar eller anger rutnätslinjetyp"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/gridlinetype/
---
## ImageOrPrintOptions.GridlineType property

Hämtar eller anger typ av rutnätslinje.

```csharp
public GridlineType GridlineType { get; set; }
```

### Anmärkningar

Standard är prickad typ.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyGridlineTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och fyll i exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Book");
            worksheet.Cells["B2"].PutValue("$19.99");
            worksheet.Cells["A3"].PutValue("Pen");
            worksheet.Cells["B3"].PutValue("$2.99");

            // Skapa en ImageOrPrintOptions-instans
            ImageOrPrintOptions imageOptions = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png,
                GridlineType = GridlineType.Dotted // Use valid enum value
            };

            // Visa aktuell rutnätslinjetyp
            Console.WriteLine("Initial GridlineType: " + imageOptions.GridlineType);

            // Rendera kalkylblad med initial rutnätslinjetyp
            SheetRender solidLineRenderer = new SheetRender(worksheet, imageOptions);
            solidLineRenderer.ToImage(0, "SolidGridlines.png");

            // Ändra rutnätslinjetyp och rendera igen
            imageOptions.GridlineType = GridlineType.Hair; // Use valid enum value
            Console.WriteLine("\nModified GridlineType: " + imageOptions.GridlineType);

            SheetRender dashedLineRenderer = new SheetRender(worksheet, imageOptions);
            dashedLineRenderer.ToImage(0, "DashedGridlines.png");

            Console.WriteLine("Generated images demonstrate different gridline styles.");
        }
    }
}
```

### Se även

* enum [GridlineType](../../../aspose.cells/gridlinetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


