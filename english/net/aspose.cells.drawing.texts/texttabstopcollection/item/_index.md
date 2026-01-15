---
title: TextTabStopCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: TextTabStopCollection property. Gets TextTabStop by the index
type: docs
url: /net/aspose.cells.drawing.texts/texttabstopcollection/item/
---
## TextTabStopCollection indexer

Gets [`TextTabStop`](../../texttabstop/) by the index.

```csharp
public TextTabStop this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

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
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a textbox shape containing tab characters
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 300, 50);
            shape.Text = "Left\tCenter\tRight";

            // Access the first paragraph's tab stops collection
            var textParagraph = shape.TextBody.TextParagraphs[0];
            var tabStops = textParagraph.Stops;

            // Prepare the collection with known tab stops
            tabStops.Clear();
            tabStops.Add(TextTabAlignmentType.Left, 50);
            tabStops.Add(TextTabAlignmentType.Center, 150);
            tabStops.Add(TextTabAlignmentType.Right, 250);

            try
            {
                // Use the Item (indexer) property to read a specific tab stop
                TextTabStop firstStop = tabStops[0]; // Item property (read‑only)
                Console.WriteLine($"First Tab Stop -> Position: {firstStop.TabPosition}, Alignment: {firstStop.TabAlignment}");

                // Demonstrate reading another item
                TextTabStop secondStop = tabStops[1];
                Console.WriteLine($"Second Tab Stop -> Position: {secondStop.TabPosition}, Alignment: {secondStop.TabAlignment}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error accessing Item property: {ex.Message}");
            }

            // Save the workbook with the changes
            workbook.Save("TextTabStopCollectionItemDemo.xlsx");
        }
    }
}
```

### See Also

* class [TextTabStop](../../texttabstop/)
* class [TextTabStopCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


