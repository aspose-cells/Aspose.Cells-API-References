---
title: "Shape.LowerDeltaY"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает или задает вертикальное смещение формы от её строки в нижнем правом углу"
type: docs
url: /ru/net/aspose.cells.drawing/shape/lowerdeltay/
---
## Shape.LowerDeltaY property

Получает или задает вертикальное смещение фигуры от строки её нижнего правого угла.

```csharp
public int LowerDeltaY { get; set; }
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
    public class ShapePropertyLowerDeltaYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образец формы с правильными параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Установите и продемонстрируйте свойство LowerDeltaY
            shape.LowerDeltaY = 20;
            Console.WriteLine("Initial LowerDeltaY: " + shape.LowerDeltaY);

            // Условно измените LowerDeltaY
            if (shape.LowerDeltaY == 20)
            {
                shape.LowerDeltaY = 10;
                Console.WriteLine("Modified LowerDeltaY: " + shape.LowerDeltaY);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


