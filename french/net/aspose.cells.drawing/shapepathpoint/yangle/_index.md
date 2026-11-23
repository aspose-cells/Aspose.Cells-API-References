---
title: "ShapePathPoint.YAngle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapePathPoint. Lorsque l'objet est un repère d'angle, obtenez ou définissez le deuxième angle en degrés"
type: docs
url: /fr/net/aspose.cells.drawing/shapepathpoint/yangle/
---
## ShapePathPoint.YAngle property

Lorsque l'objet est un marqueur d'angle, obtenez ou définissez le deuxième angle en degrés.

```csharp
public int YAngle { get; set; }
```

### Remarques

Si cet angle est l'angle d'oscillation d'un arc. Cet angle spécifiera jusqu'où, en termes d'angle, le long du chemin circulaire supposé l'arc sera prolongé. L'extension à partir de l'angle de départ sera toujours dans le sens horaire autour du cercle supposé.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYAngleDemo
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

                // Ajoutez des points avec des repères d'angle (en utilisant XAngle et YAngle)
                ShapePathPoint point1 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point1.XAngle = 45;  // First angle in degrees
                point1.YAngle = 90;  // Second angle in degrees

                // Affichez la valeur YAngle
                Console.WriteLine($"Point 1 YAngle: {point1.YAngle} degrees");

                // Créer un autre point avec des angles différents
                ShapePathPoint point2 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point2.XAngle = 30;
                point2.YAngle = 60;

                // Affichez la valeur YAngle
                Console.WriteLine($"Point 2 YAngle: {point2.YAngle} degrees");

                // Créer un chemin de forme et ajouter un arc en utilisant des marqueurs d'angle
                ShapePath path = new ShapePath();
                path.ArcTo(point1.XAngle, point1.YAngle, 100, 100);

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
                workbook.Save("YAngleDemo.xlsx");
                Console.WriteLine("YAngle property demonstration completed successfully.");
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


