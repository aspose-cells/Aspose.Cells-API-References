##WarningInfo.Description
WarningInfo property. Get description of warning info
## WarningInfo.Description property
Get description of warning info.
```csharp
public string Description { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WarningInfoPropertyDescriptionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a duplicate defined name to trigger warning
worksheet.Cells.CreateRange(0, 0, 10, 10).Name = "_XLNM.PRINT_AREA";
worksheet.Cells.CreateRange(0, 0, 10, 10).Name = "_XLNM.PRINT_AREA"; // Different name to actually trigger warning
// Get warning callback
WarningCallback callback = new WarningCallback();
workbook.Settings.WarningCallback = callback; // Correct property path
// Save to trigger warning
workbook.Save("output.xlsx");
// Demonstrate Description property usage
if (callback.LastWarning != null)
{
Console.WriteLine("Warning Description: " + callback.LastWarning.Description);
Console.WriteLine("Warning Type: " + callback.LastWarning.Type);
}
}
}
public class WarningCallback : IWarningCallback
{
public WarningInfo LastWarning { get; private set; }
public void Warning(WarningInfo warningInfo)
{
LastWarning = warningInfo;
}
}
}
```
### See Also
* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
