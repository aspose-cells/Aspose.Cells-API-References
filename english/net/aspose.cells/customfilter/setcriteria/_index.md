---
title: CustomFilter.SetCriteria
second_title: Aspose.Cells for .NET API Reference
description: CustomFilter method. Sets the filter criteria
type: docs
url: /net/aspose.cells/customfilter/setcriteria/
---
## CustomFilter.SetCriteria method

Sets the filter criteria.

```csharp
public void SetCriteria(FilterOperatorType filterOperator, object criteria)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filterOperator | FilterOperatorType | filter operator type |
| criteria | Object | filter criteria value |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterMethodSetCriteriaWithFilterOperatorTObjectDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);

            // Apply auto filter
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;

            try
            {
                // Apply a custom filter to get a CustomFilter instance
                filter.Custom(0, FilterOperatorType.GreaterThan, 25);

                // Get the first custom filter from the filter collection
                CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];

                // Set criteria using the SetCriteria method
                customFilter.SetCriteria(FilterOperatorType.GreaterThan, 25);

                // Display the set criteria
                Console.WriteLine("Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Criteria Value: " + customFilter.Criteria);

                // Save the workbook
                workbook.Save("SetCriteriaDemo.xlsx");
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

* enum [FilterOperatorType](../../filteroperatortype/)
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


