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
namespace AsposeCellsExamples.BorderCollectionPropertyItemDemo
{
    using Aspose.Cells;
    using System;

    public class BorderCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access cell A1 and get its style
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();

            // Get the BorderCollection from the style
            BorderCollection borders = style.Borders;

            // Demonstrate reading the Item property for different border types
            Border topBorder = borders[BorderType.TopBorder];
            Console.WriteLine("Top Border Style: " + topBorder.LineStyle);
            Console.WriteLine("Top Border Color: " + topBorder.Color);

            // Change border properties through the Item property
            borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;

            borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dotted;
            borders[BorderType.BottomBorder].Color = System.Drawing.Color.Blue;

            // Apply the modified style back to the cell
            cell.SetStyle(style);

            // Expand the cell to make borders more visible
            worksheet.Cells.SetRowHeight(0, 30);
            worksheet.Cells.SetColumnWidth(0, 20);

            // Save the result
            workbook.Save("BorderCollectionPropertyItemDemo.xlsx");
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


