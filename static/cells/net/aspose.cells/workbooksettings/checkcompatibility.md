##WorkbookSettings.CheckCompatibility
WorkbookSettings property. Indicates whether check compatibility with earlier versions when saving workbook
## WorkbookSettings.CheckCompatibility property
Indicates whether check compatibility with earlier versions when saving workbook.
```csharp
public bool CheckCompatibility { get; set; }
```
### Remarks
The default value is true. Only for Excel97-2003 xls or xlt files.
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyCheckCompatibilityDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set CheckCompatibility to true and save
workbook.Settings.CheckCompatibility = true;
workbook.Save("CheckCompatibilityDemo_true.xlsx");
// Reload and verify
workbook = new Workbook("CheckCompatibilityDemo_true.xlsx");
Console.WriteLine("CheckCompatibility (true): " + workbook.Settings.CheckCompatibility);
// Set CheckCompatibility to false and save
workbook.Settings.CheckCompatibility = false;
workbook.Save("CheckCompatibilityDemo_false.xlsx");
// Reload and verify
workbook = new Workbook("CheckCompatibilityDemo_false.xlsx");
Console.WriteLine("CheckCompatibility (false): " + workbook.Settings.CheckCompatibility);
// Demonstrate color operations
Console.WriteLine("Is Red in palette: " + workbook.IsColorInPalette(Color.Red));
Color customColor = workbook.GetMatchingColor(Color.FromArgb(255, 123, 123, 123));
Console.WriteLine("Matching color R value: " + customColor.R);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
