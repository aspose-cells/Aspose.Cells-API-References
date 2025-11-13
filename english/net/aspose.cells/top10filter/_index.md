---
title: Class Top10Filter
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Top10Filter class. Represents the top N percent or number of items to filter by
type: docs
url: /net/aspose.cells/top10filter/
---
## Top10Filter class

Represents the top N (percent or number of items) to filter by.

```csharp
public class Top10Filter
```

## Properties

| Name | Description |
| --- | --- |
| [Criteria](../../aspose.cells/top10filter/criteria/) { get; set; } | (**Obsolete.**) The actual cell value in the range which is used to perform the comparison for this filter. This is the cache value during the refresh process. |
| [IsPercent](../../aspose.cells/top10filter/ispercent/) { get; set; } | Indicates whether or not to filter by percent value of the column |
| [IsTop](../../aspose.cells/top10filter/istop/) { get; set; } | Indicates whether or not to filter by top order |
| [Items](../../aspose.cells/top10filter/items/) { get; set; } | Gets and sets top or bottom value to use as the filter criteria. |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTop10FilterDemo
    {
        public static void Run()
        {
            // Create a workbook with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data
            worksheet.Cells["B6"].PutValue("Value");
            for (int i = 7; i <= 16; i++)
            {
                worksheet.Cells["B" + i].PutValue(20 - i);
                worksheet.Cells["C" + i].PutValue("Item " + (i-6));
            }
            
            // Apply auto filter and top 10 filter
            worksheet.AutoFilter.Range = "B6:C16";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5); // Filter top 5 values in column B
            
            // Get the Top10Filter and verify its properties
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop);
            Console.WriteLine("IsPercent: " + filter.IsPercent);
            Console.WriteLine("Items: " + filter.Items);
            
            // Refresh the filter and check hidden rows
            worksheet.AutoFilter.Refresh();
            for (int i = 6; i <= 16; i++)
            {
                Console.WriteLine($"Row {i} hidden: {worksheet.Cells.IsRowHidden(i)}");
            }
            
            // Save the workbook
            workbook.Save("Top10FilterDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


