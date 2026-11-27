---
title: "TextTabStopCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextTabStopCollection-metod. Lägger till ett tabbstopp"
type: docs
url: /sv/net/aspose.cells.drawing.texts/texttabstopcollection/add/
---
## TextTabStopCollection.Add method

Lägger till ett tabbstopp.

```csharp
public int Add(TextTabAlignmentType tabAlignment, double tabPosition)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tabAlignment | TextTabAlignmentType |  |
| tabPosition | Double |  |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en form för att lägga till text med tabbstopp
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            var textParagraph = shape.TextBody.TextParagraphs[0];
            
            // Hämta TextTabStopCollection
            var tabStops = textParagraph.Stops;

            try
            {
                // Anropa Add-metoden med TextTabAlignmentType.Left och position 50.0
                int index1 = tabStops.Add(TextTabAlignmentType.Left, 50.0);
                
                // Anropa Add-metoden med TextTabAlignmentType.Right och position 100.0
                int index2 = tabStops.Add(TextTabAlignmentType.Right, 100.0);
                
                // Lägg till text med tabbar för att demonstrera tabbstoppen
                shape.Text = "Left-aligned\tRight-aligned";

                Console.WriteLine("Added tab stops at positions 50.0 (Left) and 100.0 (Right)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("TextTabStopCollectionMethodAddDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextTabAlignmentType](../../texttabalignmenttype/)
* class [TextTabStopCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


