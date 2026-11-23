---
title: "Shape.HeightPt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente la hauteur de la forme en unité de points"
type: docs
url: /fr/net/aspose.cells.drawing/shape/heightpt/
---
## Shape.HeightPt property

Représente la hauteur de la forme, en unité de points.

```csharp
public double HeightPt { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme d'exemple avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 100);

            // Définir et obtenir la propriété HeightPt
            shape.HeightPt = 50;
            Console.WriteLine("Shape height in points: " + shape.HeightPt);

            // Modifier la hauteur si elle correspond à une condition
            if (shape.HeightPt == 50)
            {
                shape.HeightPt = 30;
                Console.WriteLine("Modified shape height: " + shape.HeightPt);
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


