---
title: "Shape.IsFlippedVertically"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene e imposta se la forma è capovolta verticalmente"
type: docs
url: /it/net/aspose.cells.drawing/shape/isflippedvertically/
---
## Shape.IsFlippedVertically property

Ottiene e imposta se la forma è capovolta verticalmente.

```csharp
public bool IsFlippedVertically { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsFlippedVerticallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            
            Console.WriteLine("Original IsFlippedVertically: " + shape.IsFlippedVertically);
            
            if (shape.IsFlippedVertically == false)
            {
                shape.IsFlippedVertically = true;
                Console.WriteLine("Shape has been flipped vertically");
            }
            
            Console.WriteLine("Current IsFlippedVertically: " + shape.IsFlippedVertically);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


