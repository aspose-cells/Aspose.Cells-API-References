---
title: "TextTabStopCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextTabStopCollection. Получает TextTabStop по индексу"
type: docs
url: /ru/net/aspose.cells.drawing.texts/texttabstopcollection/item/
---
## TextTabStopCollection indexer

Получает [`TextTabStop`](../../texttabstop/) по индексу.

```csharp
public TextTabStop this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextTabStopCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму текстового поля, содержащую символы табуляции
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 300, 50);
            shape.Text = "Left\tCenter\tRight";

            // Получить доступ к коллекции таб-стопов первого абзаца
            var textParagraph = shape.TextBody.TextParagraphs[0];
            var tabStops = textParagraph.Stops;

            // Подготовить коллекцию с известными таб-стопами
            tabStops.Clear();
            tabStops.Add(TextTabAlignmentType.Left, 50);
            tabStops.Add(TextTabAlignmentType.Center, 150);
            tabStops.Add(TextTabAlignmentType.Right, 250);

            try
            {
                // Использовать свойство Item (индексатор) для чтения конкретного таб-стопа
                TextTabStop firstStop = tabStops[0]; // Item property (read‑only)
                Console.WriteLine($"First Tab Stop -> Position: {firstStop.TabPosition}, Alignment: {firstStop.TabAlignment}");

                // Продемонстрировать чтение другого элемента
                TextTabStop secondStop = tabStops[1];
                Console.WriteLine($"Second Tab Stop -> Position: {secondStop.TabPosition}, Alignment: {secondStop.TabAlignment}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error accessing Item property: {ex.Message}");
            }

            // Сохранить книгу с изменениями
            workbook.Save("TextTabStopCollectionItemDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextTabStop](../../texttabstop/)
* class [TextTabStopCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


