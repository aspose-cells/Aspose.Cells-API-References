---
title: "ShapePath.HeightPixel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapePath. Obtient la hauteur de ce chemin en unité de pixels"
type: docs
url: /fr/net/aspose.cells.drawing/shapepath/heightpixel/
---
## ShapePath.HeightPixel property

Obtient la hauteur de ce chemin en unités de pixels.

```csharp
public int HeightPixel { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyHeightPixelDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Créer un nouveau chemin de forme
                ShapePath shapePath = new ShapePath();

                // Créer un chemin rectangulaire simple
                shapePath.MoveTo(10, 10);
                shapePath.LineTo(100, 10);
                shapePath.LineTo(100, 50);
                shapePath.LineTo(10, 50);
                shapePath.Close();

                // Afficher la valeur actuelle de HeightPixel
                Console.WriteLine("Initial HeightPixel value: " + shapePath.HeightPixel);

                // Définir une nouvelle valeur de hauteur
                shapePath.HeightPixel = 200;
                Console.WriteLine("Updated HeightPixel value: " + shapePath.HeightPixel);

                // Ajouter la forme à la feuille de calcul
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                // Enregistrez le classeur
                workbook.Save("HeightPixelDemo.xlsx");
                Console.WriteLine("HeightPixel property demonstrated successfully.");
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

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


