##GlobalizationSettings.GetBooleanValueString
GlobalizationSettings method. Gets the display string value for cells boolean value
## GlobalizationSettings.GetBooleanValueString method
Gets the display string value for cell's boolean value
```csharp
public virtual string GetBooleanValueString(bool bv)
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
public class GlobalizationSettingsMethodGetBooleanValueStringWithBooleanDemo
{
public static void Run()
{
// Create a new workbook with custom globalization settings
Workbook workbook = new Workbook();
workbook.Settings.GlobalizationSettings = new CustomBooleanGlobalizationSettings();
Worksheet worksheet = workbook.Worksheets[0];
try
{
// Demonstrate GetBooleanValueString with both boolean values
var globalizationSettings = workbook.Settings.GlobalizationSettings;
string trueResult = globalizationSettings.GetBooleanValueString(true);
string falseResult = globalizationSettings.GetBooleanValueString(false);
Console.WriteLine($"GetBooleanValueString(true) returns: {trueResult}");
Console.WriteLine($"GetBooleanValueString(false) returns: {falseResult}");
// Apply boolean values to cells to show spreadsheet effect
worksheet.Cells["A1"].PutValue(true);
worksheet.Cells["A2"].PutValue(false);
workbook.Save("GlobalizationBooleanDemo.xlsx");
Console.WriteLine("Workbook saved with custom boolean representations.");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetBooleanValueString: {ex.Message}");
}
}
}
// Custom globalization settings overriding boolean string representation
public class CustomBooleanGlobalizationSettings : GlobalizationSettings
{
public override string GetBooleanValueString(bool bv)
{
return bv ? "Enabled" : "Disabled";
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
