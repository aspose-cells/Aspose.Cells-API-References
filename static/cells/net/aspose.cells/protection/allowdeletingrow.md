##Protection.AllowDeletingRow
Protection property. Represents if the deletion of rows is allowed on a protected worksheet
## Protection.AllowDeletingRow property
Represents if the deletion of rows is allowed on a protected worksheet.
```csharp
public bool AllowDeletingRow { get; set; }
```
### Remarks
The rows containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectionPropertyAllowDeletingRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Set protection settings
Protection protection = sheet.Protection;
protection.AllowDeletingRow = true;
protection.AllowSorting = true;
protection.AllowFiltering = true;
protection.AllowFormattingColumn = true;
// Protect the worksheet
sheet.Protect(ProtectionType.All);
// Save the workbook
workbook.Save("output.xlsx");
// Load the saved workbook to verify settings
Workbook loadedWorkbook = new Workbook("output.xlsx");
Worksheet loadedSheet = loadedWorkbook.Worksheets[0];
// Verify AllowDeletingRow and other properties
Console.WriteLine("AllowDeletingRow: " + loadedSheet.Protection.AllowDeletingRow);
Console.WriteLine("AllowSorting: " + loadedSheet.Protection.AllowSorting);
Console.WriteLine("AllowFiltering: " + loadedSheet.Protection.AllowFiltering);
Console.WriteLine("AllowFormattingColumn: " + loadedSheet.Protection.AllowFormattingColumn);
}
}
}
```
### See Also
* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
