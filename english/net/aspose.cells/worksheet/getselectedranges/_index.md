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
namespace AsposeCellsExamples.WorksheetMethodGetSelectedRangesDemo
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class WorksheetMethodGetSelectedRangesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Select multiple ranges in the worksheet
            worksheet.SelectRange(0, 0, 2, 2, false);  // Selects A1:B2
            worksheet.SelectRange(2, 2, 2, 2, false);  // Adds C3:D4 to selection

            try
            {
                // Get selected ranges
                ArrayList ranges = worksheet.GetSelectedRanges();

                Console.WriteLine("Selected Ranges:");
                foreach (Aspose.Cells.Range range in ranges)
                {
                    Console.WriteLine(range.Address);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSelectedRanges method: {ex.Message}");
            }

            workbook.Save("MethodGetSelectedRangesDemo.xlsx");
        }
    }
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


