---
title: "TextureFill.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextureFill. Obtient et définit le type de texture"
type: docs
url: /fr/net/aspose.cells.drawing/texturefill/type/
---
## TextureFill.Type property

Obtient et définit le type de texture

```csharp
public TextureType Type { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangulaire pour démontrer le remplissage de texture
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);

            // Définir le type de remplissage sur texture
            shape.Fill.FillType = FillType.Texture;

            // Accéder aux propriétés de remplissage de texture
            TextureFill textureFill = shape.Fill.TextureFill;

            try
            {
                // Afficher la valeur initiale de Type
                Console.WriteLine("Initial Texture Type: " + textureFill.Type);

                // Définir un type de texture différent
                textureFill.Type = TextureType.Granite;
                Console.WriteLine("Updated Texture Type: " + textureFill.Type);

                // Démontrer un autre type de texture
                textureFill.Type = TextureType.WaterDroplets;
                Console.WriteLine("Final Texture Type: " + textureFill.Type);

                // Enregistrer le classeur pour voir l'effet
                workbook.Save("TextureFillTypeDemo.xlsx");
                Console.WriteLine("Texture fill type demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [TextureType](../../texturetype/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


