---
title: "Shape.SoftEdges"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient et définit le rayon du flou à appliquer aux bords, en unité de points"
type: docs
url: /fr/net/aspose.cells.drawing/shape/softedges/
---
## Shape.SoftEdges property

Obtient et définit le rayon du flou à appliquer aux bords, en unités de points.

```csharp
public double SoftEdges { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySoftEdgesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un shape rectangle avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Définissez l'effet de bords doux avec un rayon de 5 points (0,5d = 5 points)
            shape.SoftEdges = 0.5d;

            // Enregistrez le classeur
            workbook.Save("SoftEdgesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


