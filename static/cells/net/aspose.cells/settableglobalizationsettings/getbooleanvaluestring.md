##SettableGlobalizationSettings.GetBooleanValueString
SettableGlobalizationSettings method. Gets the display string value for cells boolean value
## SettableGlobalizationSettings.GetBooleanValueString method
Gets the display string value for cell's boolean value
```csharp
public override string GetBooleanValueString(bool bv)
```
| Parameter | Type | Description |
| --- | --- | --- |
| bv | Boolean | boolean value |
### Return Value
By default returns "TRUE" for true value and "FALSE" for false value.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SettableGlobalizationSettingsMethodGetBooleanValueStringWithBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create custom globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
// Set custom boolean value strings
settings.SetBooleanValueString(true, "TRUE_CUSTOM");
settings.SetBooleanValueString(false, "FALSE_CUSTOM");
// Apply the settings to the workbook
workbook.Settings.GlobalizationSettings = settings;
try
{
// Call GetBooleanValueString with true
string trueValue = settings.GetBooleanValueString(true);
Console.WriteLine("Custom true value: " + trueValue);
// Call GetBooleanValueString with false
string falseValue = settings.GetBooleanValueString(false);
Console.WriteLine("Custom false value: " + falseValue);
// Demonstrate the effect in the worksheet
worksheet.Cells["A1"].PutValue(true);
worksheet.Cells["A2"].PutValue(false);
Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].StringValue);
Console.WriteLine("Cell A2 value: " + worksheet.Cells["A2"].StringValue);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetBooleanValueString method: {ex.Message}");
}
// Save the workbook
workbook.Save("SettableGlobalizationSettingsMethodGetBooleanValueStringDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
