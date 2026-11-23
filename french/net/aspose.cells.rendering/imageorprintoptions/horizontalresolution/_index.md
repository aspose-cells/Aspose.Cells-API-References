---
title: "ImageOrPrintOptions.HorizontalResolution"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Obtient ou définit la résolution horizontale des images générées en points par pouce"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/horizontalresolution/
---
## ImageOrPrintOptions.HorizontalResolution property

Obtient ou définit la résolution horizontale des images générées, en points par pouce.

```csharp
public int HorizontalResolution { get; set; }
```

### Remarques

La valeur par défaut est 96.

La configuration de `HorizontalResolution` et de [`VerticalResolution`](../verticalresolution/) affecte la largeur et la hauteur de l'image de sortie en pixels.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyHorizontalResolutionDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text for Image Rendering");

            // Initialiser ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            
            // Définir la résolution horizontale et verticale
            options.HorizontalResolution = 192;
            options.VerticalResolution = 192;

            // Rendre la feuille de calcul en image avec la résolution spécifiée
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "WorksheetImage_192dpi.png");

            // Démontrer différentes résolutions
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;
            renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "WorksheetImage_300dpi.png");
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


