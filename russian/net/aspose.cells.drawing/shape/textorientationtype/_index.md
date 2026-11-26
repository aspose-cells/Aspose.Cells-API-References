---
title: "Shape.TextOrientationType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает тип ориентации текста формы"
type: docs
url: /ru/net/aspose.cells.drawing/shape/textorientationtype/
---
## Shape.TextOrientationType property

Получает и задает тип ориентации текста в фигуре.

```csharp
public TextOrientationType TextOrientationType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextOrientationTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);

            // Установите текст для формы
            shape.Text = "Sample Text";

            // Проверьте и измените ориентацию текста
            if (shape.TextOrientationType == TextOrientationType.NoRotation)
            {
                shape.TextOrientationType = TextOrientationType.TopToBottom;
            }

            // Сохраните книгу
            workbook.Save("ShapeTextOrientationDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextOrientationType](../../../aspose.cells/textorientationtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


