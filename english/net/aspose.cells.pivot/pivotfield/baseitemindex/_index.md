---
title: PivotField.BaseItemIndex
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields
type: docs
url: /net/aspose.cells.pivot/pivotfield/baseitemindex/
---
## PivotField.BaseItemIndex property

Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields.

```csharp
[Obsolete("Use PivotField.ShowValuesSetting.BaseItemIndex property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int BaseItemIndex { get; set; }
```

### Remarks

NOTE: This property is now obsolete. Instead, please use PivotField.ShowValuesSetting.BaseItemIndex property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: rowField.BaseItemIndex = 0;
public static void PivotField_Property_BaseItemIndex()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Add some data to the worksheet
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Add a pivot table to the worksheet
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "year");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "amount");

            // Set pivot table style
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Access the row field
            PivotField rowField = pivotTable.RowFields[0];

            // Set properties of the PivotField
            rowField.DisplayName = "Custom Display Name";
            rowField.IsAutoSubtotals = false;
            rowField.DragToColumn = true;
            rowField.DragToHide = true;
            rowField.DragToRow = true;
            rowField.DragToPage = true;
            rowField.DragToData = true;
            rowField.IsMultipleItemSelectionAllowed = true;
            rowField.IsRepeatItemLabels = true;
            rowField.IsIncludeNewItemsInFilter = true;
            rowField.IsInsertPageBreaksBetweenItems = true;
            rowField.ShowAllItems = true;
            rowField.NonAutoSortDefault = true;
            rowField.IsAutoSort = true;
            rowField.IsAscendSort = true;
            rowField.AutoSortField = -1;
            rowField.IsAutoShow = true;
            rowField.IsAscendShow = true;
            rowField.AutoShowCount = 5;
            rowField.AutoShowField = -1;
            rowField.Function = ConsolidationFunction.Sum;
            rowField.DataDisplayFormat = PivotFieldDataDisplayFormat.PercentageOfTotal;
            rowField.BaseFieldIndex = 0;
            rowField.BaseItemPosition = PivotItemPosition.Next;
            rowField.BaseItemIndex = 0;
            rowField.CurrentPageItem = 1;
            rowField.Number = 0;
            rowField.InsertBlankRow = true;
            rowField.ShowSubtotalAtTop = true;
            rowField.ShowInOutlineForm = true;
            rowField.NumberFormat = "0.00";
            rowField.ShowCompact = true;

            // Refresh and calculate the pivot table data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Save the workbook
            workbook.Save("PivotFieldExample.xlsx");
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


