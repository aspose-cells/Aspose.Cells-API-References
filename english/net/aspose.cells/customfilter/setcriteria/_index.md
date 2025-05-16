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
namespace AsposeCellsExamples.CustomFilterMethodSetCriteriaWithFilterOperatorTypeObjectDemo
{
    using Aspose.Cells;
    using System;

    public class CustomFilterMethodSetCriteriaWithFilterOperatorTypeObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate test data
            worksheet.Cells["A1"].PutValue("Numbers");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(150);
            worksheet.Cells["A5"].PutValue(300);
            worksheet.Cells["A6"].PutValue(50);

            // Enable auto filtering
            worksheet.AutoFilter.Range = "A1:A6";

            try
            {
                // Apply custom filter to first column (index 0)
                worksheet.AutoFilter.Custom(0, FilterOperatorType.GreaterThan, 150);
                worksheet.AutoFilter.Refresh();

                Console.WriteLine("Filter applied: Show values greater than 150");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error applying filter: {ex.Message}");
            }

            workbook.Save("CustomFilterSetCriteriaExample.xlsx");
        }
    }
}
```

### See Also

* enum [FilterOperatorType](../../filteroperatortype/)
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


