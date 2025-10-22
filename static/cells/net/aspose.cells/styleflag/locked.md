##StyleFlag.Locked
StyleFlag property. Locked setting will be applied
## StyleFlag.Locked property
Locked setting will be applied.
```csharp
public bool Locked { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyLockedDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create a style and set its locked property
Style style = workbook.CreateStyle();
style.IsLocked = true;
// Create a style flag and enable locked flag
StyleFlag styleFlag = new StyleFlag();
styleFlag.Locked = true;
// Apply the style to cell A1
Cell cell = cells["A1"];
cell.SetStyle(style, styleFlag);
// Verify the locked status
Console.WriteLine("Cell A1 is locked: " + cell.GetStyle().IsLocked);
// Protect the worksheet to see the locking effect
worksheet.Protect(ProtectionType.All);
// Try to modify the locked cell (will throw exception when worksheet is protected)
try
{
cell.PutValue("Test");
Console.WriteLine("Cell modified successfully (worksheet not properly protected)");
}
catch
{
Console.WriteLine("Could not modify locked cell (worksheet protected)");
}
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
