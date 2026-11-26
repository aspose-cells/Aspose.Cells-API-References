---
title: "Shape.TextHorizontalAlignment"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает тип горизонтального выравнивания текста в форме"
type: docs
url: /ru/net/aspose.cells.drawing/shape/texthorizontalalignment/
---
## Shape.TextHorizontalAlignment property

Получает и задает тип горизонтального выравнивания текста в фигуре.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Установите текст и выравнивание
            shape.Text = "Sample Text";
            shape.TextHorizontalAlignment = TextAlignmentType.Center;

            // Изменить выравнивание, если в данный момент Bottom
            if (shape.TextHorizontalAlignment == TextAlignmentType.Bottom)
            {
                shape.TextHorizontalAlignment = TextAlignmentType.Center;
            }

            // Сохраните книгу
            workbook.Save("ShapeTextAlignmentDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


