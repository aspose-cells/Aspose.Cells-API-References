##Protection.AllowEditingContent
Protection property. Represents if the user is allowed to edit contents of locked cells on a protected worksheet
## Protection.AllowEditingContent property
Represents if the user is allowed to edit contents of locked cells on a protected worksheet.
```csharp
public bool AllowEditingContent { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectionPropertyAllowEditingContentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Protect the worksheet with a password
worksheet.Protect(ProtectionType.All, "password", null);
// Check and display the AllowEditingContent property
Console.WriteLine("AllowEditingContent before setting: " + worksheet.Protection.AllowEditingContent);
// Modify the AllowEditingContent property
worksheet.Protection.AllowEditingContent = true;
// Check and display the updated property
Console.WriteLine("AllowEditingContent after setting: " + worksheet.Protection.AllowEditingContent);
// Save the workbook
workbook.Save("ProtectionPropertyAllowEditingContentDemo.xlsx");
}
}
}
```
### See Also
* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
