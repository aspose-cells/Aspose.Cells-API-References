---
title: "Shape.ActualLowerRightRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получить фактическую нижнюю строку"
type: docs
url: /ru/net/aspose.cells.drawing/shape/actuallowerrightrow/
---
## Shape.ActualLowerRightRow property

Получить фактическую нижнюю строку.

```csharp
public int ActualLowerRightRow { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyActualLowerRightRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить образец фигуры (прямоугольник)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 100);

            // Получить фактическую нижнюю правую строку фигуры
            int actualLowerRightRow = shape.ActualLowerRightRow;

            // Вывести результат.
            Console.WriteLine("Actual Lower Right Row of the shape: " + actualLowerRightRow);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


