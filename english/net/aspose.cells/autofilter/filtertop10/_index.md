---
title: AutoFilter.FilterTop10
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Filter the top 10 items in the list
type: docs
url: /net/aspose.cells/autofilter/filtertop10/
---
## AutoFilter.FilterTop10 method

Filter the top 10 items in the list

```csharp
public void FilterTop10(int fieldIndex, bool isTop, bool isPercent, int itemCount)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| isTop | Boolean | Indicates whether filter from top or bottom |
| isPercent | Boolean | Indicates whether the items is percent or count |
| itemCount | Int32 | The item count |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodFilterTop10WithInt32BooleanBooleanInt32Demo
    {
        public static void Run()
        {
            // Create a workbook with sample data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data (5 rows x 3 columns with numeric values)
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Numbers");
            cells["A2"].PutValue(50);
            cells["A3"].PutValue(30);
            cells["A4"].PutValue(80);
            cells["A5"].PutValue(20);
            cells["A6"].PutValue(90);

            // Set autofilter range
            worksheet.AutoFilter.Range = "A1:A6";

            // Apply top 10 filter (showing top 2 items)
            worksheet.AutoFilter.FilterTop10(0, true, false, 2);

            // Refresh the filter
            worksheet.AutoFilter.Refresh();

            // Save the workbook
            workbook.Save("FilterTop10Demo.xlsx");
        }
    }
}
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


