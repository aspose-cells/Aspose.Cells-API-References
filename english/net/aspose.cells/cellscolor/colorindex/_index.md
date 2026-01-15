---
title: CellsColor.ColorIndex
second_title: Aspose.Cells for .NET API Reference
description: CellsColor property. Gets and sets the color index in the color palette. Only applies of indexed color
type: docs
url: /net/aspose.cells/cellscolor/colorindex/
---
## CellsColor.ColorIndex property

Gets and sets the color index in the color palette. Only applies of indexed color.

```csharp
public int ColorIndex { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;

    public class CellsColorPropertyColorIndexDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Define a range to which we will apply a colored border
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:D4");

            // Create a CellsColor instance
            CellsColor cellsColor = workbook.CreateCellsColor();

            // Set the ColorIndex (palette index) – for example, 5
            cellsColor.ColorIndex = 5;

            // Apply the CellsColor as the inside border color of the range
            range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical,
                                   CellBorderType.Thin,
                                   cellsColor);

            // Read and display the current ColorIndex value
            Console.WriteLine("Current ColorIndex value: " + cellsColor.ColorIndex);

            // Save the workbook to visualize the result
            try
            {
                workbook.Save("ColorIndexDemo.xlsx");
                Console.WriteLine("Workbook saved as ColorIndexDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


