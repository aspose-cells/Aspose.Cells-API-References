##SettableGlobalizationSettings.SetStandardFunctionName
SettableGlobalizationSettings method. Sets the locale dependent function name according to given standard function name
## SettableGlobalizationSettings.SetStandardFunctionName method
Sets the locale dependent function name according to given standard function name.
```csharp
public void SetStandardFunctionName(string localName, string standardName, bool bidirectional)
```
| Parameter | Type | Description |
| --- | --- | --- |
| localName | String | Locale dependent function name |
| standardName | String | Standard(en-US locale) function name. |
| bidirectional | Boolean | Whether map the standard function name to local function name automatically. If true, the standar name will be mapped to local name automatically so user does not need to call [`SetLocalFunctionName`](../setlocalfunctionname/) again for the same standard and local names pair |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SettableGlobalizationSettingsMethodSetStandardFunctionNameWithStringStringBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create custom globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
try
{
// Call SetStandardFunctionName to map a local function name to standard name
settings.SetStandardFunctionName("LOCAL_SUM", "SUM", true);
// Apply the settings to workbook
workbook.Settings.GlobalizationSettings = settings;
// Create a formula using the local function name
worksheet.Cells["A1"].Formula = "=LOCAL_SUM(B1:B3)";
worksheet.Cells["B1"].Value = 10;
worksheet.Cells["B2"].Value = 20;
worksheet.Cells["B3"].Value = 30;
// Calculate the formula
workbook.CalculateFormula();
Console.WriteLine("Formula with local function name 'LOCAL_SUM' calculated successfully.");
Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetStandardFunctionName method: {ex.Message}");
}
// Save the result
workbook.Save("SetStandardFunctionNameDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
