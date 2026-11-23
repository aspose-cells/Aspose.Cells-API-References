---
title: "Shape.HeightInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente la hauteur de la forme en pouces"
type: docs
url: /fr/net/aspose.cells.drawing/shape/heightinch/
---
## Shape.HeightInch property

Représente la hauteur de la forme, en unité de pouces.

```csharp
public double HeightInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangulaire avec tous les paramètres requis
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // Définir et obtenir la hauteur en pouces
            shape.HeightInch = 3;
            Console.WriteLine("Shape height (inches): " + shape.HeightInch);

            // Modifier la hauteur si la condition est remplie
            if (shape.HeightInch == 3)
            {
                shape.HeightInch = 1;
                Console.WriteLine("Modified shape height (inches): " + shape.HeightInch);
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


