---
title: Range.ClearFormats
second_title: Aspose.Cells for .NET API Reference
description: Range method. Clears the formats of this range
type: docs
url: /net/aspose.cells/range/clearformats/
---
## Range.ClearFormats method

Clears the formats of this range.

```csharp
public void ClearFormats()
```

### Examples

```csharp
namespace AsposeCellsExamples.RangeMethodClearFormatsDemo
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearFormatsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a range of cells (A1:B2)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");

            // Apply some formatting to the range
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            range.SetStyle(style);

            // Put some values in the range
            range[0, 0].PutValue("Formatted");
            range[0, 1].PutValue("Cells");
            range[1, 0].PutValue("Before");
            range[1, 1].PutValue("ClearFormats");

            try
            {
                // Clear formats by setting a default style
                Style defaultStyle = workbook.CreateStyle();
                range.SetStyle(defaultStyle);

                Console.WriteLine("Formats cleared successfully");
                Console.WriteLine($"Range {range.Address} formatting has been cleared");

                // Verify the formatting was cleared
                Cell cellAfter = range[0, 0];
                Console.WriteLine($"Cell A1 font after clearing formats: Bold={cellAfter.GetStyle().Font.IsBold}, Color={cellAfter.GetStyle().ForegroundColor}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error clearing formats: {ex.Message}");
            }

            // Save the result
            workbook.Save("RangeMethodClearFormatsDemo.xlsx");
        }
    }
}
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


