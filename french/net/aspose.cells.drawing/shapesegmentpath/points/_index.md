---
title: "ShapeSegmentPath.Points"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapeSegmentPath. Obtient les points du segment de chemin"
type: docs
url: /fr/net/aspose.cells.drawing/shapesegmentpath/points/
---
## ShapeSegmentPath.Points property

Obtient les points du segment de chemin

```csharp
public ShapePathPointCollection Points { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeSegmentPathPropertyPointsDemo
    {
        public static void Run()
        {// Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ShapePath path = new ShapePath();

            // Démarrer un nouveau chemin
            path.MoveTo(10, 10);

            // Dessine un segment de ligne
            path.LineTo(100, 100);

            // Accéder à la propriété PathSegementList
            ShapeSegmentPathCollection segmentPaths = path.PathSegementList;

            // Accéder au premier chemin de segment
            ShapeSegmentPath segmentPath = segmentPaths[1];

            // Afficher les informations des points
            Console.WriteLine("Number of points in segment: " + segmentPath.Points.Count);
            Console.WriteLine("Point coordinates:");
            foreach (ShapePathPoint point in segmentPath.Points)
            {
                Console.WriteLine($"X: {point.X}, Y: {point.Y}");
            }          

            //ajouter une forme libre
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });

            // Enregistrez le classeur
            workbook.Save("ShapeSegmentPathPointsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapePathPointCollection](../../shapepathpointcollection/)
* class [ShapeSegmentPath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


