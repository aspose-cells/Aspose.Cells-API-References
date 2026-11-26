---
title: "TextParagraph.Stops"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextParagraph. Получает список табуляций."
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraph/stops/
---
## TextParagraph.Stops property

Получает список табуляций.

```csharp
public TextTabStopCollection Stops { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyStopsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте текст в ячейку и получите свойства текстового абзаца.
            worksheet.Cells["A1"].PutValue("Sample\tText\tWith\tTabs");
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            shape.Text = "Sample\tText\tWith\tTabs";
            
            // Получите текстовый абзац.
            var textOptions = shape.TextBody.TextParagraphs[0];

            // Отобразите текущий счётчик табуляций.
            Console.WriteLine("Current tab stops count: " + textOptions.Stops.Count);

            // Добавьте новые табуляции.
            textOptions.Stops.Add(TextTabAlignmentType.Left, 50);
            textOptions.Stops.Add(TextTabAlignmentType.Center, 100);
            textOptions.Stops.Add(TextTabAlignmentType.Right, 150);

            // Отобразить обновлённые табуляции
            Console.WriteLine("Updated tab stops count: " + textOptions.Stops.Count);
            for (int i = 0; i < textOptions.Stops.Count; i++)
            {
                Console.WriteLine($"Tab {i+1}: Position={textOptions.Stops[i].TabPosition}, Alignment={textOptions.Stops[i].TabAlignment}");
            }

            // Сохранить рабочую книгу, чтобы увидеть эффект
            workbook.Save("TextParagraphStopsDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextTabStopCollection](../../texttabstopcollection/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


