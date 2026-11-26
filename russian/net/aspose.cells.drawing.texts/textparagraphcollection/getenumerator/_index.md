---
title: "TextParagraphCollection.GetEnumerator"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод TextParagraphCollection. Получает перечислитель абзацев"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraphcollection/getenumerator/
---
## TextParagraphCollection.GetEnumerator method

Получает перечислитель абзацев.

```csharp
public IEnumerator GetEnumerator()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;
    using System.Collections;

    public class TextParagraphCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле в лист с всеми необходимыми параметрами
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 200, 200, 100, 100);
            textBox.Text = "First paragraph\nSecond paragraph\nThird paragraph";

            // Получить коллекцию абзацев текста
            TextParagraphCollection paragraphs = textBox.TextBody.TextParagraphs;

            try
            {
                // Вызовите метод GetEnumerator
                IEnumerator enumerator = paragraphs.GetEnumerator();

                Console.WriteLine($"Number of paragraphs: {paragraphs.Count}");
                Console.WriteLine("Paragraphs:");

                // Итерировать абзацы с помощью перечислителя
                while (enumerator.MoveNext())
                {
                    TextParagraph paragraph = (TextParagraph)enumerator.Current;
                    Console.WriteLine(textBox.Text); // Using the text from the textbox since TextParagraph doesn't have Text property
                }

                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("MethodGetEnumeratorDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextParagraphCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


