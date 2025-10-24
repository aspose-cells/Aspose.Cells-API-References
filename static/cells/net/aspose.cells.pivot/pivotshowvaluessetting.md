##Class PivotShowValuesSetting
Aspose.Cells.Pivot.PivotShowValuesSetting class. Represents the settings about showing values as when the ShowDataAs calculation is in use
## PivotShowValuesSetting class
Represents the settings about showing values as when the ShowDataAs calculation is in use.
```csharp
public class PivotShowValuesSetting
```
## Properties
| Name | Description |
| --- | --- |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldindex/) { get; set; } | Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
| [BaseItemIndex](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemindex/) { get; set; } | Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. |
| [BaseItemPositionType](../../aspose.cells.pivot/pivotshowvaluessetting/baseitempositiontype/) { get; set; } | Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. |
| [CalculationType](../../aspose.cells.pivot/pivotshowvaluessetting/calculationtype/) { get; set; } | Represents how to show values of a data field in the pivot report. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotShowValuesSettingDemo
{
public static void PivotShowValuesSettingExample()
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
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
