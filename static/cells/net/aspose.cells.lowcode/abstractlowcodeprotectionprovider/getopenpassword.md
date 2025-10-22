##AbstractLowCodeProtectionProvider.GetOpenPassword
AbstractLowCodeProtectionProvider method. Gets the password to open spread sheet file
## AbstractLowCodeProtectionProvider.GetOpenPassword method
Gets the password to open spread sheet file.
```csharp
public virtual string GetOpenPassword()
```
### Return Value
Password to open spread sheet file. Empty means no protection for openning the filel.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class AbstractLowCodeProtectionProviderMethodGetOpenPasswordDemo
{
public static void Run()
{
try
{
// Create a protection provider instance
var protectionProvider = new DemoProtectionProvider();
// Call GetOpenPassword method to retrieve the password
string password = protectionProvider.GetOpenPassword();
// Create a new workbook and apply the password
Workbook workbook = new Workbook("sample.xlsx");
workbook.Settings.Password = password;
// Save the password-protected workbook
workbook.Save("MethodGetOpenPasswordDemo.xlsx");
Console.WriteLine($"Workbook protected with open password: {password}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing demo: {ex.Message}");
}
}
}
public class DemoProtectionProvider : AbstractLowCodeProtectionProvider
{
public override string GetOpenPassword()
{
return "AsposeDemo123!";
}
}
}
```
### See Also
* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
