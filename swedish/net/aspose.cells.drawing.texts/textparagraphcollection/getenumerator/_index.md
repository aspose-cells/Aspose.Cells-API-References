---
title: "TextParagraphCollection.GetEnumerator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraphCollection-metod. Hämtar enumeratorn för styckena"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraphcollection/getenumerator/
---
## TextParagraphCollection.GetEnumerator method

Hämtar enumeratorn för styckena.

```csharp
public IEnumerator GetEnumerator()
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet med alla nödvändiga parametrar
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 200, 200, 100, 100);
            textBox.Text = "First paragraph\nSecond paragraph\nThird paragraph";

            // Hämta samlingen av textparagrafer
            TextParagraphCollection paragraphs = textBox.TextBody.TextParagraphs;

            try
            {
                // Anropa GetEnumerator-metoden
                IEnumerator enumerator = paragraphs.GetEnumerator();

                Console.WriteLine($"Number of paragraphs: {paragraphs.Count}");
                Console.WriteLine("Paragraphs:");

                // Iterera genom paragraferna med hjälp av enumeratorn
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

            // Spara resultatet
            workbook.Save("MethodGetEnumeratorDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextParagraphCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


