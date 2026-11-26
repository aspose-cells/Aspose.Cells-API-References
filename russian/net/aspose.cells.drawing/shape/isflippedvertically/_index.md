---
title: "Shape.IsFlippedVertically"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает, перевёрнута ли фигура по вертикали"
type: docs
url: /ru/net/aspose.cells.drawing/shape/isflippedvertically/
---
## Shape.IsFlippedVertically property

Получает и задает, вертикально ли отражена фигура.

```csharp
public bool IsFlippedVertically { get; set; }
```

### Примеры

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

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


