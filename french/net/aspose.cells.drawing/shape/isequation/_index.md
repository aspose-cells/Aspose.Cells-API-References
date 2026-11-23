---
title: "Shape.IsEquation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Indique si la forme ne contient qu'une équation"
type: docs
url: /fr/net/aspose.cells.drawing/shape/isequation/
---
## Shape.IsEquation property

Indique si la forme ne contient qu'une équation.

```csharp
public bool IsEquation { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsEquationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme d'équation avec des paramètres corrects
            Shape equationShape = worksheet.Shapes.AddEquation(0, 0, 0, 0, 100, 100);
            equationShape.AlternativeText = "x^2 + y^2 = r^2";
            
            // Ajoutez une forme rectangle régulière avec des paramètres corrects
            Shape rectangleShape = worksheet.Shapes.AddRectangle(2, 0, 0, 0, 100, 100);

            foreach (Shape shape in worksheet.Shapes)
            {
                if (shape.IsEquation)
                {
                    Console.WriteLine("Shape is an equation: " + shape.AlternativeText);
                }
                else
                {
                    Console.WriteLine("Shape is not an equation");
                }
            }
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


