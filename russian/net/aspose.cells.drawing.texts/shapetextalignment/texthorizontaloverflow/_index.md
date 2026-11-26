---
title: "ShapeTextAlignment.TextHorizontalOverflow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapeTextAlignment. Получает и задает тип горизонтального переполнения текста в текстовом поле"
type: docs
url: /ru/net/aspose.cells.drawing.texts/shapetextalignment/texthorizontaloverflow/
---
## ShapeTextAlignment.TextHorizontalOverflow property

Получает и задает тип горизонтального переполнения текста в текстовом поле.

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
    public class ShapeTextAlignmentPropertyTextHorizontalOverflowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму текстового поля
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 50);
            textBox.Text = "This is a long text that demonstrates horizontal overflow behavior";

            // Установить горизонтальное переполнение в Clip
            textBox.TextBody.TextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;

            // Сохраните книгу
            workbook.Save("TextHorizontalOverflowDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextOverflowType](../../../aspose.cells.drawing/textoverflowtype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


