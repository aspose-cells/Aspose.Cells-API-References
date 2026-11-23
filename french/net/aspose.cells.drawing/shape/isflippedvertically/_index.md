---
title: "Shape.IsFlippedVertically"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient et définit si la forme est retournée verticalement"
type: docs
url: /fr/net/aspose.cells.drawing/shape/isflippedvertically/
---
## Shape.IsFlippedVertically property

Obtient et définit si la forme est retournée verticalement.

```csharp
public bool IsFlippedVertically { get; set; }
```

### Exemples

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

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


