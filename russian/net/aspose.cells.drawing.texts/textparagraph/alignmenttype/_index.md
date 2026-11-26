---
title: "TextParagraph.AlignmentType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextParagraph. Получает и задает тип горизонтального выравнивания текста абзаца"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraph/alignmenttype/
---
## TextParagraph.AlignmentType property

Получает и задает тип горизонтального выравнивания текста абзаца.

```csharp
public TextAlignmentType AlignmentType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertyAlignmentTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить форму текстового поля
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 300, 200, 100);
            textBox.Text = "First Line\nSecond Line\nThird Line";
            
            // Получить абзацы текста
            TextParagraphCollection paragraphs = textBox.TextBody.TextParagraphs;
            
            // Установить разное выравнивание для каждого абзаца
            paragraphs[0].AlignmentType = TextAlignmentType.Center;
            paragraphs[1].AlignmentType = TextAlignmentType.Left;
            paragraphs[2].AlignmentType = TextAlignmentType.Right;
            
            // Сохраните книгу
            workbook.Save("TextParagraphAlignmentDemo.xlsx");
            
            Console.WriteLine("Text paragraph alignment demo completed successfully.");
        }
    }
}
```

### См. также

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


