---
title: "TextBoxOptions.AllowTextToOverflow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "TextBoxOptions property. Позволяет ли текст выходить за пределы фигуры"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/
---
## TextBoxOptions.AllowTextToOverflow property

Разрешено ли переполнение текста за пределы формы.

```csharp
public bool AllowTextToOverflow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyAllowTextToOverflowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);

            // Установите текст, который может выходить за пределы
            textBox.Text = "This is a long text that might overflow the text box boundaries if AllowTextToOverflow is false";

            // Включите выход текста за пределы
            textBox.TextBoxOptions.AllowTextToOverflow = true;

            // Сохраните книгу
            workbook.Save("TextBoxAllowTextToOverflowDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


