---
title: "ImageOrPrintOptions.GridlineType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions Eigenschaft. Gibt den Rasterlinientyp zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/gridlinetype/
---
## ImageOrPrintOptions.GridlineType property

Liest oder legt den Typ der Gitternetzlinien fest.

```csharp
public GridlineType GridlineType { get; set; }
```

### Hinweise

Standard ist der gepunktete Typ.

### Beispiele

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
            // Erstelle eine neue Arbeitsmappe und fülle Beispieldaten ein
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Book");
            worksheet.Cells["B2"].PutValue("$19.99");
            worksheet.Cells["A3"].PutValue("Pen");
            worksheet.Cells["B3"].PutValue("$2.99");

            // Erstelle eine ImageOrPrintOptions-Instanz
            ImageOrPrintOptions imageOptions = new ImageOrPrintOptions
            {
                ImageType = ImageType.Png,
                GridlineType = GridlineType.Dotted // Use valid enum value
            };

            // Aktuellen Rasterlinientyp anzeigen
            Console.WriteLine("Initial GridlineType: " + imageOptions.GridlineType);

            // Arbeitsblatt mit initialem Rasterlinientyp rendern
            SheetRender solidLineRenderer = new SheetRender(worksheet, imageOptions);
            solidLineRenderer.ToImage(0, "SolidGridlines.png");

            // Rasterlinientyp ändern und erneut rendern
            imageOptions.GridlineType = GridlineType.Hair; // Use valid enum value
            Console.WriteLine("\nModified GridlineType: " + imageOptions.GridlineType);

            SheetRender dashedLineRenderer = new SheetRender(worksheet, imageOptions);
            dashedLineRenderer.ToImage(0, "DashedGridlines.png");

            Console.WriteLine("Generated images demonstrate different gridline styles.");
        }
    }
}
```

### Siehe auch

* enum [GridlineType](../../../aspose.cells/gridlinetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


