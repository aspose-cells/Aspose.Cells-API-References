---
title: Worksheet.Filter
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Filters the range
type: docs
url: /net/aspose.cells/worksheet/filter/
---
## Worksheet.Filter method

Filters the range.

```csharp
public void Filter(CellArea ca)
```

| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;

    public class WorksheetMethodFilterWithCellAreaDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate some sample data (including a header row)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            try
            {
                // Define the range to which the filter will be applied
                CellArea filterArea = new CellArea
                {
                    StartRow = 0,      // Row 1 (zero‑based)
                    StartColumn = 0,   // Column A
                    EndRow = 4,        // Row 5
                    EndColumn = 1      // Column B
                };

                // Apply an auto‑filter to the defined area
                worksheet.Filter(filterArea);

                // Save the workbook to verify the filter was set
                workbook.Save("WorksheetFilterWithCellAreaDemo.xlsx");

                Console.WriteLine("Filter applied successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error applying filter: {ex.Message}");
            }
        }
    }
}
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


