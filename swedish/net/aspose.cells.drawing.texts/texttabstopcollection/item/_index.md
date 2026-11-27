---
title: "TextTabStopCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextTabStopCollection-egenskap. Hämtar TextTabStop efter indexet"
type: docs
url: /sv/net/aspose.cells.drawing.texts/texttabstopcollection/item/
---
## TextTabStopCollection indexer

Hämtar [`TextTabStop`](../../texttabstop/) efter indexet.

```csharp
public TextTabStop this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Exempel

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
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruteform som innehåller tabulatortecken
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 300, 50);
            shape.Text = "Left\tCenter\tRight";

            // Få åtkomst till den första styckets samling av tabbstopp
            var textParagraph = shape.TextBody.TextParagraphs[0];
            var tabStops = textParagraph.Stops;

            // Förbered samlingen med kända tabbstopp
            tabStops.Clear();
            tabStops.Add(TextTabAlignmentType.Left, 50);
            tabStops.Add(TextTabAlignmentType.Center, 150);
            tabStops.Add(TextTabAlignmentType.Right, 250);

            try
            {
                // Använd Item (indexer)-egenskapen för att läsa ett specifikt tabbstopp
                TextTabStop firstStop = tabStops[0]; // Item property (read‑only)
                Console.WriteLine($"First Tab Stop -> Position: {firstStop.TabPosition}, Alignment: {firstStop.TabAlignment}");

                // Demonstrera läsning av ett annat objekt
                TextTabStop secondStop = tabStops[1];
                Console.WriteLine($"Second Tab Stop -> Position: {secondStop.TabPosition}, Alignment: {secondStop.TabAlignment}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error accessing Item property: {ex.Message}");
            }

            // Spara arbetsboken med ändringarna
            workbook.Save("TextTabStopCollectionItemDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextTabStop](../../texttabstop/)
* class [TextTabStopCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


