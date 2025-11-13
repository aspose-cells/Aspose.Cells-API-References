---
title: Top10Filter.Criteria
second_title: Aspose.Cells for .NET API Reference
description: Top10Filter property. The actual cell value in the range which is used to perform the comparison for this filter. This is the cache value during the refresh process
type: docs
url: /net/aspose.cells/top10filter/criteria/
---
## Top10Filter.Criteria property

The actual cell value in the range which is used to perform the comparison for this filter. This is the cache value during the refresh process.

```csharp
[Obsolete("Ignore this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public object Criteria { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead,please ignore this property. This property will be removed 12 months later since October 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class Top10FilterPropertyCriteriaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            for (int i = 0; i < 20; i++)
            {
                worksheet.Cells[i, 0].PutValue(20 - i);
            }
            
            worksheet.AutoFilter.Range = "A1:A20";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // Fix: Access Filter property and cast to Top10Filter
            Top10Filter filter = (Top10Filter)worksheet.AutoFilter.FilterColumns[0].Filter;
            Console.WriteLine("Current Criteria value: " + filter.Criteria);
            
            filter.Criteria = 14;
            
            worksheet.AutoFilter.Refresh();
            
            workbook.Save("Top10FilterCriteriaDemo.xlsx");
        }
    }
}
```

### See Also

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


