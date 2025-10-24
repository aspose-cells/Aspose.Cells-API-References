##PivotGlobalizationSettings.GetTextOf4Quaters
PivotGlobalizationSettings method. Gets the local text of 4 Quaters
## PivotGlobalizationSettings.GetTextOf4Quaters method
Gets the local text of 4 Quaters.
```csharp
public virtual string[] GetTextOf4Quaters()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Settings;
using System;
public class PivotGlobalizationSettingsMethodGetTextOf4QuatersDemo
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
// Call the GetTextOf4Quaters method
string[] quarterNames = customGlobalizationSettings.GetTextOf4Quaters();
// Output the quarter names to console
Console.WriteLine("Names of 4 quarters:");
foreach (string quarterName in quarterNames)
{
Console.WriteLine(quarterName);
}
// Add the quarter names to the worksheet
for (int i = 0; i < quarterNames.Length; i++)
{
worksheet.Cells[i, 0].PutValue(quarterNames[i]);
}
Console.WriteLine("Method executed successfully. Quarter names added to worksheet.");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetTextOf4Quaters method: {ex.Message}");
}
// Save the result
workbook.Save("MethodGetTextOf4QuatersDemo.xlsx");
}
}
// Custom implementation of PivotGlobalizationSettings to override GetTextOf4Quaters
public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
{
public override string[] GetTextOf4Quaters()
{
// Return custom quarter names
return new string[] { "First Quarter", "Second Quarter",
"Third Quarter", "Fourth Quarter" };
}
}
}
```
### See Also
* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)
