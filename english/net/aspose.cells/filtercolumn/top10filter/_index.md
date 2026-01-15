---
title: FilterColumn.Top10Filter
second_title: Aspose.Cells for .NET API Reference
description: FilterColumn property. Gets Top10Filter for filtering data by rank of data
type: docs
url: /net/aspose.cells/filtercolumn/top10filter/
---
## FilterColumn.Top10Filter property

Gets [`Top10Filter`](../../top10filter/) for filtering data by rank of data.

```csharp
public Top10Filter Top10Filter { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyTop10FilterDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook and get the first worksheet
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Populate some sample data
                sheet.Cells["A1"].PutValue("Values");
                sheet.Cells["A2"].PutValue(10);
                sheet.Cells["A3"].PutValue(20);
                sheet.Cells["A4"].PutValue(30);
                sheet.Cells["A5"].PutValue(40);

                // Apply an AutoFilter to the data range
                sheet.AutoFilter.Range = "A1:A5";

                // Get the first filter column (column index 0)
                FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];

                // Display the current Filter object (may be null)
                Console.WriteLine("Current Filter object type: " +
                    (filterColumn.Filter != null ? filterColumn.Filter.GetType().FullName : "null"));

                // Check whether the filter applied is a Top10Filter
                if (filterColumn.Filter != null && filterColumn.Filter.GetType().Name == "Top10Filter")
                {
                    Console.WriteLine("The filter column contains a Top10Filter.");
                }
                else
                {
                    Console.WriteLine("No Top10Filter is applied to this column.");
                }

                // Save the workbook (optional)
                workbook.Save("Top10FilterDemo.xlsx");
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

* class [Top10Filter](../../top10filter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


