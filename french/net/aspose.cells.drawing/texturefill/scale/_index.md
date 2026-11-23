---
title: "TextureFill.Scale"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextureFill. Obtient et définit l'échelle du format d'image"
type: docs
url: /fr/net/aspose.cells.drawing/texturefill/scale/
---
## TextureFill.Scale property

Obtient et définit l'échelle du format d'image.

```csharp
public double Scale { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TextureFillPropertyScaleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme et obtenir son format de remplissage
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 10, 10, 500, 300);
            FillFormat fillFormat = shape.Fill;

            // Configurer le remplissage de texture
            fillFormat.FillType = FillType.Texture;
            TextureFill textureFill = fillFormat.TextureFill;

            // Charger l'image de texture et configurer les propriétés
            textureFill.ImageData = File.ReadAllBytes("texture.jpg");
            textureFill.Type = TextureType.Unknown; // Changed from UserDefined to Unknown
            textureFill.IsTiling = true;

            // Afficher et modifier l'échelle
            Console.WriteLine("Initial Scale: " + textureFill.Scale);
            textureFill.Scale = 0.5;
            Console.WriteLine("Modified Scale: " + textureFill.Scale);

            // Enregistrer le résultat
            workbook.Save("TextureFillScaleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


