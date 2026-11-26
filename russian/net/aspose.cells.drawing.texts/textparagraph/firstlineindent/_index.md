---
title: "TextParagraph.FirstLineIndent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextParagraph. Указывает размер отступа, который будет применен к первой строке текста в абзаце"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraph/firstlineindent/
---
## TextParagraph.FirstLineIndent property

Указывает размер отступа, который будет применён к первой строке текста в абзаце.

```csharp
public double FirstLineIndent { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyFirstLineIndentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 100, 300, 200, 100);
            textBox.Text = "This is a sample paragraph with multiple lines.\nFirst line should have indent.\nSecond line should be normal.";

            // Получите текстовый абзац из текстового блока
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // Отобразите текущее значение FirstLineIndent
            Console.WriteLine("Current FirstLineIndent value: " + textParagraph.FirstLineIndent);

            // Установите новое значение FirstLineIndent (20 пунктов)
            textParagraph.FirstLineIndent = 20;
            Console.WriteLine("FirstLineIndent set to: " + textParagraph.FirstLineIndent);

            // Добавьте еще один текстовый блок для сравнения с отступом по умолчанию
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 5, 150, 300, 200, 100);
            textBox2.Text = "This is a comparison paragraph without indent.\nFirst line has no indent.\nSecond line is normal.";

            // Сохраните книгу, чтобы увидеть эффекты
            workbook.Save("TextParagraphPropertyFirstLineIndentDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


