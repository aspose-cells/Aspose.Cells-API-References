##GlobalizationSettings.GetLocalFunctionName
GlobalizationSettings method. Gets the locale dependent function name according to given standard function name
## GlobalizationSettings.GetLocalFunctionName method
Gets the locale dependent function name according to given standard function name.
```csharp
public virtual string GetLocalFunctionName(string standardName)
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
public class GlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set custom globalization settings
workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
// Add sample data
worksheet.Cells["B1"].PutValue(5);
worksheet.Cells["B2"].PutValue(15);
// Create formula with localized function name
Cell cell = worksheet.Cells["B3"];
cell.Formula = "=LOCALSUM(B1:B2)";
try
{
workbook.CalculateFormula();
Console.WriteLine($"Calculation result using localized function: {cell.DoubleValue}");
}
catch (Exception ex)
{
Console.WriteLine($"Calculation error: {ex.Message}");
}
workbook.Save("GlobalizationSettingsFunctionDemo.xlsx");
}
private class CustomGlobalizationSettings : GlobalizationSettings
{
public override string GetLocalFunctionName(string standardName)
{
if (standardName == "SUM")
{
return "LOCALSUM";
}
return base.GetLocalFunctionName(standardName);
}
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
