---
title: "TextParagraph.Stops"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraph egenskap. Hämtar listan med tabbstopp"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/stops/
---
## TextParagraph.Stops property

Hämtar tabbstopp-listan.

```csharp
public TextTabStopCollection Stops { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till text i en cell och hämta dess textstyckeegenskaper
            worksheet.Cells["A1"].PutValue("Sample\tText\tWith\tTabs");
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            shape.Text = "Sample\tText\tWith\tTabs";
            
            // Hämta textstycket
            var textOptions = shape.TextBody.TextParagraphs[0];

            // Visa aktuellt antal tabbstopp
            Console.WriteLine("Current tab stops count: " + textOptions.Stops.Count);

            // Lägg till nya tabbstopp
            textOptions.Stops.Add(TextTabAlignmentType.Left, 50);
            textOptions.Stops.Add(TextTabAlignmentType.Center, 100);
            textOptions.Stops.Add(TextTabAlignmentType.Right, 150);

            // Visa uppdaterade tabbstopp
            Console.WriteLine("Updated tab stops count: " + textOptions.Stops.Count);
            for (int i = 0; i < textOptions.Stops.Count; i++)
            {
                Console.WriteLine($"Tab {i+1}: Position={textOptions.Stops[i].TabPosition}, Alignment={textOptions.Stops[i].TabAlignment}");
            }

            // Spara arbetsboken för att se effekten
            workbook.Save("TextParagraphStopsDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextTabStopCollection](../../texttabstopcollection/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


