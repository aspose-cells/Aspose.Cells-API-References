---
title: "Classe Geometry"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.Geometry. Représente une forme géométrique"
type: docs
url: /fr/net/aspose.cells.drawing/geometry/
---
## Geometry class

Représente une forme géométrique.

```csharp
public abstract class Geometry
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ShapeAdjustValues](../../aspose.cells.drawing/geometry/shapeadjustvalues/) { get; } | Obtient une collection de valeurs d'ajustement de forme |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    
    public class DrawingClassGeometryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangle à la feuille de calcul
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);

            // Accéder à la géométrie de la forme
            Geometry geometry = rectangle.Geometry;

            // Ajouter des guides d'ajustement de forme directement à la collection
            geometry.ShapeAdjustValues.Add("Roundness", 0.3);
            geometry.ShapeAdjustValues.Add("Angle", 45.0);

            // Enregistrer le classeur modifié
            workbook.Save("GeometryDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


