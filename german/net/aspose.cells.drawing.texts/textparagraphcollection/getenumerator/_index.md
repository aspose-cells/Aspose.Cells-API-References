---
title: "TextParagraphCollection.GetEnumerator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextParagraphCollection-Methode. Gibt den Enumerator der Absätze zurück"
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraphcollection/getenumerator/
---
## TextParagraphCollection.GetEnumerator method

Liest den Enumerator der Absätze.

```csharp
public IEnumerator GetEnumerator()
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt mit allen erforderlichen Parametern hinzu
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 200, 200, 100, 100);
            textBox.Text = "First paragraph\nSecond paragraph\nThird paragraph";

            // Holen Sie die Textabsatzsammlung
            TextParagraphCollection paragraphs = textBox.TextBody.TextParagraphs;

            try
            {
                // Rufen Sie die GetEnumerator-Methode auf
                IEnumerator enumerator = paragraphs.GetEnumerator();

                Console.WriteLine($"Number of paragraphs: {paragraphs.Count}");
                Console.WriteLine("Paragraphs:");

                // Iterieren Sie durch die Absätze mit dem Enumerator
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

            // Ergebnis speichern
            workbook.Save("MethodGetEnumeratorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextParagraphCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


