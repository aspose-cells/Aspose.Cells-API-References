---
title: "TextParagraph.FontAlignType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextParagraph. Определяет, где вертикально на строке текста находятся фактические слова. Это относится к вертикальному расположению символов относительно базовых линий."
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraph/fontaligntype/
---
## TextParagraph.FontAlignType property

Определяет, где вертикально на строке текста располагаются реальные слова. Это относится к вертикальному размещению символов относительно базовых линий.

```csharp
public TextFontAlignType FontAlignType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyFontAlignTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            int textboxIndex = worksheet.TextBoxes.Add(1, 1, 200, 400);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample Text\nFor Font Alignment Demo";

            // Получите первый абзац текстового поля.
            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];

            // Отобразите текущее значение FontAlignType.
            Console.WriteLine("Current FontAlignType value: " + paragraph.FontAlignType);

            // Установите FontAlignType в Bottom.
            paragraph.FontAlignType = TextFontAlignType.Bottom;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Установите FontAlignType в Center.
            paragraph.FontAlignType = TextFontAlignType.Center;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Установите FontAlignType в Top.
            paragraph.FontAlignType = TextFontAlignType.Top;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Сохраните книгу, чтобы увидеть эффекты
            workbook.Save("TextParagraphPropertyFontAlignTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextFontAlignType](../../textfontaligntype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


