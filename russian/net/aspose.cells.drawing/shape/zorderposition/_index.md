---
title: "Shape.ZOrderPosition"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Возвращает позицию фигуры в порядке Z-слоя"
type: docs
url: /ru/net/aspose.cells.drawing/shape/zorderposition/
---
## Shape.ZOrderPosition property

Возвращает позицию фигуры в z-порядке.

```csharp
public int ZOrderPosition { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyZOrderPositionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить три фигуры для демонстрации ZOrder
            Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);
            Shape shape3 = worksheet.Shapes.AddRectangle(90, 90, 100, 100, 0, 0);

            // Установить позиции ZOrder
            shape1.ZOrderPosition = 0;
            shape2.ZOrderPosition = 1;
            shape3.ZOrderPosition = 2;

            // Изменить ZOrder фигуры shape3, чтобы переместить её на передний план
            shape3.ZOrderPosition = 0;

            // Сохраните книгу
            workbook.Save("ShapeZOrderDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


