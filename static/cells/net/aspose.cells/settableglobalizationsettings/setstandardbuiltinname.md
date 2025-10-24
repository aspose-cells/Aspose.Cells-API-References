##SettableGlobalizationSettings.SetStandardBuiltInName
SettableGlobalizationSettings method. Sets the locale dependent function name according to given standard function name
## SettableGlobalizationSettings.SetStandardBuiltInName method
Sets the locale dependent function name according to given standard function name.
```csharp
public void SetStandardBuiltInName(string localName, string standardName, bool bidirectional)
```
| Parameter | Type | Description |
| --- | --- | --- |
| localName | String | Locale dependent function name |
| standardName | String | Standard(en-US locale) function name. |
| bidirectional | Boolean | Whether map the standard name text to local name text automatically. If true, the standar name text will be mapped to local name text automatically so user does not need to call [`SetLocalBuiltInName`](../setlocalbuiltinname/) again for the same standard and local names pair |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SettableGlobalizationSettingsMethodSetStandardBuiltInNameWithStringStringBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create custom globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
// Set the globalization settings for the workbook
workbook.Settings.GlobalizationSettings = settings;
try
{
// Call SetStandardBuiltInName to map a local name to a standard built-in name
// Parameters: localName, standardName, bidirectional
settings.SetStandardBuiltInName("MyLocalName", "SUM", true);
Console.WriteLine("SetStandardBuiltInName executed successfully with parameters (\"MyLocalName\", \"SUM\", true)");
// Demonstrate the effect by using the local name in a formula
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].Formula = "=MyLocalName(A1:A2)";
// Calculate the formula to show it works with the local name
workbook.CalculateFormula();
Console.WriteLine("Result of formula with local name: " + worksheet.Cells["A3"].Value);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetStandardBuiltInName method: {ex.Message}");
}
// Save the result
workbook.Save("SetStandardBuiltInNameDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
