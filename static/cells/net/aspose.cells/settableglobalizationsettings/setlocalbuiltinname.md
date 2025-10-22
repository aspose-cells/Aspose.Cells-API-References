##SettableGlobalizationSettings.SetLocalBuiltInName
SettableGlobalizationSettings method. Sets the locale dependent text for the builtin name with given standard name text
## SettableGlobalizationSettings.SetLocalBuiltInName method
Sets the locale dependent text for the built-in name with given standard name text.
```csharp
public void SetLocalBuiltInName(string standardName, string localName, bool bidirectional)
```
| Parameter | Type | Description |
| --- | --- | --- |
| standardName | String | Standard(en-US locale) name text of built-in name. |
| localName | String | Locale dependent name text |
| bidirectional | Boolean | Whether map the local name text to standard name text automatically. If true, the local name text will be mapped to standard name text automatically so user does not need to call [`SetStandardBuiltInName`](../setstandardbuiltinname/) again for the same standard and local names pair |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SettableGlobalizationSettingsMethodSetLocalBuiltInNameWithStringStringBooleanDemo
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
// Call SetLocalBuiltInName to map a standard built-in name to a local name
settings.SetLocalBuiltInName("SUM", "LOCAL_SUM", true);
// Apply the settings to the workbook
workbook.Settings.GlobalizationSettings = settings;
// Create a formula using the standard built-in name
worksheet.Cells["A1"].Formula = "=SUM(B1:B3)";
worksheet.Cells["B1"].Value = 5;
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["B3"].Value = 15;
// Calculate the formula
workbook.CalculateFormula();
Console.WriteLine("Formula with standard built-in name 'SUM' calculated successfully.");
Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");
// Verify the local name mapping
string localName = settings.GetLocalBuiltInName("SUM");
Console.WriteLine($"Local name for 'SUM': {localName}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetLocalBuiltInName method: {ex.Message}");
}
// Save the result
workbook.Save("SetLocalBuiltInNameDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
