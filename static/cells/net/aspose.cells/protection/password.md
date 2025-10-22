##Protection.Password
Protection property. Represents the password to protect the worksheet
## Protection.Password property
Represents the password to protect the worksheet.
```csharp
public string Password { get; set; }
```
### Remarks
If password is set to null or blank string, you can unprotect the worksheet or workbook without using a password. Otherwise, you must specify the password to unprotect the worksheet or workbook.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectionPropertyPasswordDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set protection settings with password
Protection protection = worksheet.Protection;
protection.AllowEditingContent = false;
protection.AllowDeletingColumn = false;
protection.Password = "test123";
// Verify password protection
Console.WriteLine("Worksheet is protected: " + (protection.Password != null));
Console.WriteLine("Protection password: " + protection.Password);
// Create another protection object to compare
Protection protection2 = worksheet.Protection;
protection2.Password = "test123";
// Compare password protection
Console.WriteLine("Passwords match: " + (protection.Password == protection2.Password));
}
}
}
```
### See Also
* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
