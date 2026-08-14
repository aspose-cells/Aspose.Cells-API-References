---
title: PivotField.HideItem
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Sets whether the specific PivotItem in a data field is hidden
type: docs
url: /net/aspose.cells.pivot/pivotfield/hideitem/
---
## HideItem(int, bool) {#hideitem}

Sets whether the specific PivotItem in a data field is hidden.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItem(int index, bool isHidden)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the index of the pivotItem in the pivotField. |
| isHidden | Boolean | whether the specific PivotItem is hidden |

### Remarks

NOTE: This method is now obsolete. Instead, please use PivotField.PivotItems[int].IsHidden property instead . This method will be removed 12 months later since August 2026. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideItemWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Create a workbook with a sample pivot table
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Sample data for pivot table
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("PO-23-05");
            sheet.Cells["A3"].PutValue("PO-23-06");
            sheet.Cells["A4"].PutValue("PO-23-05");
            sheet.Cells["A5"].PutValue("PO-23-07");
            
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(1500);
            sheet.Cells["B5"].PutValue(3000);

            // Create pivot table
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Add row field
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Add data field
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Get the pivot field
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Hide items that are not "PO-23-05"
            for (int i = 0; i < pivotField.ItemCount; i++)
            {
                pivotField.HideItem(i, pivotField.Items[i] != "PO-23-05");
            }
            
            // Calculate pivot table
            pivotTable.CalculateData();
            
            // Save the workbook
            workbook.Save("PivotFieldHideItemDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## HideItem(string, bool) {#hideitem_1}

```csharp
[Obsolete("Use PivotField.PivotItems[string].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItem(string itemValue, bool isHidden)
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


