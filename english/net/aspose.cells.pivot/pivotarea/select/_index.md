---
title: PivotArea.Select
second_title: Aspose.Cells for .NET API Reference
description: PivotArea method. Select the area with filters
type: docs
url: /net/aspose.cells.pivot/pivotarea/select/
---
## PivotArea.Select method

Select the area with filters.

```csharp
public void Select(PivotFieldType axisType, int fieldPosition, 
    PivotTableSelectionType selectionType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| axisType | PivotFieldType | The region of the PivotTable to which this rule applies. |
| fieldPosition | Int32 | Position of the field within the axis to which this rule applies. |
| selectionType | PivotTableSelectionType | Specifies what can be selected in a PivotTable during a structured selection. |

### Examples

```csharp
// Called: pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);
public static void PivotArea_Method_Select()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data for the PivotTable
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(250);

            // Create a PivotTable
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Create a PivotArea and set its properties
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.OnlyData = false;
            pivotArea.OnlyLabel = true;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.IsOutline = false;

            // Select the area with specific selection type
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            // Save the workbook
            workbook.Save("PivotTableSelectionTypeExample.xlsx");

            return;
        }
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* enum [PivotTableSelectionType](../../pivottableselectiontype/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


