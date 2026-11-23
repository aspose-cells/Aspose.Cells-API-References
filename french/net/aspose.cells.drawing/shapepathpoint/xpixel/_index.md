---
title: "ShapePathPoint.XPixel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapePathPoint. Lorsque l'objet est une coordonnée de position, obtenir ou définir la coordonnée x en pixels"
type: docs
url: /fr/net/aspose.cells.drawing/shapepathpoint/xpixel/
---
## ShapePathPoint.XPixel property

Lorsque l'objet est une coordonnée de position, obtenez ou définissez la coordonnée x en pixels.

```csharp
public int XPixel { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXPixelDemo
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

                // Ajouter des points avec des coordonnées
                pathPoints.Add(100, 50);
                pathPoints.Add(200, 100);

                // Accéder au premier point et démontrer la propriété XPixel
                ShapePathPoint firstPoint = pathPoints[0];

                // Afficher la valeur XPixel (opération de lecture)
                Console.WriteLine($"Initial XPixel value: {firstPoint.XPixel}");

                // Définir une nouvelle valeur pour XPixel (puisqu'elle est en lecture/écriture)
                firstPoint.XPixel = 150;
                Console.WriteLine($"Updated XPixel value: {firstPoint.XPixel}");

                // Créer un chemin de forme et ajouter les points
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

                // Ajouter le deuxième point
                ShapePathPoint secondPoint = pathPoints[1];
                path.LineTo(secondPoint.XPixel, secondPoint.YPixel);
                path.Close();

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
                workbook.Save("XPixelDemo.xlsx");
                Console.WriteLine("XPixel property demonstration completed successfully.");
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


