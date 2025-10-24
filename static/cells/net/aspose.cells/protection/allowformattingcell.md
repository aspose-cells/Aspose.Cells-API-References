##Protection.AllowFormattingCell
Protection property. Represents if the formatting of cells is allowed on a protected worksheet
## Protection.AllowFormattingCell property
Represents if the formatting of cells is allowed on a protected worksheet.
```csharp
public bool AllowFormattingCell { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectionPropertyAllowFormattingCellDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Enable worksheet protection
Protection protection = worksheet.Protection;
// Set various protection properties using a flag
int flag = 0x40; // Only AllowFormattingCell flag is set
protection.AllowFormattingCell = (flag & 0x40) != 0;
// Verify the setting
Console.WriteLine("AllowFormattingCell is set to: " + protection.AllowFormattingCell);
// Save the workbook
workbook.Save("ProtectionDemo.xlsx");
}
}
}
```
### See Also
* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
