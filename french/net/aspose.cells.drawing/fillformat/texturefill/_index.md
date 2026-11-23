---
title: "FillFormat.TextureFill"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FillFormat. Obtient l'objet TextureFill"
type: docs
url: /fr/net/aspose.cells.drawing/fillformat/texturefill/
---
## FillFormat.TextureFill property

Obtient l'objet `TextureFill`.

```csharp
public TextureFill TextureFill { get; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyTextureFillDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme d'image
            string imagePath = Path.Combine("your_image_directory", "texture.png");
            int pictureIndex = worksheet.Pictures.Add(0, 0, imagePath);
            Shape picture = worksheet.Shapes[pictureIndex];

            // Définir les propriétés du remplissage de texture
            picture.Fill.TextureFill.ImageData = File.ReadAllBytes(imagePath);
            picture.Fill.TextureFill.IsTiling = true;
            picture.Fill.TextureFill.Scale = 0.5;

            // Enregistrez le classeur
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextureFill](../../texturefill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


