---
title: Top10Filter.IsPercent
second_title: Aspose.Cells for .NET API Reference
description: Top10Filter property. Indicates whether or not to filter by percent value of the column
type: docs
url: /net/aspose.cells/top10filter/ispercent/
---
## Top10Filter.IsPercent property

Indicates whether or not to filter by percent value of the column

```csharp
public bool IsPercent { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyIsPercentDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue((i + 1) * (j + 1));
                }
            }

            // Apply top 10 filter (not percent)
            worksheet.AutoFilter.Range = "A1:J10";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // Get the filter and demonstrate IsPercent property
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop);
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output False

            // Apply top 10 percent filter
            worksheet.AutoFilter.FilterTop10(1, true, true, 20);
            filter = worksheet.AutoFilter.FilterColumns[1].Filter as Top10Filter;
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output True
        }
    }
}
```

### See Also

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


