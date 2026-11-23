---
title: "SvgImageOptions.ImageType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SvgImageOptions. Obtient ou définit le format des images générées. valeur par défaut PNG"
type: docs
url: /fr/net/aspose.cells.rendering/svgimageoptions/imagetype/
---
## SvgImageOptions.ImageType property

Obtient ou définit le format des images générées. Valeur par défaut : PNG.

```csharp
public override ImageType ImageType { get; set; }
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple et une image
            worksheet.Cells["A1"].PutValue("Embedded Image Type Demonstration");
            int pictureIndex = worksheet.Pictures.Add(0, 1, "inputImage.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Créer des options de rendu SVG
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Afficher le ImageType actuel (par défaut : PNG)
            Console.WriteLine("Current ImageType: " + svgOptions.ImageType);

            // Modifier le format d'image pour les images raster incorporées
            svgOptions.ImageType = ImageType.Jpeg;

            // Enregistrer le contenu de la feuille de calcul en SVG avec différents formats d'image
            using (MemoryStream stream = new MemoryStream())
            {
                picture.ToImage(stream, svgOptions);
                File.WriteAllBytes("output_with_jpeg.svg", stream.ToArray());
            }

            // Réinitialiser au format PNG
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

### Voir aussi

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


