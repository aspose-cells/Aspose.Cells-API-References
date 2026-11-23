---
title: "Enum ImageBinarizationMethod"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Rendering.ImageBinarizationMethod enum. Spécifie la méthode utilisée pour binariser l'image"
type: docs
url: /fr/net/aspose.cells.rendering/imagebinarizationmethod/
---
## ImageBinarizationMethod enumeration

Spécifie la méthode utilisée pour binariser l'image.

```csharp
public enum ImageBinarizationMethod
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Threshold | `0` | Spécifie la méthode de seuillage. |
| FloydSteinbergDithering | `1` | Spécifie le dithérage en utilisant la méthode de diffusion d'erreur de Floyd‑Steinberg. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class RenderingClassImageBinarizationMethodDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec des données de test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir les cellules avec des valeurs de gradient à des fins de démonstration
            for (int row = 0; row < 50; row++)
            {
                for (int col = 0; col < 10; col++)
                {
                    worksheet.Cells[row, col].PutValue((double)(row * col) / 500);
                }
            }

            // Configurer les options de rendu d'image
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT4,
                TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering
            };

            // Créer le rendu de la feuille avec les options configurées
            SheetRender renderer = new SheetRender(worksheet, options);
            
            // Rendre la première page de la feuille de calcul en image avec binarisation
            renderer.ToImage(0, "BinarizedOutput.tiff");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


