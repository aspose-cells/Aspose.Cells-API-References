---
title: "SvgImageOptions.ImageType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SvgImageOptions Eigenschaft. Gibt das Format der erzeugten Bilder zurück oder setzt es. Standardwert PNG"
type: docs
url: /de/net/aspose.cells.rendering/svgimageoptions/imagetype/
---
## SvgImageOptions.ImageType property

Liest oder setzt das Format der erzeugten Bilder. Standardwert: PNG.

```csharp
public override ImageType ImageType { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten und ein Bild hinzufügen
            worksheet.Cells["A1"].PutValue("Embedded Image Type Demonstration");
            int pictureIndex = worksheet.Pictures.Add(0, 1, "inputImage.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Erstelle SVG-Renderoptionen
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Zeige den aktuellen ImageType an (Standard: PNG)
            Console.WriteLine("Current ImageType: " + svgOptions.ImageType);

            // Ändere das Bildformat für eingebettete Rasterbilder
            svgOptions.ImageType = ImageType.Jpeg;

            // Speichere den Arbeitsblattinhalt als SVG mit verschiedenen Bildformaten
            using (MemoryStream stream = new MemoryStream())
            {
                picture.ToImage(stream, svgOptions);
                File.WriteAllBytes("output_with_jpeg.svg", stream.ToArray());
            }

            // Zurücksetzen auf PNG-Format
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

### Siehe auch

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


