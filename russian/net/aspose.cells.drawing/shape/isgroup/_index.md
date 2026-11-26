---
title: "Shape.IsGroup"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Указывает, является ли эта фигура групповой фигурой"
type: docs
url: /ru/net/aspose.cells.drawing/shape/isgroup/
---
## Shape.IsGroup property

Указывает, является ли эта фигура групповой фигурой.

```csharp
public bool IsGroup { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsGroupDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 100, 0, 100, 100, 100);
            Shape[] shapesToGroup = { shape1, shape2 };
            worksheet.Shapes.Group(shapesToGroup);

            Shape shape3 = worksheet.Shapes.AddOval(0, 200, 0, 200, 100, 100);

            for (int i = 0; i < worksheet.Shapes.Count; i++)
            {
                Shape shape = worksheet.Shapes[i];
                if (shape.IsGroup)
                {
                    Console.WriteLine("Group shape found at index: " + i);
                }
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


