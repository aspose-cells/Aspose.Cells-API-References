---
title: "Shape.IsEquation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape egenskap. Anger om formen endast innehåller en ekvation"
type: docs
url: /sv/net/aspose.cells.drawing/shape/isequation/
---
## Shape.IsEquation property

Anger om formen endast innehåller en ekvation.

```csharp
public bool IsEquation { get; }
```

### Exempel

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

            // Lägg till en ekvationsform med korrekta parametrar
            Shape equationShape = worksheet.Shapes.AddEquation(0, 0, 0, 0, 100, 100);
            equationShape.AlternativeText = "x^2 + y^2 = r^2";
            
            // Lägg till en vanlig rektangelform med korrekta parametrar
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

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


