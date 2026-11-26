---
title: "Shape.LowerDeltaX"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает или задает горизонтальное смещение фигуры от её столбца в нижнем правом углу"
type: docs
url: /ru/net/aspose.cells.drawing/shape/lowerdeltax/
---
## Shape.LowerDeltaX property

Получает или задает горизонтальное смещение фигуры от столбца её нижнего правого угла.

```csharp
public int LowerDeltaX { get; set; }
```

### Примечания

Диапазон значений от 0 до 1024.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLowerDeltaXDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Установить и продемонстрировать свойство LowerDeltaX
            shape.LowerDeltaX = 3;
            Console.WriteLine("Initial LowerDeltaX: " + shape.LowerDeltaX);

            // Изменить LowerDeltaX, если условие выполнено
            if (shape.LowerDeltaX == 3)
            {
                shape.LowerDeltaX = 1;
                Console.WriteLine("Modified LowerDeltaX: " + shape.LowerDeltaX);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


