---
title: "Shape.Left"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет горизонтальное смещение фигуры от её левой колонки в пикселях"
type: docs
url: /ru/net/aspose.cells.drawing/shape/left/
---
## Shape.Left property

Представляет горизонтальное смещение фигуры от её левого столбца в пикселях.

```csharp
public int Left { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте фигуру, чтобы продемонстрировать свойство Left
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Установить начальное положение Left
            shape.Left = 200;
            Console.WriteLine("Shape Left position: " + shape.Left);

            // Изменить положение Left условно
            if (shape.Left == 200)
            {
                shape.Left = 150;
                Console.WriteLine("Adjusted Shape Left position: " + shape.Left);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


