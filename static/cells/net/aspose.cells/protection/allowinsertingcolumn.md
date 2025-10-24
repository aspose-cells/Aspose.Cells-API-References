##Protection.AllowInsertingColumn
Protection property. Represents if the insertion of columns is allowed on a protected worksheet
## Protection.AllowInsertingColumn property
Represents if the insertion of columns is allowed on a protected worksheet
```csharp
public bool AllowInsertingColumn { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectionPropertyAllowInsertingColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the protection settings
Protection protection = worksheet.Protection;
// Set AllowInsertingColumn to true
protection.AllowInsertingColumn = true;
// Verify the setting
Console.WriteLine("AllowInsertingColumn is set to: " + protection.AllowInsertingColumn);
// Protect the worksheet with password (using Workbook.Protect method)
workbook.Protect(ProtectionType.All, "password123");
protection.AllowInsertingColumn = true; // Explicitly set again to demonstrate
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
