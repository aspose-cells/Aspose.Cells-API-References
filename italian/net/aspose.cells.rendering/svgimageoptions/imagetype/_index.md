---
title: "SvgImageOptions.ImageType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SvgImageOptions. Ottiene o imposta il formato delle immagini generate. valore predefinito PNG"
type: docs
url: /it/net/aspose.cells.rendering/svgimageoptions/imagetype/
---
## SvgImageOptions.ImageType property

Ottiene o imposta il formato delle immagini generate. valore predefinito: PNG.

```csharp
public override ImageType ImageType { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio e un'immagine
            worksheet.Cells["A1"].PutValue("Embedded Image Type Demonstration");
            int pictureIndex = worksheet.Pictures.Add(0, 1, "inputImage.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Crea opzioni di rendering SVG
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Visualizza ImageType corrente (predefinito: PNG)
            Console.WriteLine("Current ImageType: " + svgOptions.ImageType);

            // Modifica il formato immagine per le immagini raster incorporate
            svgOptions.ImageType = ImageType.Jpeg;

            // Salva il contenuto del foglio di lavoro come SVG con diversi formati immagine
            using (MemoryStream stream = new MemoryStream())
            {
                picture.ToImage(stream, svgOptions);
                File.WriteAllBytes("output_with_jpeg.svg", stream.ToArray());
            }

            // Ripristina al formato PNG
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

### Vedi anche

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


