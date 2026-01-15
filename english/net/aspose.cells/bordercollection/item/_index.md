---
title: BorderCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: BorderCollection property. Gets the Border element at the specified index
type: docs
url: /net/aspose.cells/bordercollection/item/
---
## BorderCollection indexer

Gets the [`Border`](../../border/) element at the specified index.

```csharp
public Border this[BorderType borderType] { get; }
```

| Parameter | Description |
| --- | --- |
| borderType | The border to be retrieved. |

### Return Value

The element at the specified index.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class BorderCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Create a sample worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to make the example meaningful
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Get the cell and its style
                Cell cell = worksheet.Cells["A1"];
                Style style = cell.GetStyle();

                // Access the BorderCollection from the style
                BorderCollection borders = style.Borders;

                // Display the current value of the Item property (read operation)
                // Note: The Item property is read-only and returns a Border object
                // The Item property requires a BorderType parameter
                Border border = borders[BorderType.LeftBorder];
                Console.WriteLine("Border type: " + border.LineStyle);
                Console.WriteLine("Border color: " + border.Color);

                // Save the result
                workbook.Save("ItemDemo.xlsx");
                Console.WriteLine("Item property has been demonstrated");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Border](../../border/)
* enum [BorderType](../../bordertype/)
* class [BorderCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


