##Protection.IsProtectedWithPassword
Protection property. Indicates whether the worksheets is protected with password
## Protection.IsProtectedWithPassword property
Indicates whether the worksheets is protected with password.
```csharp
public bool IsProtectedWithPassword { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectionPropertyIsProtectedWithPasswordDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access worksheet protection settings
Protection protection = worksheet.Protection;
// Set protection password
protection.Password = "test123";
// Check if worksheet is password protected
bool isProtectedWithPassword = protection.IsProtectedWithPassword;
Console.WriteLine("Is worksheet protected with password: " + isProtectedWithPassword);
// Save the workbook
workbook.Save("PasswordProtectionDemo.xlsx");
}
}
}
```
### See Also
* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
