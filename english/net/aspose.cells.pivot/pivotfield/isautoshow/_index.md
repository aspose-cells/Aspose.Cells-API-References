---
title: PivotField.IsAutoShow
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether the specified PivotTable field is automatically shown
type: docs
url: /net/aspose.cells.pivot/pivotfield/isautoshow/
---
## PivotField.IsAutoShow property

Indicates whether the specified PivotTable field is automatically shown.

```csharp
public bool IsAutoShow { get; set; }
```

### Remarks

Only valid for excel 2003.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAutoShowDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Add pivot table
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Add row field
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Add data field and configure IsAutoShow
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            
            // Enable AutoShow and configure settings
            dataField.IsAutoShow = true;
            dataField.AutoShowCount = 2;
            dataField.AutoShowField = 0; // Index of the field to auto show
            dataField.IsAscendShow = true;
            
            // Calculate data
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Output the IsAutoShow property value
            Console.WriteLine("IsAutoShow property value: " + dataField.IsAutoShow);
            
            // Save the workbook
            workbook.Save("PivotFieldPropertyIsAutoShowDemo_out.xlsx");
        }
    }
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


