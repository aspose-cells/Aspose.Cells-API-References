---
title: "ShapePath.WidthPixel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapePath. Obtient la largeur de ce chemin en unité de pixels"
type: docs
url: /fr/net/aspose.cells.drawing/shapepath/widthpixel/
---
## ShapePath.WidthPixel property

Obtient la largeur de ce chemin en unités de pixels.

```csharp
public int WidthPixel { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyWidthPixelDemo
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

                // Afficher la valeur initiale de WidthPixel
                Console.WriteLine("Initial WidthPixel value: " + shapePath.WidthPixel);

                // Définir une nouvelle valeur de largeur
                shapePath.WidthPixel = 300;
                Console.WriteLine("Updated WidthPixel value: " + shapePath.WidthPixel);

                // Ajouter la forme à la feuille de calcul
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, shapePath.WidthPixel, 200, new ShapePath[] { shapePath });

                // Enregistrez le classeur
                workbook.Save("WidthPixelDemo.xlsx");
                Console.WriteLine("WidthPixel property demonstrated successfully.");
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


