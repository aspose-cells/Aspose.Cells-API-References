---
title: "Shape.IsEquation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt an, ob die Form ausschließlich eine Gleichung enthält"
type: docs
url: /de/net/aspose.cells.drawing/shape/isequation/
---
## Shape.IsEquation property

Gibt an, ob die Form nur eine Gleichung enthält.

```csharp
public bool IsEquation { get; }
```

### Beispiele

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

            // Füge eine Gleichungs-Form mit korrekten Parametern hinzu
            Shape equationShape = worksheet.Shapes.AddEquation(0, 0, 0, 0, 100, 100);
            equationShape.AlternativeText = "x^2 + y^2 = r^2";
            
            // Füge eine reguläre Rechteck-Form mit korrekten Parametern hinzu
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

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


