##Protection.VerifyPassword
Protection method. Verifies password
## Protection.VerifyPassword method
Verifies password.
```csharp
public bool VerifyPassword(string password)
```
| Parameter | Type | Description |
| --- | --- | --- |
| password | String | The password. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ProtectionMethodVerifyPasswordWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Protect the worksheet with a password
worksheet.Protection.AllowDeletingColumn = false;
worksheet.Protection.AllowDeletingRow = false;
worksheet.Protection.Password = "password123";
worksheet.Protect(ProtectionType.All);
try
{
// Verify the password
bool isPasswordCorrect = worksheet.Protection.VerifyPassword("password123");
Console.WriteLine($"Password verification result: {isPasswordCorrect}");
if (isPasswordCorrect)
{
Console.WriteLine("The provided password matches the worksheet protection password.");
}
else
{
Console.WriteLine("The provided password does not match the worksheet protection password.");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing VerifyPassword method: {ex.Message}");
}
// Save the workbook
workbook.Save("ProtectionMethodVerifyPasswordWithStringDemo.xlsx");
}
}
}
```
### See Also
* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
