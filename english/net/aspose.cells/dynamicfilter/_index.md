---
title: Class DynamicFilter
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.DynamicFilter class. Represents the dynamic filter
type: docs
url: /net/aspose.cells/dynamicfilter/
---
## DynamicFilter class

Represents the dynamic filter.

```csharp
public class DynamicFilter
```

## Properties

| Name | Description |
| --- | --- |
| [DynamicFilterType](../../aspose.cells/dynamicfilter/dynamicfiltertype/) { get; set; } | Gets and sets the dynamic filter type. |
| [MaxValue](../../aspose.cells/dynamicfilter/maxvalue/) { get; set; } | Gets and sets the dynamic filter max value. |
| [Value](../../aspose.cells/dynamicfilter/value/) { get; set; } | Gets and sets the dynamic filter value. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    
    public class CellsClassDynamicFilterDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue("2023-01-01");
            worksheet.Cells["A3"].PutValue("2023-02-15");
            worksheet.Cells["A4"].PutValue("2023-03-10");
            worksheet.Cells["A5"].PutValue("2023-04-20");
            
            // Create auto filter
            worksheet.AutoFilter.Range = "A1:A5";
            
            // Apply dynamic filter directly using AutoFilter's method
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.February);
            worksheet.AutoFilter.Refresh();
            
            // Save the result
            workbook.Save("DynamicFilterDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


