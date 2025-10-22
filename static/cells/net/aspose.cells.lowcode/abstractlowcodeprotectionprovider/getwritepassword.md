##AbstractLowCodeProtectionProvider.GetWritePassword
AbstractLowCodeProtectionProvider method. Gets the password to modify spread sheet file
## AbstractLowCodeProtectionProvider.GetWritePassword method
Gets the password to modify spread sheet file.
```csharp
public virtual string GetWritePassword()
```
### Return Value
Password to modify the spread sheet file. Empty means no protection for modifying the file.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class AbstractLowCodeProtectionProviderMethodGetWritePasswordDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
// Create custom protection provider instance
var protectionProvider = new CustomProtectionProvider();
try
{
// Explicitly call GetWritePassword and display result
string writePassword = protectionProvider.GetWritePassword();
Console.WriteLine($"Retrieved write password: {writePassword}");
// Save workbook - apply write protection directly
workbook.Settings.WriteProtection.Password = writePassword;
workbook.Save("MethodGetWritePasswordDemo.xlsx");
Console.WriteLine("Workbook saved with write protection password.");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetWritePassword method: {ex.Message}");
}
}
}
// Custom protection provider implementation
public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
{
public override string GetWritePassword()
{
return "AsposeTestPassword123!";
}
// Implement other required methods with default returns
public override string GetOpenPassword() => null;
public override string GetWorkbookPassword() => null;
public override ProtectionType GetWorkbookProtectionType() => ProtectionType.None;
public override string GetWorksheetPassword(string sheetName) => null;
public override ProtectionType GetWorksheetProtectionType(string sheetName) => ProtectionType.None;
}
}
```
### See Also
* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
