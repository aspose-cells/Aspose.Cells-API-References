---
title: "ImageOrPrintOptions.TiffBinarizationMethod"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Obtient ou définit la méthode utilisée lors de la conversion d'images au format 1 bpp lorsque ImageType est Tiff et TiffCompression est égal à Ccitt3 ou Ccitt4"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/
---
## ImageOrPrintOptions.TiffBinarizationMethod property

Obtient ou définit la méthode utilisée lors de la conversion d'images au format 1 bpp lorsque [`ImageType`](../imagetype/) est Tiff et que [`TiffCompression`](../tiffcompression/) est égal à Ccitt3 ou Ccitt4.

```csharp
public ImageBinarizationMethod TiffBinarizationMethod { get; set; }
```

### Remarques

La valeur par défaut est FloydSteinbergDithering.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ImageOrPrintOptionsPropertyTiffBinarizationMethodDemo
    {
        public static void Run()
        {
            // Créer un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données de dégradé pour la démonstration visuelle
            for (int i = 0; i < 15; i++)
            {
                Cell cell = worksheet.Cells[i, 0];
                cell.PutValue(i * 7);
                Style style = cell.GetStyle();
                style.BackgroundColor = Color.FromArgb(i * 18, i * 18, i * 18);
                cell.SetStyle(style);
            }

            // Configurer les options de rendu TIFF
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT3,
                TiffColorDepth = ColorDepth.Format1bpp
            };

            // Afficher la méthode de binarisation actuelle
            Console.WriteLine("Initial TiffBinarizationMethod: " + options.TiffBinarizationMethod);

            // Rendre avec la méthode de seuil par défaut
            new SheetRender(worksheet, options).ToImage(0, "ThresholdBinarization.tiff");

            // Passer au tramage Floyd‑Steinberg
            options.TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering;
            Console.WriteLine("\nModified TiffBinarizationMethod: " + options.TiffBinarizationMethod);

            // Rendre avec la nouvelle méthode
            new SheetRender(worksheet, options).ToImage(0, "DitheringBinarization.tiff");

            Console.WriteLine("\nGenerated TIFF files demonstrate different 1bpp conversion methods.");
        }
    }
}
```

### Voir aussi

* enum [ImageBinarizationMethod](../../imagebinarizationmethod/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


