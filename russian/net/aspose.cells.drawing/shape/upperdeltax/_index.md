---
title: "Shape.UpperDeltaX"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает или задает горизонтальное смещение формы от её столбца в верхнем левом углу"
type: docs
url: /ru/net/aspose.cells.drawing/shape/upperdeltax/
---
## Shape.UpperDeltaX property

Получает или задает горизонтальное смещение фигуры от столбца её верхнего левого угла.

```csharp
public int UpperDeltaX { get; set; }
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
    public class ShapePropertyUpperDeltaXDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Задайте и отобразите свойство UpperDeltaX
            shape.UpperDeltaX = 150;
            Console.WriteLine("UpperDeltaX: " + shape.UpperDeltaX);

            // Измените UpperDeltaX, если выполнено условие
            if (shape.UpperDeltaX == 150)
            {
                shape.UpperDeltaX = 100;
                Console.WriteLine("Modified UpperDeltaX: " + shape.UpperDeltaX);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


