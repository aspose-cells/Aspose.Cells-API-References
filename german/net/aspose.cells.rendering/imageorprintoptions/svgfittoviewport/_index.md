---
title: "ImageOrPrintOptions.SVGFitToViewPort"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Wenn diese Eigenschaft true ist, passt das erzeugte SVG an den Viewport an"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/svgfittoviewport/
---
## ImageOrPrintOptions.SVGFitToViewPort property

Wenn diese Eigenschaft wahr ist, passt das erzeugte SVG an den Viewport an.

```csharp
[Obsolete("Use SvgImageOptions.FitToViewPort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SVGFitToViewPort { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen verwenden Sie bitte [`FitToViewPort`](../../svgimageoptions/fittoviewport/). Diese Eigenschaft wird 12 Monate später, seit April 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertySVGFitToViewPortDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            
            // Bildoptionen für SVG-Ausgabe erstellen
            ImageOrPrintOptions opts = new ImageOrPrintOptions();
            opts.ImageType = Aspose.Cells.Drawing.ImageType.Svg;
            opts.OnePagePerSheet = true;
            opts.SVGFitToViewPort = true; // This is the key property being demonstrated
            
            // Das Arbeitsblatt in ein SVG-Bild rendern
            SheetRender sr = new SheetRender(worksheet, opts);
            sr.ToImage(0, "output.svg");
            
            Console.WriteLine("SVG file with SVGFitToViewPort=true created successfully.");
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


