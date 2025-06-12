---
title: SubtotalSetting.GroupBy
second_title: Aspose.Cells for .NET API Reference
description: SubtotalSetting property. The field to group by as a zerobased integer offset
type: docs
url: /net/aspose.cells/subtotalsetting/groupby/
---
## SubtotalSetting.GroupBy property

The field to group by, as a zero-based integer offset

```csharp
public int GroupBy { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertyGroupByDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sample data
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Create subtotal setting by retrieving existing settings
            CellArea area = CellArea.CreateCellArea("A1", "B5");
            SubtotalSetting subtotal = worksheet.Cells.RetrieveSubtotalSetting(area);
            
            // Configure subtotal settings through the proper API
            // Note: GroupBy and SubtotalFunction are read from the setting, not set directly
            // We apply subtotals directly to the worksheet
            worksheet.Cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 1 });

            // Save the workbook
            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### See Also

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


