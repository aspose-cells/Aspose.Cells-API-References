---
title: "SvgImageOptions.ImageType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SvgImageOptions-egenskap. Hämtar eller anger formatet för de genererade bilderna. Standardvärde PNG"
type: docs
url: /sv/net/aspose.cells.rendering/svgimageoptions/imagetype/
---
## SvgImageOptions.ImageType property

Hämtar eller anger formatet för de genererade bilderna. standardvärde: PNG.

```csharp
public override ImageType ImageType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SvgImageOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata och en bild
            worksheet.Cells["A1"].PutValue("Embedded Image Type Demonstration");
            int pictureIndex = worksheet.Pictures.Add(0, 1, "inputImage.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Skapa SVG-renderingsalternativ
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Visa aktuell ImageType (standard: PNG)
            Console.WriteLine("Current ImageType: " + svgOptions.ImageType);

            // Ändra bildformat för inbäddade rasterbilder
            svgOptions.ImageType = ImageType.Jpeg;

            // Spara kalkylbladets innehåll som SVG med olika bildformat
            using (MemoryStream stream = new MemoryStream())
            {
                picture.ToImage(stream, svgOptions);
                File.WriteAllBytes("output_with_jpeg.svg", stream.ToArray());
            }

            // Återställ till PNG-format
            svgOptions.ImageType = ImageType.Png;
            
            using (MemoryStream stream = new MemoryStream())
            {
                picture.ToImage(stream, svgOptions);
                File.WriteAllBytes("output_with_png.svg", stream.ToArray());
            }

            Console.WriteLine("SVG files created with different embedded image formats.");
        }
    }
}
```

### Se även

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


