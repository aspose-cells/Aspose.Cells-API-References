##SettableGlobalizationSettings.SetListSeparator
SettableGlobalizationSettings method. Sets the separator for list parameters of function ...etc
## SettableGlobalizationSettings.SetListSeparator method
Sets the separator for list, parameters of function, ...etc.
```csharp
public void SetListSeparator(char c)
```
| Parameter | Type | Description |
| --- | --- | --- |
| c | Char | the specified separator |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SettableGlobalizationSettingsMethodSetListSeparatorWithCharDemo
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
// Call the SetListSeparator method with a character parameter
settings.SetListSeparator(';');
// Apply the settings to the workbook
workbook.Settings.GlobalizationSettings = settings;
// Demonstrate the effect by creating a formula with list separator
worksheet.Cells["A1"].Formula = "SUM(1;2;3)";
worksheet.Cells["A2"].Value = "Formula using custom list separator: SUM(1;2;3)";
Console.WriteLine("SetListSeparator method executed successfully with parameter ';'");
Console.WriteLine("Formula using custom list separator created in cell A1");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetListSeparator method: {ex.Message}");
}
// Save the result
workbook.Save("SetListSeparatorWithCharDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
