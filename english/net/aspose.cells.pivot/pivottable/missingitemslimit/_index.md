---
title: PivotTable.MissingItemsLimit
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them
type: docs
url: /net/aspose.cells.pivot/pivottable/missingitemslimit/
---
## PivotTable.MissingItemsLimit property

Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.

```csharp
[Obsolete("Use PivotCache.MissingItemsLimit propery  instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotMissingItemLimitType MissingItemsLimit { get; set; }
```

### Remarks

NOTE: This property is now obsolete. Instead, please use PivotCache.MissingItemsLimit propery instead . This method will be removed 12 months later since September 2026. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyMissingItemsLimitDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sample data
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 30;

            // Create pivot table and get the instance
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:B4", "E3");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Configure pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value
            
            // Demonstrate MissingItemsLimit property
            pivotTable.MissingItemsLimit = PivotMissingItemLimitType.Max;
            
            // Refresh data
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            workbook.Save("PivotTableMissingItemsLimitDemo.xlsx");
        }
    }
}
```

### See Also

* enum [PivotMissingItemLimitType](../../pivotmissingitemlimittype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


