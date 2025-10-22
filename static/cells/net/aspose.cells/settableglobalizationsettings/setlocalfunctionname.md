##SettableGlobalizationSettings.SetLocalFunctionName
SettableGlobalizationSettings method. Sets the locale dependent function name corresponding to given standard function name
## SettableGlobalizationSettings.SetLocalFunctionName method
Sets the locale dependent function name corresponding to given standard function name.
```csharp
public void SetLocalFunctionName(string standardName, string localName, bool bidirectional)
```
| Parameter | Type | Description |
| --- | --- | --- |
| standardName | String | Standard(en-US locale) function name. |
| localName | String | Locale dependent function name |
| bidirectional | Boolean | Whether map the local function name to standard function name automatically. If true, the local name will be mapped to standard name automatically so user does not need to call [`SetStandardFunctionName`](../setstandardfunctionname/) again for the same standard and local names pair |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SettableGlobalizationSettingsMethodSetLocalFunctionNameWithStringStringBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
try
{
// Call SetLocalFunctionName to map standard function name to local name
settings.SetLocalFunctionName("SUM", "SOMMA", true); // Italian localization for SUM function
settings.SetLocalFunctionName("AVERAGE", "MEDIA", true); // Italian localization for AVERAGE function
// Apply the settings to the workbook
workbook.Settings.GlobalizationSettings = settings;
// Create formulas using both standard and localized names
worksheet.Cells["A1"].Formula = "=SUM(B1:B5)";
worksheet.Cells["A2"].Formula = "=SOMMA(B1:B5)";
worksheet.Cells["A3"].Formula = "=AVERAGE(B1:B5)";
worksheet.Cells["A4"].Formula = "=MEDIA(B1:B5)";
// Calculate formulas
workbook.CalculateFormula();
Console.WriteLine("SetLocalFunctionName executed successfully with parameters (String, String, Boolean)");
Console.WriteLine("Standard and localized function names work equivalently in formulas.");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetLocalFunctionName method: {ex.Message}");
}
// Save the result
workbook.Save("MethodSetLocalFunctionNameWithStringStringBooleanDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
