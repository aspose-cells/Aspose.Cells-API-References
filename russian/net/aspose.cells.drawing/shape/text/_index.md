---
title: "Shape.Text"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает текст этой фигуры"
type: docs
url: /ru/net/aspose.cells.drawing/shape/text/
---
## Shape.Text property

Получает и задает текст этой фигуры.

```csharp
public string Text { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму с правильными параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Установить текст, если он null
            if (shape.Text == null)
            {
                shape.Text = "This is a test.";
            }

            // Изменить текст
            shape.Text = "Updated text demo";

            // Сохраните книгу
            workbook.Save("ShapeTextDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


