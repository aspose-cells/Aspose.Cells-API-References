##ProtectedRange.IsProtectedWithPassword
ProtectedRange property. Indicates whether the worksheets is protected with password
## ProtectedRange.IsProtectedWithPassword property
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
public class ProtectedRangePropertyIsProtectedWithPasswordDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create protected ranges and get their indices
int protectedIndex = worksheet.AllowEditRanges.Add("PasswordProtected", 0, 0, 5, 5);
ProtectedRange protectedWithPassword = worksheet.AllowEditRanges[protectedIndex];
protectedWithPassword.Password = "test123";
int unprotectedIndex = worksheet.AllowEditRanges.Add("Unprotected", 6, 0, 11, 5);
ProtectedRange unprotected = worksheet.AllowEditRanges[unprotectedIndex];
// Protect worksheet to enforce restrictions
worksheet.Protect(ProtectionType.All);
// Verify password protection status
Console.WriteLine($"Range '{protectedWithPassword.Name}' password protected: {protectedWithPassword.IsProtectedWithPassword}");
Console.WriteLine($"Range '{unprotected.Name}' password protected: {unprotected.IsProtectedWithPassword}");
}
}
}
```
### See Also
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
