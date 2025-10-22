##PivotGlobalizationSettings.GetShortTextOf12Months
PivotGlobalizationSettings method. Gets all short formatted string of 12 months
## PivotGlobalizationSettings.GetShortTextOf12Months method
Gets all short formatted string of 12 months.
```csharp
public virtual string[] GetShortTextOf12Months()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Settings;
using System;
public class PivotGlobalizationSettingsMethodGetShortTextOf12MonthsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a custom globalization settings class that inherits from PivotGlobalizationSettings
var customGlobalizationSettings = new CustomPivotGlobalizationSettings();
try
{
// Call the GetShortTextOf12Months method
string[] monthShortNames = customGlobalizationSettings.GetShortTextOf12Months();
// Output the month names to console
Console.WriteLine("Short names of 12 months:");
foreach (string monthName in monthShortNames)
{
Console.WriteLine(monthName);
}
// Add the month names to the worksheet
for (int i = 0; i < monthShortNames.Length; i++)
{
worksheet.Cells[i, 0].PutValue(monthShortNames[i]);
}
Console.WriteLine("Method executed successfully. Month names added to worksheet.");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetShortTextOf12Months method: {ex.Message}");
}
// Save the result
workbook.Save("MethodGetShortTextOf12MonthsDemo.xlsx");
}
}
// Custom implementation of PivotGlobalizationSettings to override GetShortTextOf12Months
public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
{
public override string[] GetShortTextOf12Months()
{
// Return custom short month names
return new string[] { "Jan", "Feb", "Mar", "Apr", "May", "Jun",
"Jul", "Aug", "Sep", "Oct", "Nov", "Dec" };
}
}
}
```
### See Also
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)
