---
title: "TextParagraph.LeftMargin"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextParagraph. Указывает левый отступ абзаца"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraph/leftmargin/
---
## TextParagraph.LeftMargin property

Указывает левый отступ абзаца.

```csharp
public double LeftMargin { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyLeftMarginDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 2, 2, 200, 200);
            textBox.Text = "This is a sample text paragraph.\nSecond line of the paragraph.";

            // Получите текстовый абзац из первого абзаца текстового поля
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Отобразите текущее значение левого отступа
            Console.WriteLine("Current LeftMargin value: " + paragraph.LeftMargin);

            // Установите новое значение левого отступа (в пунктах)
            paragraph.LeftMargin = 20.0;

            // Продемонстрируйте эффект, добавив еще один текстовый блок с отступом по умолчанию
            TextBox textBox2 = worksheet.Shapes.AddTextBox(0, 3, 2, 2, 200, 200);
            textBox2.Text = "This text box has default left margin.\nCompare the indentation.";

            // Сохраните книгу, чтобы показать разницу
            workbook.Save("TextParagraphLeftMarginDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


