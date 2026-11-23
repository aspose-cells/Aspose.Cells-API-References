---
title: "Enum FillPictureType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.FillPictureType enum. Représente le type de remplissage d'image"
type: docs
url: /fr/net/aspose.cells.drawing/fillpicturetype/
---
## FillPictureType enumeration

Représente le type de remplissage d'image.

```csharp
public enum FillPictureType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Stretch | `0` | Étirement |
| Stack | `1` | Empilement |
| StackAndScale | `2` | StackAndScale |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassFillPictureTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire pour démontrer le remplissage d'image
            Shape shape = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 200, 200);

            // Définir les propriétés du remplissage d'image
            shape.Fill.Type = FillType.Texture;
            shape.Fill.PictureFormatType = FillPictureType.StackAndScale;

            // Utiliser une image minimale de 1x1 pixel (blanche) pour la démonstration
            string base64Image = "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=";
            shape.Fill.ImageData = Convert.FromBase64String(base64Image);

            // Ajouter une autre forme avec un type de remplissage différent
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 5, 2, 0, 200, 200);
            shape2.Fill.Type = FillType.Texture;
            shape2.Fill.PictureFormatType = FillPictureType.Stretch;
            shape2.Fill.ImageData = Convert.FromBase64String(base64Image);

            // Enregistrer le classeur avec différentes configurations de remplissage
            workbook.Save("FillPictureTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


