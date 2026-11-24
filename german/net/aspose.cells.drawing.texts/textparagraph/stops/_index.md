---
title: "TextParagraph.Stops"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextParagraph-Eigenschaft. Gibt die Tabulator-Stoppliste zurück."
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraph/stops/
---
## TextParagraph.Stops property

Liest die Tabulatorliste.

```csharp
public TextTabStopCollection Stops { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einer Zelle Text hinzu und erhalten Sie deren TextParagraph-Eigenschaften.
            worksheet.Cells["A1"].PutValue("Sample\tText\tWith\tTabs");
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            shape.Text = "Sample\tText\tWith\tTabs";
            
            // Holen Sie den Textabsatz.
            var textOptions = shape.TextBody.TextParagraphs[0];

            // Zeigen Sie die aktuelle Anzahl der Tabulatorstopps an.
            Console.WriteLine("Current tab stops count: " + textOptions.Stops.Count);

            // Fügen Sie neue Tabulatorstopps hinzu.
            textOptions.Stops.Add(TextTabAlignmentType.Left, 50);
            textOptions.Stops.Add(TextTabAlignmentType.Center, 100);
            textOptions.Stops.Add(TextTabAlignmentType.Right, 150);

            // Aktualisierte Tabstopps anzeigen
            Console.WriteLine("Updated tab stops count: " + textOptions.Stops.Count);
            for (int i = 0; i < textOptions.Stops.Count; i++)
            {
                Console.WriteLine($"Tab {i+1}: Position={textOptions.Stops[i].TabPosition}, Alignment={textOptions.Stops[i].TabAlignment}");
            }

            // Speichern Sie die Arbeitsmappe, um den Effekt zu sehen
            workbook.Save("TextParagraphStopsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextTabStopCollection](../../texttabstopcollection/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


