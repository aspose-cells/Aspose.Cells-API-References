---
title: DynamicFilter.DynamicFilterType
second_title: Aspose.Cells for .NET API Reference
description: DynamicFilter property. Gets and sets the dynamic filter type
type: docs
url: /net/aspose.cells/dynamicfilter/dynamicfiltertype/
---
## DynamicFilter.DynamicFilterType property

Gets and sets the dynamic filter type.

```csharp
public DynamicFilterType DynamicFilterType { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.DynamicFilterPropertyDynamicFilterTypeDemo
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyDynamicFilterTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate sample data with dates and values
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Amount");
            DateTime baseDate = DateTime.Today;
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[$"A{i + 2}"].PutValue(baseDate.AddMonths(-i));
                worksheet.Cells[$"B{i + 2}"].PutValue(1000 * (i + 1));
            }

            // Apply auto filter to the data range
            worksheet.AutoFilter.Range = "A1:B11";

            // Apply dynamic filter with DynamicFilterType
            Console.WriteLine("Applying DynamicFilterType: LastMonth");
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.LastMonth);

            // Change filter type and reapply
            Console.WriteLine("Applying DynamicFilterType: ThisMonth");
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.ThisMonth);

            workbook.Save("DynamicFilterTypeDemo.xlsx");
        }
    }
}
```

### See Also

* enum [DynamicFilterType](../../dynamicfiltertype/)
* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


