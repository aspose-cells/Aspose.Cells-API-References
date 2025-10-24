##PivotShowValuesSetting.BaseItemIndex
PivotShowValuesSetting property. Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields
## PivotShowValuesSetting.BaseItemIndex property
Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields.
```csharp
public int BaseItemIndex { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotShowValuesSettingPropertyBaseItemIndexDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["A2"].Value = "A";
worksheet.Cells["B2"].Value = 100;
worksheet.Cells["A3"].Value = "B";
worksheet.Cells["B3"].Value = 150;
worksheet.Cells["A4"].Value = "C";
worksheet.Cells["B4"].Value = 200;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E5", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Configure show values settings
PivotField dataField = pivotTable.DataFields[0];
dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOf;
dataField.ShowValuesSetting.BaseFieldIndex = 0;
dataField.ShowValuesSetting.BaseItemIndex = 1; // Using BaseItemIndex property
pivotTable.RefreshData();
pivotTable.CalculateData();
workbook.Save("PivotShowValuesSettingBaseItemIndexDemo.xlsx");
}
}
}
```
### See Also
* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
