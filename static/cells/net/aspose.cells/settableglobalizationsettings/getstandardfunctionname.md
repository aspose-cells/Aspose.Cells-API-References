##SettableGlobalizationSettings.GetStandardFunctionName
SettableGlobalizationSettings method. Gets the standard function name according to given locale dependent function name
## SettableGlobalizationSettings.GetStandardFunctionName method
Gets the standard function name according to given locale dependent function name.
```csharp
public override string GetStandardFunctionName(string localName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| localName | String | Locale dependent function name. The locale was specified by the Workbook for which this settings is used. |
### Return Value
Standard(en-US locale) function name.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create custom globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
// Set a local function name mapping
settings.SetStandardFunctionName("LocalSum", "SUM", true);
// Apply the settings to the workbook
workbook.Settings.GlobalizationSettings = settings;
try
{
// Call GetStandardFunctionName with a local function name
string standardName = settings.GetStandardFunctionName("LocalSum");
// Display the result
Console.WriteLine($"Standard function name for 'LocalSum' is: {standardName}");
// Use the standard function in a cell formula
worksheet.Cells["A1"].Formula = $"={standardName}(1,2,3)";
worksheet.Cells["A2"].Value = 1;
worksheet.Cells["A3"].Value = 2;
worksheet.Cells["A4"].Value = 3;
// Calculate the formula
workbook.CalculateFormula();
// Display the result
Console.WriteLine($"Formula result in A1: {worksheet.Cells["A1"].Value}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
}
// Save the workbook
workbook.Save("SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
