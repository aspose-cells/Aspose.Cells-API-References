---
title: "ShapePathPointCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapePathPointCollection. Ajoute un point de chemin en unité EMU"
type: docs
url: /fr/net/aspose.cells.drawing/shapepathpointcollection/add/
---
## ShapePathPointCollection.Add method

Ajoute un point de chemin en unité EMU.

```csharp
[Obsolete("Use the MoveTo,LineTo,CubicBezierTo and ArcTo methods in ShapePath instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(int x, int y)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| x | Int32 | La coordonnée x. |
| y | Int32 | La coordonnée y. |

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser les méthodes MoveTo, LineTo, CubicBezierTo et ArcTo dans ShapePath. Cette méthode sera supprimée 12 mois plus tard, à partir d'août 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez une collection de points de chemin de forme
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();

            try
            {
                // Appelez la méthode Add avec les paramètres (Int32, Int32)
                pathPoints.Add(50, 10);
                pathPoints.Add(50, 50);
                pathPoints.Add(10, 50);

                // Créer un chemin de forme et ajouter les points
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

                // Enregistrer le résultat
                workbook.Save("ShapePathPointCollectionMethodAddWithInt32Int32Demo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ShapePathPointCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


