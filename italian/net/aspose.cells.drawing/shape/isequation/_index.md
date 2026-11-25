---
title: "Shape.IsEquation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Indica se la forma contiene solo un'equazione"
type: docs
url: /it/net/aspose.cells.drawing/shape/isequation/
---
## Shape.IsEquation property

Indica se la forma contiene solo un'equazione.

```csharp
public bool IsEquation { get; }
```

### Esempi

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

            // Aggiungi una forma di equazione con parametri corretti
            Shape equationShape = worksheet.Shapes.AddEquation(0, 0, 0, 0, 100, 100);
            equationShape.AlternativeText = "x^2 + y^2 = r^2";
            
            // Aggiungi una forma rettangolare regolare con parametri corretti
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

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


