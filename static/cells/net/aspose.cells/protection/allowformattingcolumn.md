##Protection.AllowFormattingColumn
Protection property. Represents if the formatting of columns is allowed on a protected worksheet
## Protection.AllowFormattingColumn property
Represents if the formatting of columns is allowed on a protected worksheet
```csharp
public bool AllowFormattingColumn { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectionPropertyAllowFormattingColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access protection settings
Protection protection = worksheet.Protection;
// Set AllowFormattingColumn property
protection.AllowFormattingColumn = true;
// Verify and print the property value
Console.WriteLine("AllowFormattingColumn: " + protection.AllowFormattingColumn);
// Demonstrate setting multiple protection properties
protection.AllowDeletingColumn = true;
protection.AllowFormattingRow = true;
// Call the flag calculation method
int protectionFlags = CalculateProtectionFlags(protection);
Console.WriteLine("Protection Flags: 0x" + protectionFlags.ToString("X4"));
}
private static int CalculateProtectionFlags(Protection protection)
{
int flag = 0;
if (protection.AllowDeletingColumn) { flag |= 0x0001; }
if (protection.AllowDeletingRow) { flag |= 0x0002; }
if (protection.AllowEditingContent) { flag |= 0x0004; }
if (protection.AllowEditingObject) { flag |= 0x0008; }
if (protection.AllowEditingScenario) { flag |= 0x0010; }
if (protection.AllowFiltering) { flag |= 0x0020; }
if (protection.AllowFormattingCell) { flag |= 0x0040; }
if (protection.AllowFormattingColumn) { flag |= 0x0080; }
if (protection.AllowFormattingRow) { flag |= 0x0100; }
if (protection.AllowInsertingColumn) { flag |= 0x0200; }
if (protection.AllowInsertingHyperlink) { flag |= 0x0400; }
if (protection.AllowInsertingRow) { flag |= 0x0800; }
if (protection.AllowSelectingLockedCell) { flag |= 0x1000; }
if (protection.AllowSelectingUnlockedCell) { flag |= 0x2000; }
if (protection.AllowSorting) { flag |= 0x4000; }
if (protection.AllowUsingPivotTable) { flag |= 0x8000; }
return flag;
}
}
}
```
### See Also
* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
