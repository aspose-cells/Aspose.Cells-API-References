##AbstractLowCodeProtectionProvider.GetWorkbookPassword
AbstractLowCodeProtectionProvider method. Gets the password to protect the workbook with specified protection type
## AbstractLowCodeProtectionProvider.GetWorkbookPassword method
Gets the password to protect the workbook with specified protection type.
```csharp
public virtual string GetWorkbookPassword()
```
### Return Value
Password to protect the workbook.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class AbstractLowCodeProtectionProviderMethodGetWorkbookPasswordDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
var provider = new DemoProtectionProvider();
try
{
string password = provider.GetWorkbookPassword();
ProtectionType protectionType = provider.GetWorkbookProtectionType();
workbook.Protect(protectionType, password);
Console.WriteLine($"Workbook protected with password: {password}");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
workbook.Save("ProtectedWorkbook.xlsx");
}
}
public class DemoProtectionProvider : AbstractLowCodeProtectionProvider
{
public override string GetWorkbookPassword()
{
return "Aspose1234!";
}
public override ProtectionType GetWorkbookProtectionType()
{
return ProtectionType.Structure;
}
}
}
```
### See Also
* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
