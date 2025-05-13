---
title: AutoFilter.DynamicFilter
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Adds a dynamic filter
type: docs
url: /net/aspose.cells/autofilter/dynamicfilter/
---
## AutoFilter.DynamicFilter method

Adds a dynamic filter.

```csharp
public void DynamicFilter(int fieldIndex, DynamicFilterType dynamicFilterType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| dynamicFilterType | DynamicFilterType | Dynamic filter type. |

### Examples

```csharp
// Called: worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);
public static void AutoFilter_Method_DynamicFilter()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 1));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 5, 1));

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["B6"].PutValue(50);

            // Apply auto filter to the worksheet
            worksheet.AutoFilter.SetRange(0, 0, 5);

            // Apply a dynamic filter to show only dates in March
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

            // Save the workbook
            workbook.Save("DynamicFilterTypeExample.xlsx");
            workbook.Save("DynamicFilterTypeExample.pdf");

            // Output the results
            Console.WriteLine("Dynamic filter applied to show only dates in March.");
        }
```

### See Also

* enum [DynamicFilterType](../../dynamicfiltertype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


