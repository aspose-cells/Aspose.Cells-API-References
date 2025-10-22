##SettableGlobalizationSettings.GetStandardBuiltInName
SettableGlobalizationSettings method. Gets the standard text of builtin Name according to given locale dependent text
## SettableGlobalizationSettings.GetStandardBuiltInName method
Gets the standard text of built-in Name according to given locale dependent text.
```csharp
public override string GetStandardBuiltInName(string localName)
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
public class SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of SettableGlobalizationSettings
SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
// Set a local built-in name for demonstration
globalizationSettings.SetLocalBuiltInName("SUM", "LocalSumName", true);
try
{
// Call the GetStandardBuiltInName method with a local name
string standardName = globalizationSettings.GetStandardBuiltInName("LocalSumName");
// Display the result
Console.WriteLine($"Standard name for 'LocalSumName' is: {standardName}");
// Apply the result to a cell
worksheet.Cells["A1"].Formula = "=" + standardName + "(1,2,3)";
workbook.CalculateFormula();
// Display the calculated result
Console.WriteLine($"Result of formula in A1: {worksheet.Cells["A1"].Value}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetStandardBuiltInName method: {ex.Message}");
}
// Save the workbook
workbook.Save("SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
