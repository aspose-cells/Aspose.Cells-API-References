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
| [DynamicFilterType](../../aspose.cells/dynamicfilter/dynamicfiltertype/) { get; set; } | Gets and sets the type of this dynamic filter. |
| [MaxValue](../../aspose.cells/dynamicfilter/maxvalue/) { get; set; } | Gets and sets the dynamic filter max value. |
| [Value](../../aspose.cells/dynamicfilter/value/) { get; set; } | Gets and sets the dynamic filter value. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Create a workbook and a worksheet (optional for context)
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Name = "DemoSheet";

                // Populate some sample numeric data
                worksheet.Cells["A1"].PutValue("Numbers");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["A5"].PutValue(40);
                worksheet.Cells["A6"].PutValue(50);

                // Define an autofilter range
                worksheet.AutoFilter.Range = "A1:A6";

                // Apply a dynamic filter (AboveAverage) to the first column
                worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.AboveAverage);

                // Retrieve the DynamicFilter instance created by the AutoFilter
                DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

                // Set additional properties if desired
                filter.Value = 25;      // Example custom value
                filter.MaxValue = 45;   // Example max value

                // Display the set properties
                Console.WriteLine($"DynamicFilterType: {filter.DynamicFilterType}");
                Console.WriteLine($"Value: {filter.Value}");
                Console.WriteLine($"MaxValue: {filter.MaxValue}");

                // Refresh the filter to apply changes
                worksheet.AutoFilter.Refresh();

                // Save the workbook (the filtered data will be saved)
                workbook.Save("DynamicFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DynamicFilter: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


