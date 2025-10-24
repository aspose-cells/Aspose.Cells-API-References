##SettableGlobalizationSettings.GetLocalFunctionName
SettableGlobalizationSettings method. Gets the locale dependent function name according to given standard function name
## SettableGlobalizationSettings.GetLocalFunctionName method
Gets the locale dependent function name according to given standard function name.
```csharp
public override string GetLocalFunctionName(string standardName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| standardName | String | Standard(en-US locale) function name. |
### Return Value
Locale dependent function name. The locale was specified by the Workbook for which this settings is used.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SettableGlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create custom globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
// Set a custom local function name for "SUM"
settings.SetLocalFunctionName("SUM", "SOMME", true);
// Apply the settings to the workbook
workbook.Settings.GlobalizationSettings = settings;
try
{
// Call GetLocalFunctionName to retrieve the localized name
string localName = settings.GetLocalFunctionName("SUM");
// Display the result
Console.WriteLine($"Localized function name for 'SUM': {localName}");
// Use the localized function in a cell
worksheet.Cells["A1"].Formula = "=SOMME(B1:B5)";
worksheet.Cells["B1"].PutValue(1);
worksheet.Cells["B2"].PutValue(2);
worksheet.Cells["B3"].PutValue(3);
worksheet.Cells["B4"].PutValue(4);
worksheet.Cells["B5"].PutValue(5);
// Calculate formulas
workbook.CalculateFormula();
// Display the result
Console.WriteLine($"Calculation result with localized function: {worksheet.Cells["A1"].Value}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetLocalFunctionName method: {ex.Message}");
}
// Save the workbook
workbook.Save("MethodGetLocalFunctionNameWithStringDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
