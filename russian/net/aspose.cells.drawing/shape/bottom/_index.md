---
title: "Shape.Bottom"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет ширину вертикального смещения фигур от её нижнего углового ряда в пикселях"
type: docs
url: /ru/net/aspose.cells.drawing/shape/bottom/
---
## Shape.Bottom property

Представляет ширину вертикального смещения фигуры от её нижней строки, в пикселях.

```csharp
public int Bottom { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyBottomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образец фигуры со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Установить начальное положение
            shape.Top = 200;
            shape.Left = 200;

            // Продемонстрировать свойство Bottom
            Console.WriteLine("Original Bottom position: " + shape.Bottom);

            // Изменить положение Bottom
            if (shape.Bottom == 300)  // 200 (Top) + 100 (Height)
            {
                shape.Bottom = 250;  // This will change the Top position (250 - 100 = 150)
                Console.WriteLine("New Bottom position: " + shape.Bottom);
                Console.WriteLine("New Top position: " + shape.Top);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


