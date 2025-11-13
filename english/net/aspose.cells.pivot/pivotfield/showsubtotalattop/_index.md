---
title: PivotField.ShowSubtotalAtTop
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether to display subtotals at the top or bottom of items when ShowInOutlineForm is true then
type: docs
url: /net/aspose.cells.pivot/pivotfield/showsubtotalattop/
---
## PivotField.ShowSubtotalAtTop property

Indicates whether to display subtotals at the top or bottom of items when ShowInOutlineForm is true, then

```csharp
public bool ShowSubtotalAtTop { get; set; }
```

### Remarks

Only works when ShowInOutlineForm is true.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowSubtotalAtTopDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bikes";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Bikes";
            worksheet.Cells["B3"].Value = 1500;
            worksheet.Cells["A4"].Value = "Cars";
            worksheet.Cells["B4"].Value = 2000;
            worksheet.Cells["A5"].Value = "Cars";
            worksheet.Cells["B5"].Value = 2500;

            // Create pivot table
            int index = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Add row field and configure subtotal position
            PivotField rowField = pivotTable.RowFields[pivotTable.AddFieldToArea(PivotFieldType.Row, "Product")];
            rowField.ShowSubtotalAtTop = true; // Demonstrate the property
            rowField.IsAutoSubtotals = true;

            // Add data field
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Save the workbook
            workbook.Save("PivotFieldShowSubtotalAtTopDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


