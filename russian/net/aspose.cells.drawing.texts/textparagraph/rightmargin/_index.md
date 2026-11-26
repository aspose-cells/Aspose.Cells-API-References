---
title: "TextParagraph.RightMargin"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextParagraph. Указывает правый отступ абзаца"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraph/rightmargin/
---
## TextParagraph.RightMargin property

Указывает правый отступ абзаца.

```csharp
public double RightMargin { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyRightMarginDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            textBox.Text = "This is a sample text to demonstrate RightMargin property of TextParagraph.";

            // Получите текстовый абзац из первого абзаца текстового поля
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Отобразите текущее значение правого отступа
            Console.WriteLine("Current RightMargin value: " + paragraph.RightMargin);

            // Установите новое значение правого отступа (в пунктах)
            paragraph.RightMargin = 20.0;

            // Добавьте еще один текстовый блок, чтобы показать разницу
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 2, 1, 2, 200, 200);
            textBox2.Text = "This text has default RightMargin for comparison.";
            
            // Сохранить рабочую книгу, чтобы увидеть эффект
            workbook.Save("TextParagraphRightMarginDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


