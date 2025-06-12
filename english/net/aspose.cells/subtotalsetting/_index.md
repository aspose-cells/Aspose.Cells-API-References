---
title: Class SubtotalSetting
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.SubtotalSetting class. Represents the setting of the subtotal 
type: docs
url: /net/aspose.cells/subtotalsetting/
---
## SubtotalSetting class

Represents the setting of the subtotal .

```csharp
public class SubtotalSetting
```

## Properties

| Name | Description |
| --- | --- |
| [GroupBy](../../aspose.cells/subtotalsetting/groupby/) { get; } | The field to group by, as a zero-based integer offset |
| [SubtotalFunction](../../aspose.cells/subtotalsetting/subtotalfunction/) { get; } | The subtotal function. |
| [SummaryBelowData](../../aspose.cells/subtotalsetting/summarybelowdata/) { get; } | Indicates whether add summary below data. |
| [TotalList](../../aspose.cells/subtotalsetting/totallist/) { get; } | An array of zero-based field offsets, indicating the fields to which the subtotals are added. |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSubtotalSettingDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i % 2 == 0 ? "Group A" : "Group B");
                worksheet.Cells["B" + i].PutValue(i * 100);
            }
            
            // Create cell area for subtotal
            CellArea area = CellArea.CreateCellArea("A1", "B10");
            
            // Apply subtotals directly instead of modifying read-only properties
            worksheet.Cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] {1});
            
            // Save the workbook
            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


