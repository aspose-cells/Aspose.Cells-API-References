##GlobalizationSettings.GetDefaultSheetName
GlobalizationSettings method. Gets the default sheet name for adding worksheet automatically. Default is Sheet
## GlobalizationSettings.GetDefaultSheetName method
Gets the default sheet name for adding worksheet automatically. Default is "Sheet".
```csharp
public virtual string GetDefaultSheetName()
```
### Return Value
the default sheet name for adding worksheet automatically
### Remarks
The automatically added(such as by [`Add`](../../worksheetcollection/add/)) sheet's name will be the specified name plus sequence number. For example, for Germany user maybe wants the sheet name to be "Tabellenblatt2" instead of "Sheet2". Then user may implement this method to return "Tabellenblatt".
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class GlobalizationSettingsMethodGetDefaultSheetNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set custom globalization settings
workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
try
{
// Get the default sheet name from custom globalization settings
string defaultSheetName = workbook.Settings.GlobalizationSettings.GetDefaultSheetName();
Console.WriteLine($"Default sheet name retrieved: {defaultSheetName}");
// Add a new worksheet to demonstrate naming based on the custom default
int sheetIndex = workbook.Worksheets.Add();
Worksheet newWorksheet = workbook.Worksheets[sheetIndex];
Console.WriteLine($"New worksheet name after method call: {newWorksheet.Name}");
Console.WriteLine("GetDefaultSheetName method demonstration completed successfully.");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetDefaultSheetName method: {ex.Message}");
}
// Save the workbook
workbook.Save("MethodGetDefaultSheetNameDemo.xlsx");
}
}
// Custom globalization settings implementation
public class CustomGlobalizationSettings : GlobalizationSettings
{
public override string GetDefaultSheetName()
{
return "CustomSheet"; // Custom default sheet name
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
