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
[C#]

using Aspose.Cells;
using System;

namespace Demos
{
    public class CustomFilterDemo
    {
        public static void RunDemo()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            sheet.Cells["A1"].PutValue("Apple");
            sheet.Cells["A2"].PutValue("Banana");
            sheet.Cells["A3"].PutValue("Cherry");
            sheet.Cells["A4"].PutValue("Date");
            sheet.Cells["A5"].PutValue("Elderberry");

            // Create a CustomFilterCollection
            CustomFilterCollection customFilters = new CustomFilterCollection();

            //// Create a CustomFilter for filtering fruits that start with 'A' or 'B'
            //CustomFilter filter1 = new CustomFilter()
            //{
            //    FilterOperatorType = FilterOperatorType.Equal,
            //    Criteria = "Apple"
            //};

            //CustomFilter filter2 = new CustomFilter()
            //{
            //    FilterOperatorType = FilterOperatorType.Equal,
            //    Criteria = "Banana"
            //};

            //// Add filters to the collection with "And" relationship
            //customFilters.And = true;

            //// Set criteria for the filters
            //customFilters.Append(filter1);
            //customFilters.Append(filter2);

            // Apply the custom filters to the worksheet
            // Assuming we have a method to apply filters (not defined in the provided code)
            ApplyCustomFilters(sheet, customFilters);

            // Save the workbook
            workbook.Save("CustomFilterDemo.xlsx");
            workbook.Save("CustomFilterDemo.pdf");
        }

        private static void ApplyCustomFilters(Worksheet sheet, CustomFilterCollection filters)
        {
            // This method would contain logic to apply the filters to the worksheet.
            // The implementation of this method is not provided in the original reflection.
            // For demonstration purposes, we will just print the filters.
            Console.WriteLine("Applying custom filters:");
            foreach (var filter in filters)
            {
                Console.WriteLine($"Filter: {filter.FilterOperatorType}, Criteria: {filter.Criteria}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


