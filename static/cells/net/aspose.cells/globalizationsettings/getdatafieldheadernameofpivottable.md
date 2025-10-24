##GlobalizationSettings.GetDataFieldHeaderNameOfPivotTable
GlobalizationSettings method. Gets the the name of the value area field header in the PivotTable
## GlobalizationSettings.GetDataFieldHeaderNameOfPivotTable method
Gets the the name of the value area field header in the PivotTable.
```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfDataFieldHeader() method instead.")]
public virtual string GetDataFieldHeaderNameOfPivotTable()
```
### Return Value
The name of data field header name
### Remarks
NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class GlobalizationSettingsMethodGetDataFieldHeaderNameOfPivotTableDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for PivotTable
worksheet.Cells["A1"].Value = "Category";
worksheet.Cells["B1"].Value = "Value";
worksheet.Cells["A2"].Value = "A";
worksheet.Cells["B2"].Value = 100;
worksheet.Cells["A3"].Value = "B";
worksheet.Cells["B3"].Value = 200;
// Set custom globalization settings
workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
try
{
// Create PivotTable and configure fields
int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:B3", "D1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category as row
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);  // Value as data
// Refresh PivotTable to apply localization changes
pivotTable.RefreshData();
pivotTable.CalculateData();
Console.WriteLine("PivotTable created with custom data field header name.");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
// Save the modified workbook
workbook.Save("GlobalizationSettingsMethodDemo.xlsx");
}
}
// Custom GlobalizationSettings implementation
public class CustomGlobalizationSettings : GlobalizationSettings
{
public override string GetDataFieldHeaderNameOfPivotTable()
{
return "Custom Values";
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
