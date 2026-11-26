---
title: "TextBoxOptions.WrapTextInShape"
second_title: "Справочник API Aspose.Cells для .NET"
description: "TextBoxOptions property. Указывает обтекание текста внутри фигуры. False  Обтекание не будет происходить в теле текста. True  Обтекание будет происходить в теле текста"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textboxoptions/wraptextinshape/
---
## TextBoxOptions.WrapTextInShape property

Указывает перенос текста внутри формы. False - перенос текста не будет происходить. True - перенос текста будет происходить.

```csharp
public bool WrapTextInShape { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyWrapTextInShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму текстового поля с правильными параметрами
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);

            // Установите текст, который будет обтекаться внутри фигуры
            textBox.Text = "This is a long text that should wrap within the text box shape boundaries when WrapTextInShape is enabled.";

            // Включите обтекание текста внутри фигуры
            textBox.TextBoxOptions.WrapTextInShape = true;

            // Сохраните книгу
            workbook.Save("TextBoxWrapTextDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


