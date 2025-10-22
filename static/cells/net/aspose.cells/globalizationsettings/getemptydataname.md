##GlobalizationSettings.GetEmptyDataName
GlobalizationSettings method. Gets the name of blank label in the PivotTable
## GlobalizationSettings.GetEmptyDataName method
Gets the name of "(blank)" label in the PivotTable.
```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfEmptyData() method instead.")]
public virtual string GetEmptyDataName()
```
### Return Value
The name of empty data
### Remarks
NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class GlobalizationSettingsMethodGetEmptyDataNameDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data with empty cells
object[,] data = new object[,]
{
{"Category", "Sales"},
{"Electronics", 1500},
{null, 2000}, // Empty category cell
{"Furniture", 3000}
};
// Populate worksheet
int rows = data.GetLength(0);
int cols = data.GetLength(1);
for (int i = 0; i < rows; i++)
{
for (int j = 0; j < cols; j++)
{
worksheet.Cells[i, j].PutValue(data[i, j]);
}
}
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Corrected: Remove invalid assignment of AddFieldToArea result
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Configure custom globalization settings
workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
try
{
// Refresh pivot table to apply localization
pivotTable.RefreshData();
pivotTable.CalculateData();
// Demonstrate direct method call
string emptyName = workbook.Settings.GlobalizationSettings.GetEmptyDataName();
Console.WriteLine($"Custom empty data label: {emptyName}");
workbook.Save("GlobalizationGetEmptyDataNameDemo.xlsx");
Console.WriteLine("Demo executed successfully. Check output file.");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
private class CustomGlobalizationSettings : GlobalizationSettings
{
[Obsolete]
public override string GetEmptyDataName()
{
return "[[UNSPECIFIED]]"; // Custom empty data label
}
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
