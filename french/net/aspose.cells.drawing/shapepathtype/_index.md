---
title: "Enum ShapePathType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Drawing.ShapePathType. Représente le type de segment de chemin"
type: docs
url: /fr/net/aspose.cells.drawing/shapepathtype/
---
## ShapePathType enumeration

Représente le type de segment de chemin.

```csharp
public enum ShapePathType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| LineTo | `1` | Segment de ligne droite |
| CubicBezierCurveTo | `3` | Courbe de Bézier cubique |
| MoveTo | `0` | Démarrer un nouveau chemin |
| Close | `128` | Si le POINT de départ et le POINT de fin ne sont pas identiques, une ligne droite unique est tracée pour relier le POINT de départ et le POINT de fin du chemin. |
| End | `4` | La fin du chemin actuel |
| Escape | `5` | Échapper |
| ArcTo | `6` | Un arc |
| Unknown | `7` | Inconnu |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Créer une forme pour démontrer les types de chemin
                Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 10, 10, 200, 200);

                // Créer un chemin géométrique personnalisé
                Geometry geometry = shape.Geometry;
                ShapePath path = new ShapePath();

                // Démontrer différentes valeurs de ShapePathType
                Console.WriteLine("Available ShapePathType values:");
                Console.WriteLine($"LineTo: {ShapePathType.LineTo}");
                Console.WriteLine($"CubicBezierCurveTo: {ShapePathType.CubicBezierCurveTo}");
                Console.WriteLine($"MoveTo: {ShapePathType.MoveTo}");
                Console.WriteLine($"Close: {ShapePathType.Close}");
                Console.WriteLine($"End: {ShapePathType.End}");

                // Appliquer certaines opérations de chemin
                path.MoveTo(10, 10);
                path.LineTo(100, 100);
                path.Close();

                // Enregistrez le classeur
                workbook.Save("ShapePathTypeDemo.xlsx");
                Console.WriteLine("Demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathType: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


