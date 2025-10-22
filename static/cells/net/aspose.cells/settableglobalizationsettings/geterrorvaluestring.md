##SettableGlobalizationSettings.GetErrorValueString
SettableGlobalizationSettings method. Gets the display string value for cells error value
## SettableGlobalizationSettings.GetErrorValueString method
Gets the display string value for cell's error value
```csharp
public override string GetErrorValueString(string err)
```
| Parameter | Type | Description |
| --- | --- | --- |
| err | String | error values such as #VALUE!,#NAME? |
### Return Value
By default returns the error value itself
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class SettableGlobalizationSettingsMethodGetErrorValueStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create custom globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
workbook.Settings.GlobalizationSettings = settings;
// Create a cell with error value
Cell cell = worksheet.Cells["A1"];
cell.PutValue("#N/A");
Style style = workbook.CreateStyle();
cell.SetStyle(style);
style.Number = 10; // Set format to Error value
try
{
// Call GetErrorValueString with error value string
string errorString = settings.GetErrorValueString("#N/A");
// Display the result
Console.WriteLine("Error value string: " + errorString);
// Show effect by setting another cell's value to the returned string
worksheet.Cells["A2"].PutValue("Error representation: " + errorString);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetErrorValueString method: {ex.Message}");
}
// Save the workbook
workbook.Save("MethodGetErrorValueStringDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
