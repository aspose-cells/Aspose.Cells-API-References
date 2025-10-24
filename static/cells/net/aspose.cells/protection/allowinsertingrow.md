##Protection.AllowInsertingRow
Protection property. Represents if the insertion of rows is allowed on a protected worksheet
## Protection.AllowInsertingRow property
Represents if the insertion of rows is allowed on a protected worksheet
```csharp
public bool AllowInsertingRow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectionPropertyAllowInsertingRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access the protection settings
Protection protection = worksheet.Protection;
// Enable inserting rows while protected
protection.AllowInsertingRow = true;
protection.Password = "password123";
worksheet.Protect(ProtectionType.All);
// Try to insert a row (should work since AllowInsertingRow is true)
worksheet.Cells.InsertRow(0);
// Save the workbook
workbook.Save("AllowInsertingRowDemo.xlsx");
}
}
}
```
### See Also
* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
