##AbstractLowCodeProtectionProvider.GetWorksheetPassword
AbstractLowCodeProtectionProvider method. Gets the password to protect the specified worksheet
## AbstractLowCodeProtectionProvider.GetWorksheetPassword method
Gets the password to protect the specified worksheet.
```csharp
public virtual string GetWorksheetPassword(string sheetName)
```
### Return Value
Password to protect the specified worksheet.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class AbstractLowCodeProtectionProviderMethodGetWorksheetPasswordWithStringDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
string sheetName = worksheet.Name;
// Create custom protection provider instance
var provider = new CustomProtectionProvider();
try
{
// Call GetWorksheetPassword with worksheet name
string password = provider.GetWorksheetPassword(sheetName);
// Apply protection to worksheet using retrieved password
worksheet.Protect(ProtectionType.All, password, null);
Console.WriteLine($"Protected worksheet '{sheetName}' with password: {password}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetWorksheetPassword: {ex.Message}");
}
// Save the protected workbook
workbook.Save("WorksheetPasswordDemo.xlsx");
}
}
// Custom implementation returning password based on sheet name
public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
{
public new string GetWorksheetPassword(string sheetName)
{
// Simple password generation logic for demonstration
return $"pw_{sheetName}";
}
}
}
```
### See Also
* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
