##GlobalizationSettings.GetStandardFunctionName
GlobalizationSettings method. Gets the standard function name according to given locale dependent function name
## GlobalizationSettings.GetStandardFunctionName method
Gets the standard function name according to given locale dependent function name.
```csharp
public virtual string GetStandardFunctionName(string localName)
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
public class GlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare sample data
worksheet.Cells["A1"].PutValue(5);
worksheet.Cells["A2"].PutValue(15);
// Create custom globalization settings and assign to workbook
var customSettings = new CustomGlobalizationSettings();
workbook.Settings.GlobalizationSettings = customSettings;
try
{
// Demonstrate GetStandardFunctionName with German SUM function name
string localName = "SUMME";
string standardName = customSettings.GetStandardFunctionName(localName);
Console.WriteLine($"Local function name: {localName}");
Console.WriteLine($"Standard function name: {standardName}");
// Apply localized function name in formula
worksheet.Cells["A3"].Formula = "=SUMME(A1:A2)";
workbook.CalculateFormula();
Console.WriteLine($"Formula result: {worksheet.Cells["A3"].Value}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
}
workbook.Save("MethodGetStandardFunctionNameDemo.xlsx");
}
private class CustomGlobalizationSettings : GlobalizationSettings
{
public override string GetStandardFunctionName(string localName)
{
// Convert German function name to standard English
if (localName.Equals("SUMME", StringComparison.OrdinalIgnoreCase))
{
return "SUM";
}
return base.GetStandardFunctionName(localName);
}
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
