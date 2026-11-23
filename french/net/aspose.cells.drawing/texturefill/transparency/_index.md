---
title: "TextureFill.Transparency"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextureFill. Retourne ou définit le degré de transparence de la zone sous forme d'une valeur de 0,0 opaque à 1,0 clair"
type: docs
url: /fr/net/aspose.cells.drawing/texturefill/transparency/
---
## TextureFill.Transparency property

Renvoie ou définit le degré de transparence de la zone comme une valeur de 0,0 (opaque) à 1,0 (transparent).

```csharp
public double Transparency { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangle à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Définir le type de remplissage sur texture
            shape.Fill.FillType = FillType.Texture;

            // Accéder aux propriétés de remplissage de texture
            TextureFill textureFill = shape.Fill.TextureFill;

            // Définir un type de texture intégré
            textureFill.Type = TextureType.BlueTissuePaper;

            // Afficher la valeur de transparence initiale
            Console.WriteLine("Initial Transparency: " + textureFill.Transparency);

            // Modifier la transparence à 70 % (0,0 = opaque, 1,0 = totalement transparent)
            textureFill.Transparency = 0.7;
            Console.WriteLine("Updated Transparency: " + textureFill.Transparency);

            // Enregistrer le classeur avec l'effet de transparence visible
            workbook.Save("TextureFillTransparencyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


