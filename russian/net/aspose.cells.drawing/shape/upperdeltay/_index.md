---
title: "Shape.UpperDeltaY"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает или задает вертикальное смещение фигуры от её строки в верхнем левом углу"
type: docs
url: /ru/net/aspose.cells.drawing/shape/upperdeltay/
---
## Shape.UpperDeltaY property

Получает или задает вертикальное смещение фигуры от строки её верхнего левого угла.

```csharp
public int UpperDeltaY { get; set; }
```

### Примечания

Диапазон значения от 0 до 256.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperDeltaYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте фигуру, чтобы продемонстрировать свойство UpperDeltaY
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Установите и отобразите начальное значение UpperDeltaY
            shape.UpperDeltaY = 3;
            Console.WriteLine("Initial UpperDeltaY: " + shape.UpperDeltaY);

            // Измените значение UpperDeltaY
            if (shape.UpperDeltaY == 3)
            {
                shape.UpperDeltaY = 1;
                Console.WriteLine("Modified UpperDeltaY: " + shape.UpperDeltaY);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


