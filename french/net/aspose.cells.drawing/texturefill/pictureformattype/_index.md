---
title: "TextureFill.PictureFormatType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextureFill. Obtient et définit le type de format d'image"
type: docs
url: /fr/net/aspose.cells.drawing/texturefill/pictureformattype/
---
## TextureFill.PictureFormatType property

Obtient et définit le type de format d'image.

```csharp
public FillPictureType PictureFormatType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyPictureFormatTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangulaire avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Définir le type de remplissage sur texture
            shape.Fill.FillType = FillType.Texture;
            TextureFill textureFill = shape.Fill.TextureFill;

            // Charger une image PNG minimale de 1x1 pixel (blanche)
            string base64Image = "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=";
            textureFill.ImageData = Convert.FromBase64String(base64Image);

            // Afficher le PictureFormatType actuel
            Console.WriteLine("Initial PictureFormatType: " + textureFill.PictureFormatType);

            // Passer au format empilé et activer le carrelage
            textureFill.PictureFormatType = FillPictureType.Stack;
            textureFill.IsTiling = true;

            // Ajouter une autre forme pour comparer le format étiré original
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 0, 210, 0, 100, 200);
            shape2.Fill.FillType = FillType.Texture;
            TextureFill textureFill2 = shape2.Fill.TextureFill;
            textureFill2.ImageData = Convert.FromBase64String(base64Image);

            // Enregistrer le classeur avec les deux exemples de remplissage de texture
            workbook.Save("TextureFillPictureFormatTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [FillPictureType](../../fillpicturetype/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


