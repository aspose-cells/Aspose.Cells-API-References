---
title: Worksheet.GetSelectedRanges
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Gets selected ranges of cells in the designer spreadsheet
type: docs
url: /net/aspose.cells/worksheet/getselectedranges/
---
## Worksheet.GetSelectedRanges method

Gets selected ranges of cells in the designer spreadsheet.

```csharp
[Obsolete("Use Worksheet.GetSelectedAreas() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetSelectedRanges()
```

### Return Value

An ArrayList which contains selected ranges.

### Remarks

NOTE: This method is now obsolete. Instead, please use Worksheet.GetSelectedAreas() method. This property will be removed 12 months later since March 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class WorksheetMethodGetSelectedRangesDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B2"].Value = "Test Value";

            try
            {
                // Note: GetSelectedRanges is marked as obsolete in the reflection
                // This demonstrates the method call as requested
                ArrayList selectedRanges = worksheet.GetSelectedRanges();

                // Display the number of selected ranges
                Console.WriteLine($"Number of selected ranges: {selectedRanges.Count}");

                // Display each selected range
                foreach (var range in selectedRanges)
                {
                    Console.WriteLine($"Selected range: {range}");
                }

                // Save the workbook
                workbook.Save("GetSelectedRangesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


