##WriteProtection.ValidatePassword
WriteProtection method. Returns true if the specified password is the same as the writeprotection password the file was protected with
## WriteProtection.ValidatePassword method
Returns true if the specified password is the same as the write-protection password the file was protected with.
```csharp
public bool ValidatePassword(string password)
```
| Parameter | Type | Description |
| --- | --- | --- |
| password | String | The specified password. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WriteProtectionMethodValidatePasswordWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set write protection password
workbook.Settings.WriteProtection.Password = "1234";
// Validate password
Console.WriteLine("Password '1234' is valid: " +
workbook.Settings.WriteProtection.ValidatePassword("1234"));
Console.WriteLine("Password 'wrong' is valid: " +
workbook.Settings.WriteProtection.ValidatePassword("wrong"));
}
}
}
```
### See Also
* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
