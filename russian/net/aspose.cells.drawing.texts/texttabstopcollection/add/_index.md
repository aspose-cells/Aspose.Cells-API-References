---
title: "TextTabStopCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод TextTabStopCollection. Добавляет табуляцию"
type: docs
url: /ru/net/aspose.cells.drawing.texts/texttabstopcollection/add/
---
## TextTabStopCollection.Add method

Добавляет табуляцию.

```csharp
public int Add(TextTabAlignmentType tabAlignment, double tabPosition)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| tabAlignment | TextTabAlignmentType |  |
| tabPosition | Double |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextTabStopCollectionMethodAddWithTextTabAlignmentTypeDoubleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму для добавления текста с табуляциями
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            var textParagraph = shape.TextBody.TextParagraphs[0];
            
            // Получить TextTabStopCollection
            var tabStops = textParagraph.Stops;

            try
            {
                // Вызвать метод Add с TextTabAlignmentType.Left и позицией 50.0
                int index1 = tabStops.Add(TextTabAlignmentType.Left, 50.0);
                
                // Вызвать метод Add с TextTabAlignmentType.Right и позицией 100.0
                int index2 = tabStops.Add(TextTabAlignmentType.Right, 100.0);
                
                // Добавить текст с табуляциями для демонстрации таб-стопов
                shape.Text = "Left-aligned\tRight-aligned";

                Console.WriteLine("Added tab stops at positions 50.0 (Left) and 100.0 (Right)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("TextTabStopCollectionMethodAddDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextTabAlignmentType](../../texttabalignmenttype/)
* class [TextTabStopCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


