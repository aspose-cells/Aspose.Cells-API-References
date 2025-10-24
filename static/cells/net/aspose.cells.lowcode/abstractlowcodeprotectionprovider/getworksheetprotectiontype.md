##AbstractLowCodeProtectionProvider.GetWorksheetProtectionType
AbstractLowCodeProtectionProvider method. Gets the protection type to protect the specified worksheet
## AbstractLowCodeProtectionProvider.GetWorksheetProtectionType method
Gets the protection type to protect the specified worksheet.
```csharp
public virtual ProtectionType GetWorksheetProtectionType(string sheetName)
```
### Return Value
Protection type to protect the specified worksheet. None means no protection for the worksheet.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class AbstractLowCodeProtectionProviderMethodGetWorksheetProtectionTypeWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets.Add("newSheet");
string name = worksheet.Name;
var protectionProvider = new CustomProtectionProvider();
try
{
worksheet.Protect(protectionProvider.GetWorksheetProtectionType(name), protectionProvider.GetWorksheetPassword(name), "");
// Display the result
Console.WriteLine($"Worksheet '{name}' protection type: {protectionProvider.GetWorksheetProtectionType(name)}");
}
catch (Exception ex)
{
Console.WriteLine($"Error retrieving protection type: {ex.Message}");
}
// Save the workbook
workbook.Save("GetWorksheetProtectionTypeDemo.xlsx");
}
private class CustomProtectionProvider : AbstractLowCodeProtectionProvider
{
public override ProtectionType GetWorksheetProtectionType(string sheetName)
{
return ProtectionType.Structure;
}
public override string GetWorksheetPassword(string sheetName)
{
return $"aspose123_{sheetName}";
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
