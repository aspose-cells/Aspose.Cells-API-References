---
title: "Shape.AlternativeText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Возвращает или задает описательную альтернативную текстовую строку объекта Shape"
type: docs
url: /ru/net/aspose.cells.drawing/shape/alternativetext/
---
## Shape.AlternativeText property

Возвращает или задает описательную (альтернативную) текстовую строку объекта [`Shape`](../).

```csharp
public string AlternativeText { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAlternativeTextDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Установить альтернативный текст для фигуры
            shape.AlternativeText = "A rectangle shape with width 100 and height 200";

            // Сохраните книгу
            workbook.Save("ShapeAlternativeTextDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


