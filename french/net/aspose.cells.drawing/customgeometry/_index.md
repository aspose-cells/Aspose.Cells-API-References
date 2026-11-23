---
title: "Classe CustomGeometry"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.CustomGeometry. Représente une forme géométrique personnalisée"
type: docs
url: /fr/net/aspose.cells.drawing/customgeometry/
---
## CustomGeometry class

Représente une forme géométrique personnalisée.

```csharp
public class CustomGeometry : Geometry
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Paths](../../aspose.cells.drawing/customgeometry/paths/) { get; } | Obtient les informations de la collection de chemins lorsque la forme est une autoshape NotPrimitive |
| [ShapeAdjustValues](../../aspose.cells.drawing/geometry/shapeadjustvalues/) { get; } | Obtient une collection de valeurs d'ajustement de forme (héritée de [`Geometry`](../geometry/).) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassCustomGeometryDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une autoshape NotPrimitive avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 0, 0, 0, 0, 200, 300);

            // Obtenir l'instance CustomGeometry à partir de la forme
            CustomGeometry customGeometry = shape.Geometry as CustomGeometry;

            // Créer un nouveau chemin dans la collection de chemins de la géométrie
            int pathIndex = customGeometry.Paths.Add();
            ShapePath path = customGeometry.Paths[pathIndex];

            // Ajouter des segments de chemin en utilisant des appels de méthode directs
            path.MoveTo(0, 0);
            path.LineTo(1000, 0);
            path.LineTo(1000, 1000);
            path.LineTo(0, 1000);
            path.Close();

            // Enregistrez le classeur
            workbook.Save("CustomGeometryDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Geometry](../geometry/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


