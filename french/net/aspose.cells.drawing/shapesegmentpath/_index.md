---
title: "Classe ShapeSegmentPath"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.ShapeSegmentPath. Représente un segment de chemin dans un chemin du tracé libre"
type: docs
url: /fr/net/aspose.cells.drawing/shapesegmentpath/
---
## ShapeSegmentPath class

Représente un segment de chemin dans un tracé de forme libre.

```csharp
public class ShapeSegmentPath
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Points](../../aspose.cells.drawing/shapesegmentpath/points/) { get; } | Obtient les points du segment de chemin |
| [Type](../../aspose.cells.drawing/shapesegmentpath/type/) { get; } | Obtient le type de segment de chemin |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapeSegmentPathDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme libre à la feuille de calcul
            Shape shape = worksheet.Shapes.AddFreeform(0, 0, 0, 0, 200, 200, new ShapePath[] { new ShapePath() });

            // Obtenir le chemin géométrique de la forme
            CustomGeometry geometry = shape.Geometry as CustomGeometry;
            ShapePath shapePath = geometry.Paths[0];

            // Accéder au premier segment de chemin (si existant)
            if (shapePath.PathSegementList.Count > 0)
            {
                ShapeSegmentPath segmentPath = shapePath.PathSegementList[0];

                // Démontrer les propriétés de ShapeSegmentPath
                Console.WriteLine("Segment Path Type: " + segmentPath.Type);
                Console.WriteLine("Number of Points: " + segmentPath.Points.Count);

                // Itérer à travers les points du segment de chemin
                foreach (ShapePathPoint point in segmentPath.Points)
                {
                    Console.WriteLine($"Point coordinates: X={point.X}, Y={point.Y}");
                }
            }

            // Enregistrez le classeur
            workbook.Save("ShapeSegmentPathDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


