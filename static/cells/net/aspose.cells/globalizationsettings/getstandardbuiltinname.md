##GlobalizationSettings.GetStandardBuiltInName
GlobalizationSettings method. Gets the standard text of builtin Name according to given locale dependent text
## GlobalizationSettings.GetStandardBuiltInName method
Gets the standard text of built-in Name according to given locale dependent text.
```csharp
public virtual string GetStandardBuiltInName(string localName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| localName | String | Locale dependent text of built-in Name. The locale was specified by the Workbook for which this settings is used. |
### Return Value
Standard(en-US locale) text.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class GlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
{
public static void Run()
{
// Create a workbook with custom globalization settings
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Initialize custom globalization settings and assign to workbook
var globalizationSettings = new CustomGlobalizationSettings();
workbook.Settings.GlobalizationSettings = globalizationSettings;
// Test parameter for GetStandardBuiltInName
string localFunctionName = "MyLocalSum";
try
{
// Call GetStandardBuiltInName with local function name
string standardName = globalizationSettings.GetStandardBuiltInName(localFunctionName);
Console.WriteLine($"Local name: '{localFunctionName}' => Standard name: '{standardName}'");
// Demonstrate effect by using the local name in a formula
worksheet.Cells["A1"].Value = 5;
worksheet.Cells["A2"].Value = 7;
worksheet.Cells["A3"].Formula = $"{localFunctionName}(A1:A2)";
// Calculate formula to show correct interpretation
workbook.CalculateFormula();
Console.WriteLine($"Formula result: {worksheet.Cells["A3"].Value}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetStandardBuiltInName: {ex.Message}");
}
// Save the modified workbook
workbook.Save("GlobalizationGetStandardBuiltInNameDemo.xlsx");
}
}
// Custom globalization settings overriding GetStandardBuiltInName
public class CustomGlobalizationSettings : GlobalizationSettings
{
public override string GetStandardBuiltInName(string localName)
{
// Map custom local function name to standard SUM
if (localName.Equals("MyLocalSum", StringComparison.OrdinalIgnoreCase))
{
return "SUM";
}
return base.GetStandardBuiltInName(localName);
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
