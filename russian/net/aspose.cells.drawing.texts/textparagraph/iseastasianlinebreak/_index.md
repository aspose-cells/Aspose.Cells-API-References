---
title: "TextParagraph.IsEastAsianLineBreak"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextParagraph. Указывает, может ли восточноазиатское слово быть разбито пополам и перенесено на следующую строку без добавления дефиса."
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraph/iseastasianlinebreak/
---
## TextParagraph.IsEastAsianLineBreak property

Указывает, можно ли разрывать слово восточноазиатского происхождения и переносить его на следующую строку без добавления дефиса.

```csharp
public bool IsEastAsianLineBreak { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsEastAsianLineBreakDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            textBox.Text = "これは東アジアのテキストの例です。This is Latin text example.";

            // Получите текстовый абзац из первого абзаца текстового поля
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Отобразите текущее значение IsEastAsianLineBreak.
            Console.WriteLine("Current IsEastAsianLineBreak value: " + paragraph.IsEastAsianLineBreak);

            // Установите IsEastAsianLineBreak в false (восточноазиатские слова могут быть разбиты).
            paragraph.IsEastAsianLineBreak = false;
            Console.WriteLine("After setting IsEastAsianLineBreak to false, text may break East Asian words.");

            // Сохраните книгу с отключённым разрывом строк для восточноазиатского текста.
            workbook.Save("EastAsianLineBreakDisabled.xlsx");

            // Установите IsEastAsianLineBreak в true (восточноазиатские слова не будут разбиваться).
            paragraph.IsEastAsianLineBreak = true;
            Console.WriteLine("After setting IsEastAsianLineBreak to true, text won't break East Asian words.");

            // Сохраните книгу с включённым разрывом строк для восточноазиатского текста.
            workbook.Save("EastAsianLineBreakEnabled.xlsx");
        }
    }
}
```

### См. также

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


