---
title: "Shape.IsTextWrapped"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar och anger den textomslagstyp som formen som innehåller text har"
type: docs
url: /sv/net/aspose.cells.drawing/shape/istextwrapped/
---
## Shape.IsTextWrapped property

Hämtar och anger typ av textbrytning för figuren som innehåller text.

```csharp
public bool IsTextWrapped { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form och ange lite text
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            shape.Text = "This is a sample text that will demonstrate text wrapping functionality";

            // Demonstrera IsTextWrapped-egenskapen
            Console.WriteLine("Initial IsTextWrapped value: " + shape.IsTextWrapped);
            
            // Växla textomslag
            shape.IsTextWrapped = !shape.IsTextWrapped;
            Console.WriteLine("After toggle, IsTextWrapped value: " + shape.IsTextWrapped);

            // Spara arbetsboken
            workbook.Save("ShapeTextWrappingDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


