---
title: Class CustomFilter
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.CustomFilter class. Represents the custom filter
type: docs
url: /net/aspose.cells/customfilter/
---
## CustomFilter class

Represents the custom filter.

```csharp
public class CustomFilter
```

## Properties

| Name | Description |
| --- | --- |
| [Criteria](../../aspose.cells/customfilter/criteria/) { get; set; } | Gets and sets the criteria. |
| [FilterOperatorType](../../aspose.cells/customfilter/filteroperatortype/) { get; set; } | Gets and sets the filter operator type. |

## Methods

| Name | Description |
| --- | --- |
| [SetCriteria](../../aspose.cells/customfilter/setcriteria/)(FilterOperatorType, object) | Sets the filter criteria. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCustomFilterDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add sample data to the worksheet
                worksheet.Cells["A1"].PutValue("Values");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["A5"].PutValue(40);

                // Apply auto filter to the range
                worksheet.AutoFilter.Range = "A1:A5";
                AutoFilter filter = worksheet.AutoFilter;

                // Apply a custom filter to get a CustomFilter instance
                filter.Custom(0, FilterOperatorType.GreaterThan, 25);

                // Get the first custom filter from the filter collection
                CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];

                // Display the filter properties
                Console.WriteLine("Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Criteria Value: " + customFilter.Criteria);

                // Modify the filter criteria using the SetCriteria method
                customFilter.SetCriteria(FilterOperatorType.LessThan, 35);

                // Display the updated filter properties
                Console.WriteLine("Updated Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Updated Criteria Value: " + customFilter.Criteria);

                // Save the workbook
                workbook.Save("CustomFilterDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with CustomFilter: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


