---
title: "ShapePathPoint.Y"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapePathPoint. Obtient la coordonnée y pour cette coordonnée de position. Unité EMUs"
type: docs
url: /fr/net/aspose.cells.drawing/shapepathpoint/y/
---
## ShapePathPoint.Y property

Obtient la coordonnée y pour cette coordonnée de position. Unité EMUs.

```csharp
[Obsolete("Use ShapePathPoint.YPixel and ShapePathPoint.YAngle properties instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Y { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser les propriétés ShapePathPoint.YPixel et ShapePathPoint.YAngle. Cette propriété sera supprimée 12 mois plus tard à compter d'août 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez une collection de points de chemin de forme et ajoutez des points
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(50, 10);
            pathPoints.Add(50, 50);
            pathPoints.Add(10, 50);

            // Accédez aux points en utilisant la propriété Item
            Console.WriteLine("First point coordinates:");
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"X: {firstPoint.X}, Y: {firstPoint.Y}");

            Console.WriteLine("\nAll points in collection:");
            for (int i = 0; i < pathPoints.Count; i++)
            {
                ShapePathPoint point = pathPoints[i];
                Console.WriteLine($"Point {i}: X={point.X}, Y={point.Y}");
            }

            // Créez un chemin de forme en utilisant les points
            ShapePath path = new ShapePath();

            // Déplacer vers le point de départ
            path.MoveTo(10, 10);

            foreach (ShapePathPoint point in pathPoints)
            {
                path.LineTo(point.X, point.Y);
            }
            path.Close();

            // Ajoutez une forme libre avec le chemin configuré
            Shape shape = worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path }
                );

            // Enregistrer le classeur modifié
            workbook.Save("ShapePathPointYDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


