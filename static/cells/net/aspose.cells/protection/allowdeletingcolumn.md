##Protection.AllowDeletingColumn
Protection property. Represents if the deletion of columns is allowed on a protected worksheet
## Protection.AllowDeletingColumn property
Represents if the deletion of columns is allowed on a protected worksheet.
```csharp
public bool AllowDeletingColumn { get; set; }
```
### Remarks
The columns containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectionPropertyAllowDeletingColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Enable worksheet protection
Protection protection = worksheet.Protection;
protection.AllowDeletingColumn = true;
worksheet.Protect(ProtectionType.All);
// Verify the setting
Console.WriteLine("AllowDeletingColumn: " + protection.AllowDeletingColumn);
// Try to delete a column (should work since AllowDeletingColumn is true)
worksheet.Cells.DeleteColumn(0);
Console.WriteLine("Column deleted successfully");
// Disable column deletion
protection.AllowDeletingColumn = false;
// Try to delete another column (should fail)
try
{
worksheet.Cells.DeleteColumn(1);
}
catch (Exception ex)
{
Console.WriteLine("Failed to delete column: " + ex.Message);
}
}
}
}
```
### See Also
* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
