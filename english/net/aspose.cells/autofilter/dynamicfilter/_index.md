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
public static void Method_DynamicFilterType_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Date&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells[&quot;A3&quot;].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells[&quot;A4&quot;].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells[&quot;A5&quot;].PutValue(new DateTime(2023, 4, 1));
            worksheet.Cells[&quot;A6&quot;].PutValue(new DateTime(2023, 5, 1));

            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Value&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(10);
            worksheet.Cells[&quot;B3&quot;].PutValue(20);
            worksheet.Cells[&quot;B4&quot;].PutValue(30);
            worksheet.Cells[&quot;B5&quot;].PutValue(40);
            worksheet.Cells[&quot;B6&quot;].PutValue(50);

            // Apply auto filter to the worksheet
            worksheet.AutoFilter.SetRange(0, 0, 5);

            // Apply a dynamic filter to show only dates in March
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

            // Save the workbook
            workbook.Save(&quot;DynamicFilterTypeExample.xlsx&quot;);
            workbook.Save(&quot;DynamicFilterTypeExample.pdf&quot;);

            // Output the results
            Console.WriteLine(&quot;Dynamic filter applied to show only dates in March.&quot;);
        }
```

### See Also

* enum [DynamicFilterType](../../dynamicfiltertype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


