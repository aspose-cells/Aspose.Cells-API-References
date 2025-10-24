##SettableGlobalizationSettings.SetBooleanValueString
SettableGlobalizationSettings method. Sets the display string value for cells boolean value
## SettableGlobalizationSettings.SetBooleanValueString method
Sets the display string value for cell's boolean value
```csharp
public void SetBooleanValueString(bool bv, string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| bv | Boolean | boolean value |
| name | String | string value of the boolean value |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SettableGlobalizationSettingsMethodSetBooleanValueStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create custom globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
// Set custom boolean value strings
settings.SetBooleanValueString(true, "Yes");
settings.SetBooleanValueString(false, "No");
// Apply the settings to the workbook
workbook.Settings.GlobalizationSettings = settings;
// Set boolean values in cells
worksheet.Cells["A1"].PutValue(true);
worksheet.Cells["A2"].PutValue(false);
// Set display style to show boolean values as text
Style style = workbook.CreateStyle();
style.Custom = "BOOLEAN";
worksheet.Cells["A1"].SetStyle(style);
worksheet.Cells["A2"].SetStyle(style);
try
{
// Save the workbook
workbook.Save("SetBooleanValueStringDemo.xlsx");
Console.WriteLine("Workbook saved with custom boolean value strings.");
}
catch (Exception ex)
{
Console.WriteLine($"Error saving workbook: {ex.Message}");
}
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
