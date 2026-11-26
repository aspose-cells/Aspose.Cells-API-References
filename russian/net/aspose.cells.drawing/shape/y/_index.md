---
title: "Shape.Y"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает вертикальное смещение shape от верхней границы листа в пикселях"
type: docs
url: /ru/net/aspose.cells.drawing/shape/y/
---
## Shape.Y property

Получает и задает вертикальное смещение фигуры от верхнего края листа в пикселях.

```csharp
public int Y { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyYDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Установите и продемонстрируйте свойство Y
            shape.Y = 200;
            Console.WriteLine("Shape Y position: " + shape.Y);

            // Измените позицию Y в зависимости от условия
            if (shape.Y == 200)
                shape.Y = 100;

            Console.WriteLine("Updated Shape Y position: " + shape.Y);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


