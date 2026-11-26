---
title: "TextParagraph.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextParagraph. Получает тип текстового узла"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraph/type/
---
## TextParagraph.Type property

Получает тип текстового узла.

```csharp
public override TextNodeType Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле в лист с всеми необходимыми параметрами
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 100, 200);
            var textBody = textBox.TextBody;
            textBody.Text = "Sample Text\nSecond Line";

            // Получить первый абзац из текстового тела
            var paragraphs = textBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[0];

            // Отобразить текущее значение Type
            Console.WriteLine("Current TextNodeType: " + paragraph.Type);

            // Продемонстрировать, как свойство Type влияет на поведение
            if (paragraph.Type == TextNodeType.TextParagraph)
            {
                Console.WriteLine("This is a text paragraph node");
                Console.WriteLine("You can access paragraph-specific properties like:");
                Console.WriteLine("AlignmentType: " + paragraph.AlignmentType);
                Console.WriteLine("LineSpace: " + paragraph.LineSpace);
            }
            else if (paragraph.Type == TextNodeType.TextRun)
            {
                Console.WriteLine("This is a simple text run node");
            }
            else if (paragraph.Type == TextNodeType.Equation)
            {
                Console.WriteLine("This is an equation node");
            }

            // Сохраните книгу
            workbook.Save("TextParagraphPropertyTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextNodeType](../../textnodetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


