---
title: "ShapePathPoint.YPixel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapePathPoint. Lorsque l'objet est une coordonnée de position, obtenez ou définissez la coordonnée y en pixels"
type: docs
url: /fr/net/aspose.cells.drawing/shapepathpoint/ypixel/
---
## ShapePathPoint.YPixel property

Lorsque l'objet est une coordonnée de position, obtenez ou définissez la coordonnée y en pixels.

```csharp
public int YPixel { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYPixelDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Créez une collection de points de chemin de forme
                ShapePathPointCollection pathPoints = new ShapePathPointCollection();

                // Ajoutez un point avec des coordonnées
                pathPoints.Add(100, 50);

                // Accédez au premier point et démontrez la propriété YPixel
                ShapePathPoint firstPoint = pathPoints[0];

                // Affichez la valeur initiale de YPixel (opération de lecture)
                Console.WriteLine($"Initial YPixel value: {firstPoint.YPixel}");

                // Définissez une nouvelle valeur pour YPixel (puisqu'elle est en lecture/écriture)
                firstPoint.YPixel = 150;
                Console.WriteLine($"Updated YPixel value: {firstPoint.YPixel}");

                // Créez un chemin de forme et utilisez le point
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

                // Ajouter une forme libre à la feuille de calcul
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // Enregistrez le classeur
                workbook.Save("YPixelDemo.xlsx");
                Console.WriteLine("YPixel property demonstration completed successfully.");
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

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


