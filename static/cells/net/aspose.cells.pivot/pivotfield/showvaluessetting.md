##PivotField.ShowValuesSetting
PivotField property. Gets the settings of showing values as when the ShowDataAs calculation is in use
## PivotField.ShowValuesSetting property
Gets the settings of showing values as when the ShowDataAs calculation is in use.
```csharp
public PivotShowValuesSetting ShowValuesSetting { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyShowValuesSettingDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Product";
cells["B1"].Value = "Sales";
cells["A2"].Value = "Apple";
cells["B2"].Value = 1000;
cells["A3"].Value = "Orange";
cells["B3"].Value = 2000;
cells["A4"].Value = "Banana";
cells["B4"].Value = 3000;
cells["A5"].Value = "Apple";
cells["B5"].Value = 1500;
cells["A6"].Value = "Orange";
cells["B6"].Value = 2500;
cells["A7"].Value = "Banana";
cells["B7"].Value = 3500;
// Create pivot table
PivotTableCollection pivotTables = sheet.PivotTables;
int index = pivotTables.Add("A1:B7", "C10", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add row and data fields
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
PivotField dataField = pivotTable.DataFields[0];
// Configure ShowValuesSetting to display as percentage of total
dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
// Calculate and refresh pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotFieldShowValuesSettingDemo.xlsx");
}
}
}
```
### See Also
* class [PivotShowValuesSetting](../../pivotshowvaluessetting/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
