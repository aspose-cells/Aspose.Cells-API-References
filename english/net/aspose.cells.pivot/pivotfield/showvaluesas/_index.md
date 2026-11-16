---
title: PivotField.ShowValuesAs
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Shows values of data field as different display format when the ShowDataAs calculation is in use
type: docs
url: /net/aspose.cells.pivot/pivotfield/showvaluesas/
---
## ShowValuesAs(PivotFieldDataDisplayFormat, int, PivotItemPositionType, int) {#showvaluesas}

Shows values of data field as different display format when the ShowDataAs calculation is in use.

```csharp
[Obsolete("Use PivotField.ShowValuesAs(PivotShowValuesAsType,int int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ShowValuesAs(PivotFieldDataDisplayFormat displayFormat, int baseField, 
    PivotItemPositionType baseItemPositionType, int baseItem)
```

| Parameter | Type | Description |
| --- | --- | --- |
| displayFormat | PivotFieldDataDisplayFormat | The data display format type. |
| baseField | Int32 | The index to the field which ShowDataAs calculation bases on. |
| baseItemPositionType | PivotItemPositionType | The position type of base iteam. |
| baseItem | Int32 | The index to the base item which ShowDataAs calculation bases on. Only works when baseItemPositionType is custom. |

### Remarks

NOTE: This property is now obsolete. Instead, please use PivotField.ShowValuesAs(PivotShowValuesAsType,int,int) method instead. This method will be removed 12 months later since November 2026. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodShowValuesAsWithPivotFieldDataDisplayFormatIntDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[workbook.Worksheets.Add()];
            worksheet.Name = "PivotData";

            // Add sample data
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Quarter");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue(1000);
            
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue(1500);
            
            worksheet.Cells["A4"].PutValue("Furniture");
            worksheet.Cells["B4"].PutValue("Q1");
            worksheet.Cells["C4"].PutValue(800);
            
            worksheet.Cells["A5"].PutValue("Furniture");
            worksheet.Cells["B5"].PutValue("Q2");
            worksheet.Cells["C5"].PutValue(1200);

            // Create pivot table
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=PivotData!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Add row field
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[rowFieldIndex];

            // Add column field
            int columnFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
            PivotField columnField = pivotTable.ColumnFields[columnFieldIndex];

            // Add data field and configure ShowValuesAs
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            dataField.DisplayName = "Sales Diff";
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, columnField.BaseIndex, PivotItemPositionType.Next, 0);

            // Calculate data and save
            pivotTable.CalculateData();
            workbook.Save("PivotTableShowValuesAsDemo.xlsx");
        }
    }
}
```

### See Also

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, int, int) {#showvaluesas_1}

Sets the "Show Values As" calculation for this pivot field.

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, int baseField, int baseItem)
```

| Parameter | Type | Description |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | Type of the "Show Values As" calculation. |
| baseField | Int32 | Index of the base field used for the calculation. |
| baseItem | Int32 | Index of the base item for the calculation. Use [`PreviousPivotItem`](../../pivotshowvaluessetting/previouspivotitem/) (-1) for the preceding item, [`NextPivotItem`](../../pivotshowvaluessetting/nextpivotitem/) (-2) for the succeeding item; non‑negative values denote the ordinal index of a specific pivot item. |

### Remarks

Only for data field.

### See Also

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, string, string) {#showvaluesas_2}

Configures the "Show Values As" calculation for this data field.

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, string baseField, string baseItem)
```

| Parameter | Type | Description |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | The calculation type for Show Values As. |
| baseField | String | The name of the base field used in the calculation. |
| baseItem | String | Caption of a regular pivot item. Also accepts reserved literal keywords: `(previous)` for the previous item, `(next)` for the next item. Pass `null` if the selected calculation type does not require a base item. |

### See Also

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


