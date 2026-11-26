---
title: "Shape.TextDirection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Возвращает/устанавливает направление потока текста для этого объекта"
type: docs
url: /ru/net/aspose.cells.drawing/shape/textdirection/
---
## Shape.TextDirection property

Получает/задает направление потока текста для этого объекта.

```csharp
public TextDirectionType TextDirection { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextDirectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму текстового поля
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 100, 100);
            shape.Text = "Sample Text";

            // Установить и продемонстрировать свойство TextDirection
            shape.TextDirection = TextDirectionType.Context;
            Console.WriteLine("Initial TextDirection: " + shape.TextDirection);

            // Изменить направление текста
            shape.TextDirection = TextDirectionType.LeftToRight;
            Console.WriteLine("Updated TextDirection: " + shape.TextDirection);

            // Сохраните книгу
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


