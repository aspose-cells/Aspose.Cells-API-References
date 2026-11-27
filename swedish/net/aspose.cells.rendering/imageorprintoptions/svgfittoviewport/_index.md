---
title: "ImageOrPrintOptions.SVGFitToViewPort"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Om denna egenskap är sann kommer den genererade svg:n att anpassas till visningsporten"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/svgfittoviewport/
---
## ImageOrPrintOptions.SVGFitToViewPort property

Om denna egenskap är sann, kommer den genererade svg att anpassas till visningsporten.

```csharp
[Obsolete("Use SvgImageOptions.FitToViewPort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SVGFitToViewPort { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället [`FitToViewPort`](../../svgimageoptions/fittoviewport/). Denna egenskap kommer att tas bort 12 månader senare sedan april 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            
            // Skapa bildalternativ för SVG-utdata
            ImageOrPrintOptions opts = new ImageOrPrintOptions();
            opts.ImageType = Aspose.Cells.Drawing.ImageType.Svg;
            opts.OnePagePerSheet = true;
            opts.SVGFitToViewPort = true; // This is the key property being demonstrated
            
            // Rendera kalkylbladet till SVG-bild
            SheetRender sr = new SheetRender(worksheet, opts);
            sr.ToImage(0, "output.svg");
            
            Console.WriteLine("SVG file with SVGFitToViewPort=true created successfully.");
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


