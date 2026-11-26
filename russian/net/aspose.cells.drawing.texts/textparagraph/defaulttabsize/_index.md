---
title: "TextParagraph.DefaultTabSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "TextParagraph property. Получает и задает размер по умолчанию для символа табуляции в этом абзаце"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraph/defaulttabsize/
---
## TextParagraph.DefaultTabSize property

Получает и задает размер по умолчанию символа табуляции в этом абзаце.

```csharp
public double DefaultTabSize { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyDefaultTabSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 300, 200);
            textBox.Text = "Item\tPrice\tQuantity\nPen\t$1.20\t10\nNotebook\t$2.50\t5";

            // Получите текстовый абзац из первого абзаца текстового поля
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Отобразите текущий размер табуляции по умолчанию
            Console.WriteLine("Current DefaultTabSize: " + paragraph.DefaultTabSize);

            // Установите меньший размер табуляции (по умолчанию обычно около 36 пунктов)
            paragraph.DefaultTabSize = 20.0;
            Console.WriteLine("DefaultTabSize set to: " + paragraph.DefaultTabSize);

            // Добавьте еще один текстовый блок с размером табуляции по умолчанию для сравнения
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 3, 1, 3, 300, 200);
            textBox2.Text = "Item\tPrice\tQuantity\nPen\t$1.20\t10\nNotebook\t$2.50\t5";

            // Сохраните книгу, чтобы увидеть разницу в интервале табуляции
            workbook.Save("TextParagraphDefaultTabSizeDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


