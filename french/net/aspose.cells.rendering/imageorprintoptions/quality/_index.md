---
title: "ImageOrPrintOptions.Quality"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageOrPrintOptions. Obtient ou définit une valeur déterminant la qualité des images générées, appliquée uniquement lors de l’enregistrement des pages au format JPEG. La valeur par défaut est 100"
type: docs
url: /fr/net/aspose.cells.rendering/imageorprintoptions/quality/
---
## ImageOrPrintOptions.Quality property

Obtient ou définit une valeur déterminant la qualité des images générées à appliquer uniquement lors de l'enregistrement des pages au format `Jpeg`. La valeur par défaut est 100

```csharp
public int Quality { get; set; }
```

### Remarques

N’a d’effet que lors de l’enregistrement au format JPEG. La valeur doit être comprise entre 0 et 100. La valeur par défaut est 100.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyQualityDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["C3"].PutValue(DateTime.Now);

            // Créer des options d’image avec différents réglages de qualité
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;
            options.Quality = 100; // Highest quality

            // Rendre la feuille de calcul en image avec une haute qualité
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "HighQualityOutput.jpg");

            // Modifier la qualité pour démontrer la différence
            options.Quality = 50; // Medium quality
            renderer.ToImage(0, "MediumQualityOutput.jpg");

            options.Quality = 10; // Low quality
            renderer.ToImage(0, "LowQualityOutput.jpg");
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


