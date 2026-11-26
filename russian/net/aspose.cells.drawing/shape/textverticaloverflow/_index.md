---
title: "Shape.TextVerticalOverflow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает тип вертикального переполнения текста формы, содержащей текст"
type: docs
url: /ru/net/aspose.cells.drawing/shape/textverticaloverflow/
---
## Shape.TextVerticalOverflow property

Получает и задает тип вертикального переполнения текста в фигуре, содержащей текст.

```csharp
public TextOverflowType TextVerticalOverflow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextVerticalOverflowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);
            
            // Установите текст и заставьте его переполняться вертикально
            shape.Text = "This is a long text that will demonstrate vertical text overflow functionality in the shape.";
            shape.TextVerticalOverflow = TextOverflowType.Overflow;

            // Сохраните книгу
            workbook.Save("ShapeTextVerticalOverflowDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextOverflowType](../../textoverflowtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


