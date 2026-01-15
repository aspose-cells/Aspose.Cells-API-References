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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearFormatsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data with formatting
            Cell cell = worksheet.Cells["A1"];
            cell.Value = "Formatted Cell";
            cell.GetStyle().Font.IsBold = true;
            cell.GetStyle().ForegroundColor = System.Drawing.Color.Yellow;
            cell.GetStyle().Pattern = BackgroundType.Solid;

            // Create a range
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B5");

            try
            {
                // Clear formats from the range
                range.ClearFormats();

                Console.WriteLine("Formats cleared successfully from range A1:B5");
                Console.WriteLine($"Cell A1 value after clearing formats: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"Cell A1 is bold after clearing formats: {worksheet.Cells["A1"].GetStyle().Font.IsBold}");

                // Save the workbook
                workbook.Save("ClearFormatsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ClearFormats: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


