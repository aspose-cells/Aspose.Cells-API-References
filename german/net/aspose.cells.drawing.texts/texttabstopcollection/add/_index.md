---
title: "TextTabStopCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextTabStopCollection-Methode. Fügt einen Tabstopp hinzu"
type: docs
url: /de/net/aspose.cells.drawing.texts/texttabstopcollection/add/
---
## TextTabStopCollection.Add method

Fügt einen Tabulator hinzu.

```csharp
public int Add(TextTabAlignmentType tabAlignment, double tabPosition)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tabAlignment | TextTabAlignmentType |  |
| tabPosition | Double |  |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Form, um Text mit Tabstopps hinzuzufügen
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            var textParagraph = shape.TextBody.TextParagraphs[0];
            
            // Erhalte die TextTabStopCollection
            var tabStops = textParagraph.Stops;

            try
            {
                // Rufe die Add-Methode mit TextTabAlignmentType.Left und Position 50.0 auf
                int index1 = tabStops.Add(TextTabAlignmentType.Left, 50.0);
                
                // Rufe die Add-Methode mit TextTabAlignmentType.Right und Position 100.0 auf
                int index2 = tabStops.Add(TextTabAlignmentType.Right, 100.0);
                
                // Füge Text mit Tabs hinzu, um die Tabstopps zu demonstrieren
                shape.Text = "Left-aligned\tRight-aligned";

                Console.WriteLine("Added tab stops at positions 50.0 (Left) and 100.0 (Right)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("TextTabStopCollectionMethodAddDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextTabAlignmentType](../../texttabalignmenttype/)
* class [TextTabStopCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


