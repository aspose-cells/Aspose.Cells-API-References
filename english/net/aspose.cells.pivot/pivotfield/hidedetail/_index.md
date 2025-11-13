---
title: PivotField.HideDetail
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Sets whether the detail of all PivotItems in a pivot field are hidden. That is collapse/expand this field
type: docs
url: /net/aspose.cells.pivot/pivotfield/hidedetail/
---
## PivotField.HideDetail method

Sets whether the detail of all PivotItems in a pivot field are hidden. That is collapse/expand this field.

```csharp
public void HideDetail(bool isHiddenDetail)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isHiddenDetail | Boolean | Whether hide the detail of the pivot field. |

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideDetailWithBooleanDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Add sample data
            sheet.Cells["A1"].PutValue("Country");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Japan");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("USA");
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["A4"].PutValue("UK");
            sheet.Cells["B4"].PutValue(3000);

            // Create pivot table
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Add row field
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            
            // Add data field
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Hide details for the first row field
            PivotField rowField = pivotTable.RowFields[0];
            rowField.HideDetail(true);
            
            // Refresh and calculate pivot table
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Save the workbook
            workbook.Save("HideDetailDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


