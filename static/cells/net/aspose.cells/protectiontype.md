##Enum ProtectionType
Aspose.Cells.ProtectionType enum. Represents workbook/worksheet protection type
## ProtectionType enumeration
Represents workbook/worksheet protection type.
```csharp
public enum ProtectionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| All | `0` | Represents to protect all. |
| Contents | `1` | Represents to protect contents, used in Worksheet protection. |
| Objects | `2` | Represents to protect objects, used in Worksheet protection. |
| Scenarios | `3` | Represents to protect scenarios, used in Worksheet protection. |
| Structure | `4` | Represents to protect structure, used in Workbook protection. |
| Windows | `5` | Represents to protect window, used in Workbook protection. |
| None | `6` | Represents no protection. Only for Reading property. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassProtectionTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Protect the worksheet with all protection types
worksheet.Protect(ProtectionType.All);
// Demonstrate accessing protection properties
Console.WriteLine("Worksheet protection settings:");
Console.WriteLine("AllowDeletingColumn: " + worksheet.Protection.AllowDeletingColumn);
Console.WriteLine("AllowDeletingRow: " + worksheet.Protection.AllowDeletingRow);
Console.WriteLine("AllowFiltering: " + worksheet.Protection.AllowFiltering);
Console.WriteLine("AllowFormattingCell: " + worksheet.Protection.AllowFormattingCell);
Console.WriteLine("AllowFormattingColumn: " + worksheet.Protection.AllowFormattingColumn);
Console.WriteLine("AllowFormattingRow: " + worksheet.Protection.AllowFormattingRow);
Console.WriteLine("AllowInsertingColumn: " + worksheet.Protection.AllowInsertingColumn);
Console.WriteLine("AllowInsertingHyperlink: " + worksheet.Protection.AllowInsertingHyperlink);
Console.WriteLine("AllowInsertingRow: " + worksheet.Protection.AllowInsertingRow);
Console.WriteLine("AllowSorting: " + worksheet.Protection.AllowSorting);
Console.WriteLine("AllowUsingPivotTable: " + worksheet.Protection.AllowUsingPivotTable);
// Unprotect the worksheet
worksheet.Unprotect();
// Protect with specific protection types
worksheet.Protect(ProtectionType.Contents | ProtectionType.Objects);
Console.WriteLine("\nWorksheet protected with Contents and Objects only");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
