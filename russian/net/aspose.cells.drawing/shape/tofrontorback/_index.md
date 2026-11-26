---
title: "Shape.ToFrontOrBack"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Перемещает фигуру на передний план или отправляет её назад"
type: docs
url: /ru/net/aspose.cells.drawing/shape/tofrontorback/
---
## Shape.ToFrontOrBack method

Перемещает фигуру на передний план или отправляет её на задний план.

```csharp
public void ToFrontOrBack(int orders)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| порядки | Int32 | Если значение меньше нуля, перемещает фигуру назад. Если больше нуля, перемещает её вперёд. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodToFrontOrBackWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте две фигуры, чтобы продемонстрировать z-order
            Aspose.Cells.Drawing.Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            Aspose.Cells.Drawing.Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);

            // Переместите shape2 на 2 позиции вперёд в z-order
            shape2.ToFrontOrBack(2);

            // Переместите shape1 на 1 позицию назад в z-order
            shape1.ToFrontOrBack(-1);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


