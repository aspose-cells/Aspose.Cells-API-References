##Style.IsProtectionApplied
Style property. Indicate whether the protection formatting should be applied
## Style.IsProtectionApplied property
Indicate whether the protection formatting should be applied.
```csharp
public bool IsProtectionApplied { get; set; }
```
### Remarks
Only for named style.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyIsProtectionAppliedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a style object
Style style = workbook.CreateStyle();
// Set protection properties
style.IsLocked = true;
style.IsFormulaHidden = true;
style.IsProtectionApplied = true;
// Apply the style to a cell
Cell cell = worksheet.Cells["A1"];
cell.SetStyle(style);
// Verify protection settings
Console.WriteLine("IsProtectionApplied: " + style.IsProtectionApplied);
Console.WriteLine("IsLocked: " + style.IsLocked);
Console.WriteLine("IsFormulaHidden: " + style.IsFormulaHidden);
// Modify protection settings
style.IsProtectionApplied = false;
Console.WriteLine("\nAfter changing IsProtectionApplied to false:");
Console.WriteLine("IsProtectionApplied: " + style.IsProtectionApplied);
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
