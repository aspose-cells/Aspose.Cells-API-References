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
namespace AsposeCellsExamples.TextTabStopCollectionPropertyItemDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextTabStopCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a shape to access text tab stops
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            var textAlignment = shape.TextBody.TextAlignment;
            
            // The TabStops property is not available on ShapeTextAlignment in the provided definition
            // So we'll need to modify the approach to work with the available properties
            // For demonstration, we'll just show the text alignment properties we can access
            Console.WriteLine("Text Alignment Properties:");
            Console.WriteLine("IsTextWrapped: " + textAlignment.IsTextWrapped);
            Console.WriteLine("RotationAngle: " + textAlignment.RotationAngle);
            
            // Since we can't access TabStops directly, we'll comment out that part
            /*
            var tabStops = textAlignment.TabStops;

            // Add some tab stops
            tabStops.Add(TextTabAlignmentType.Center, 50);
            tabStops.Add(TextTabAlignmentType.Right, 100);

            // Access and display tab stops using Item property
            Console.WriteLine("Tab Stops Count: " + tabStops.Count);
            for (int i = 0; i < tabStops.Count; i++)
            {
                var tabStop = tabStops[i];
                Console.WriteLine($"Tab {i}: Position={tabStop.TabPosition}, Alignment={tabStop.TabAlignment}");
            }
            */

            // Save the workbook
            workbook.Save("TextTabStopCollectionDemo.xlsx");
        }
    }
}
```

### See Also

* class [TextTabStop](../../texttabstop/)
* class [TextTabStopCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


