---
title: "Shape.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar och anger namnet på formen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/name/
---
## Shape.Name property

Hämtar och anger namnet på formen.

```csharp
public string Name { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en form och ange dess namn
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            shape.Name = "shape1";
            
            // Verifiera att namnet har satts
            Console.WriteLine("Shape name: " + shape.Name);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


