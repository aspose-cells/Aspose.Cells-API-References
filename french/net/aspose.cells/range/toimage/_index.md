---
title: "Range.ToImage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Convertit la plage en image"
type: docs
url: /fr/net/aspose.cells/range/toimage/
---
## Range.ToImage method

Convertit la plage en image.

```csharp
public byte[] ToImage(ImageOrPrintOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | ImageOrPrintOptions | Les options pour convertir cette plage en image |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RangeMethodToImageWithImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Créez un classeur à partir d'un fichier Excel d'exemple
            Workbook workbook = new Workbook("example.xlsx");
            
            // Obtenez la première feuille de calcul et ses cellules
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Créez la plage A1:J25
            Aspose.Cells.Range range = cells.CreateRange("A1:J25");
            
            // Créer des options d’image
            ImageOrPrintOptions options = new ImageOrPrintOptions()
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            
            // Convertissez la plage en image
            byte[] imageData = range.ToImage(options);
            
            // Enregistrez l'image dans un fichier
            File.WriteAllBytes("range_output.png", imageData);
        }
    }
}
```

### Voir aussi

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


