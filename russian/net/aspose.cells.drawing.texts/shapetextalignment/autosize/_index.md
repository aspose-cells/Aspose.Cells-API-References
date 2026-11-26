---
title: "ShapeTextAlignment.AutoSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapeTextAlignment. Указывает, автоматически ли размер фигуры подстраивается под её содержимое"
type: docs
url: /ru/net/aspose.cells.drawing.texts/shapetextalignment/autosize/
---
## ShapeTextAlignment.AutoSize property

Указывает, автоматически ли размер формы регулируется в соответствии с её содержимым.

```csharp
public bool AutoSize { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyAutoSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму текстового поля
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 100, 200);
            textBox.Text = "This is a sample text that will demonstrate AutoSize property functionality";

            // Получить выравнивание текста
            ShapeTextAlignment shapeTextAlignment = textBox.TextBody.TextAlignment;

            // Продемонстрировать AutoSize = false (по умолчанию)
            shapeTextAlignment.AutoSize = false;
            Console.WriteLine("AutoSize false - Fixed size: " + textBox.Width + "x" + textBox.Height);

            // Продемонстрировать AutoSize = true
            shapeTextAlignment.AutoSize = true;
            Console.WriteLine("AutoSize true - Auto sized: " + textBox.Width + "x" + textBox.Height);

            // Сохраните книгу
            workbook.Save("ShapeTextAlignmentAutoSizeDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


