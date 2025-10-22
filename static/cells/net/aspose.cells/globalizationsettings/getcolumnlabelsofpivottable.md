##GlobalizationSettings.GetColumnLabelsOfPivotTable
GlobalizationSettings method. Gets the name of Column Labels label in the PivotTable
## GlobalizationSettings.GetColumnLabelsOfPivotTable method
Gets the name of "Column Labels" label in the PivotTable.
```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfColumnLabels() method instead.")]
public virtual string GetColumnLabelsOfPivotTable()
```
### Return Value
The name of column labels
### Remarks
NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class GlobalizationSettingsMethodGetColumnLabelsOfPivotTableDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data for PivotTable
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["B1"].Value = "Region";
worksheet.Cells["C1"].Value = "Sales";
worksheet.Cells["A2"].Value = "Bike";
worksheet.Cells["B2"].Value = "North";
worksheet.Cells["C2"].Value = 10000;
worksheet.Cells["A3"].Value = "Bike";
worksheet.Cells["B3"].Value = "South";
worksheet.Cells["C3"].Value = 8000;
worksheet.Cells["A4"].Value = "Car";
worksheet.Cells["B4"].Value = "North";
worksheet.Cells["C4"].Value = 25000;
// Create a PivotTable and get reference
int pivotTableIndex = worksheet.PivotTables.Add("PivotTable", "A1:C4", "E5");
PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region
pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales
// Apply custom globalization settings to override column labels
workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
try
{
// Refresh and calculate PivotTable to apply settings
pivotTable.RefreshData();
pivotTable.CalculateData();
Console.WriteLine("GetColumnLabelsOfPivotTable method executed successfully. Check 'output.xlsx'.");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
// Save the workbook
workbook.Save("output.xlsx");
}
}
// Custom GlobalizationSettings implementation to override column labels
public class CustomGlobalizationSettings : GlobalizationSettings
{
public override string GetColumnLabelsOfPivotTable()
{
// Return custom label for PivotTable column headers
return "Sales Regions";
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
