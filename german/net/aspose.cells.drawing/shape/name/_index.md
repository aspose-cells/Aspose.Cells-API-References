---
title: "Shape.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Ruft den Namen der Form ab und setzt ihn."
type: docs
url: /de/net/aspose.cells.drawing/shape/name/
---
## Shape.Name property

Liest und setzt den Namen der Form.

```csharp
public string Name { get; set; }
```

### Beispiele

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
            
            // Fügen Sie eine Form hinzu und setzen Sie ihren Namen.
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            shape.Name = "shape1";
            
            // Überprüfe, ob der Name gesetzt wurde
            Console.WriteLine("Shape name: " + shape.Name);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


