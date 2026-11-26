---
title: "Shape.MoveToRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Перемещает фигуру в указанный диапазон"
type: docs
url: /ru/net/aspose.cells.drawing/shape/movetorange/
---
## Shape.MoveToRange method

Перемещает фигуру в указанный диапазон.

```csharp
public void MoveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| bottomRow | Int32 | Индекс строки нижнего правого угла |
| rightColumn | Int32 | Индекс столбца нижнего правого угла |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodMoveToRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Переместите фигуру в конкретный диапазон
            shape.MoveToRange(12, 3, 13, 5);

            // Сохраните книгу
            workbook.Save("ShapeMoveToRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


