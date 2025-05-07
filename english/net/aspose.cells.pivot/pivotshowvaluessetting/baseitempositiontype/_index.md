---
title: PivotShowValuesSetting.BaseItemPositionType
second_title: Aspose.Cells for .NET API Reference
description: PivotShowValuesSetting property. Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for readif you need to set PivotItemPosition.Custom please set PivotField.BaseItemIndex attribute
type: docs
url: /net/aspose.cells.pivot/pivotshowvaluessetting/baseitempositiontype/
---
## PivotShowValuesSetting.BaseItemPositionType property

Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.

```csharp
public PivotItemPositionType BaseItemPositionType { get; set; }
```

### Examples

```csharp
// Called: showValuesSetting.BaseItemPositionType = PivotItemPositionType.Next;
public static void Property_BaseItemPositionType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[0, 0].Value = "Product";
            worksheet.Cells[0, 1].Value = "Sales";
            worksheet.Cells[1, 0].Value = "A";
            worksheet.Cells[1, 1].Value = 100;
            worksheet.Cells[2, 0].Value = "B";
            worksheet.Cells[2, 1].Value = 150;
            worksheet.Cells[3, 0].Value = "C";
            worksheet.Cells[3, 1].Value = 200;

            // Add a pivot table to the worksheet
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Access the data field
            PivotField dataField = pivotTable.DataFields[0];

            // Access the ShowValuesSetting property
            PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

            // Set properties of PivotShowValuesSetting
            showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            showValuesSetting.BaseFieldIndex = 0; // Base field index
            showValuesSetting.BaseItemPositionType = PivotItemPositionType.Next;
            showValuesSetting.BaseItemIndex = 1; // Base item index

            // Refresh and calculate the pivot table data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Save the workbook
            workbook.Save("PivotShowValuesSettingExample.xlsx");

            return;
        }
```

### See Also

* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


