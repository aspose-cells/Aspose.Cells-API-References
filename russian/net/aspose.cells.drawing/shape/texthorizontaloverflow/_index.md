---
title: "Shape.TextHorizontalOverflow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Возвращает и устанавливает тип горизонтального переполнения текста в фигуре, содержащей текст"
type: docs
url: /ru/net/aspose.cells.drawing/shape/texthorizontaloverflow/
---
## Shape.TextHorizontalOverflow property

Получает и задает тип горизонтального переполнения текста в фигуре, содержащей текст.

```csharp
public TextOverflowType TextHorizontalOverflow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextHorizontalOverflowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму текстового поля с правильными параметрами
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            textBox.Text = "This is a long text that will demonstrate text horizontal overflow functionality";

            // Установить начальный тип переполнения в Clip
            textBox.TextHorizontalOverflow = TextOverflowType.Clip;
            Console.WriteLine("TextHorizontalOverflow set to Clip (text will be clipped)");

            // Изменить тип переполнения на Overflow
            textBox.TextHorizontalOverflow = TextOverflowType.Overflow;
            Console.WriteLine("TextHorizontalOverflow changed to Overflow (text will overflow)");

            // Сохраните книгу
            workbook.Save("TextHorizontalOverflowDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextOverflowType](../../textoverflowtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


