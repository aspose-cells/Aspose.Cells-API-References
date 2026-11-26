---
title: "TextBoxOptions.ResizeToFitText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "TextBoxOptions property. Указывает, следует ли изменять размер фигуры, чтобы она соответствовала тексту"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textboxoptions/resizetofittext/
---
## TextBoxOptions.ResizeToFitText property

Указывает, следует ли изменять размер формы, чтобы вместить текст

```csharp
public bool ResizeToFitText { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyResizeToFitTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте текстовое поле с правильными параметрами
            Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(1, 1, 100, 100, 200, 50);
            textBox.Text = "This is a sample text that will make the text box resize to fit";

            // Правильно получайте доступ к TextBoxOptions
            textBox.TextBoxOptions.ResizeToFitText = true;

            // Сохраните книгу
            workbook.Save("TextBoxResizeToFitTextDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


