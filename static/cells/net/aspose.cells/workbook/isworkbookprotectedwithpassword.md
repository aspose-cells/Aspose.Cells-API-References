##Workbook.IsWorkbookProtectedWithPassword
Workbook property. Indicates whether structure or window is protected with password
## Workbook.IsWorkbookProtectedWithPassword property
Indicates whether structure or window is protected with password.
```csharp
public bool IsWorkbookProtectedWithPassword { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookPropertyIsWorkbookProtectedWithPasswordDemo
{
public static void Run()
{
// Create a new Workbook instance
Workbook workbook = new Workbook();
// Check if the workbook is protected with password (should be false for new workbook)
Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);
// Protect the workbook with a password
workbook.Protect(ProtectionType.All, "password123");
// Now check again (should be true)
Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);
// Unprotect the workbook
workbook.Unprotect("password123");
// Final check (should be false again)
Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);
// Dispose the workbook
workbook.Dispose();
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
