---
title: "ShapePathPoint.XAngle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShapePathPoint. Lorsque l'objet est un marqueur d'angle, obtenir ou définir le premier angle en degrés"
type: docs
url: /fr/net/aspose.cells.drawing/shapepathpoint/xangle/
---
## ShapePathPoint.XAngle property

Lorsque l'objet est un marqueur d'angle, obtenez ou définissez le premier angle en degrés.

```csharp
public int XAngle { get; set; }
```

### Remarques

Si cet angle est l'angle de départ d'un arc. Cet angle spécifiera quel angle le long du chemin circulaire supposé sera utilisé comme position de départ pour tracer l'arc. Cet angle de départ sera verrouillé à la dernière position connue du stylo dans le chemin de forme. Garantissant ainsi un chemin de forme continu.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXAngleDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une collection de points de chemin de forme
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(30, 20);
            pathPoints.Add(80, 20);
            pathPoints.Add(80, 70);
            pathPoints.Add(30, 70);

            // Récupérer le premier point et afficher ses coordonnées X et Y
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"First point – X: {firstPoint.X}, Y: {firstPoint.Y}");

            // NOTE : La classe ShapePathPoint (selon la réflexion actuelle de l'API) n'expose pas de propriété XAngle.
            // Par conséquent, cette démo se concentre sur les propriétés X et Y disponibles.

            // Construire une forme libre simple en utilisant les points définis
            ShapePath path = new ShapePath();
            path.MoveTo(firstPoint.X, firstPoint.Y);
            for (int i = 1; i < pathPoints.Count; i++)
            {
                ShapePathPoint pt = pathPoints[i];
                path.LineTo(pt.X, pt.Y);
            }
            path.Close();

            // Ajouter la forme libre à la feuille de calcul
            worksheet.Shapes.AddFreeform(
                topRow: 2,
                top: 0,
                leftColumn: 2,
                left: 0,
                height: 200,
                width: 200,
                paths: new ShapePath[] { path });

            // Enregistrez le classeur
            workbook.Save("ShapePathPointXAngleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


