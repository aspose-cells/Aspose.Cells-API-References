---
title: "Shape.LowerRightColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет индекс столбца нижнего правого угла"
type: docs
url: /ru/net/aspose.cells.drawing/shape/lowerrightcolumn/
---
## Shape.LowerRightColumn property

Представляет индекс столбца нижнего правого угла.

```csharp
public int LowerRightColumn { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLowerRightColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Установите и отобразите начальное значение LowerRightColumn
            shape.LowerRightColumn = 3;
            Console.WriteLine("Initial LowerRightColumn: " + shape.LowerRightColumn);

            // Измените LowerRightColumn, если он равен 3
            if (shape.LowerRightColumn == 3)
            {
                shape.LowerRightColumn = 1;
                Console.WriteLine("Modified LowerRightColumn: " + shape.LowerRightColumn);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


