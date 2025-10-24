##GlobalizationSettings.GetProtectionNameOfPivotTable
GlobalizationSettings method. Gets the protection name in the PivotTable
## GlobalizationSettings.GetProtectionNameOfPivotTable method
Gets the protection name in the PivotTable.
```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfProtectedName(string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetProtectionNameOfPivotTable()
```
### Return Value
The protection name of PivotTable
### Remarks
NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetTextOfProtectedName(string) method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class GlobalizationSettingsMethodGetProtectionNameOfPivotTableDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create standard globalization settings
GlobalizationSettings standardSettings = new GlobalizationSettings();
// Create custom globalization settings
GlobalizationSettings customSettings = new CustomGlobalizationSettings();
workbook.Settings.GlobalizationSettings = customSettings;
try
{
// Get default protection name
string defaultName = standardSettings.GetProtectionNameOfPivotTable();
Console.WriteLine($"Default protection name: {defaultName}");
// Get customized protection name
string customName = customSettings.GetProtectionNameOfPivotTable();
Console.WriteLine($"Custom protection name: {customName}");
// Create pivot table to demonstrate settings application
worksheet.Cells["A1"].Value = "Data";
worksheet.Cells["A2"].Value = 1;
worksheet.Cells["A3"].Value = 2;
worksheet.Cells["A4"].Value = 3;
int pivotIndex = worksheet.PivotTables.Add("A1", "A1:A4", "PivotTable");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Protection would typically be applied here using the retrieved name
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetProtectionNameOfPivotTable: {ex.Message}");
}
workbook.Save("GlobalizationSettingsMethodGetProtectionNameOfPivotTableDemo.xlsx");
}
}
public class CustomGlobalizationSettings : GlobalizationSettings
{
public new string GetProtectionNameOfPivotTable()
{
return "CustomPivotProtection";
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
