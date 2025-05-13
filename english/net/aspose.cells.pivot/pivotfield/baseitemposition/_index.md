---
title: PivotField.BaseItemPosition
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for readif you need to set PivotItemPosition.Custom please set PivotField.BaseItemIndex attribute
type: docs
url: /net/aspose.cells.pivot/pivotfield/baseitemposition/
---
## PivotField.BaseItemPosition property

Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.

```csharp
[Obsolete("Use PivotField.ShowValuesSetting.BaseItemPositionType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotItemPosition BaseItemPosition { get; set; }
```

### Remarks

NOTE: This property is now obsolete. Instead, please use PivotField.ShowValuesSetting.BaseItemPositionType property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: rowField.BaseItemPosition = PivotItemPosition.Next;
public static void PivotField_Property_BaseItemPosition()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2021;
            worksheet.Cells[3, 1].Value = 2022;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // Add a pivot table to the worksheet
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Access the row field
            PivotField rowField = pivotTable.RowFields[0];

            // Set the base item position for custom calculation
            rowField.BaseItemPosition = PivotItemPosition.Next;

            // Refresh and calculate the pivot table data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Save the workbook
            workbook.Save("PivotItemPositionExample.xlsx");
        }
```

### See Also

* enum [PivotItemPosition](../../pivotitemposition/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


