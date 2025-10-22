##Protection.GetPasswordHash
Protection method. Gets the hash of current password
## Protection.GetPasswordHash method
Gets the hash of current password.
```csharp
public int GetPasswordHash()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ProtectionMethodGetPasswordHashDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set protection settings with password
Protection protection = worksheet.Protection;
protection.Password = "password123";
protection.AllowDeletingColumn = true;
protection.AllowFormattingCell = true;
// Protect the worksheet
worksheet.Protect(ProtectionType.All);
try
{
// Get the password hash
int passwordHash = protection.GetPasswordHash();
// Display the result
Console.WriteLine($"Password hash: {passwordHash}");
Console.WriteLine($"Is protected with password: {protection.IsProtectedWithPassword}");
// Verify the password (demonstrating related functionality)
bool isVerified = protection.VerifyPassword("password123");
Console.WriteLine($"Password verification result: {isVerified}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetPasswordHash method: {ex.Message}");
}
// Save the workbook
workbook.Save("ProtectionMethodGetPasswordHashDemo.xlsx");
}
}
}
```
### See Also
* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
