---
title: "Shape.Geometry"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient la géométrie"
type: docs
url: /fr/net/aspose.cells.drawing/shape/geometry/
---
## Shape.Geometry property

Obtient la géométrie

```csharp
public Geometry Geometry { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyGeometryDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un shape rectangle avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Vérifiez les propriétés de géométrie
            if (shape.Geometry != null)
            {
                Console.WriteLine("Shape has geometry path with " + shape.Geometry.ShapeAdjustValues.Count + " adjustment points");
                
                // Ajoutez un point d'ajustement (démontrant la modification de la géométrie)
                shape.Geometry.ShapeAdjustValues.Add("adj1", 0.5);
                Console.WriteLine("Added adjustment point. Total now: " + shape.Geometry.ShapeAdjustValues.Count);
            }

            // Enregistrez le classeur
            workbook.Save("ShapeGeometryDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Geometry](../../geometry/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


