##AbstractLowCodeProtectionProvider.GetWorkbookProtectionType
AbstractLowCodeProtectionProvider method. Gets the protection type to protect the workbook
## AbstractLowCodeProtectionProvider.GetWorkbookProtectionType method
Gets the protection type to protect the workbook.
```csharp
public virtual ProtectionType GetWorkbookProtectionType()
```
### Return Value
Protection type to protect the workbook. None means no protection for the workbook.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class AbstractLowCodeProtectionProviderMethodGetWorkbookProtectionTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
var provider = new CustomProtectionProvider();
try
{
workbook.Protect(provider.GetWorkbookProtectionType(), provider.GetWorkbookPassword());
ProtectionType protectionType = provider.GetWorkbookProtectionType();
Console.WriteLine($"Workbook protection type: {protectionType}");
Console.WriteLine($"Protection status: {workbook.Settings.IsProtected}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetWorkbookProtectionType: {ex.Message}");
}
workbook.Save("WorkbookProtectionDemo.xlsx");
}
private class CustomProtectionProvider : AbstractLowCodeProtectionProvider
{
public override ProtectionType GetWorkbookProtectionType()
{
return ProtectionType.Structure;
}
public override string GetWorkbookPassword()
{
return "aspose123";
}
}
}
}
```
### See Also
* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
