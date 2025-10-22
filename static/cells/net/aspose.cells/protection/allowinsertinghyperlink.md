##Protection.AllowInsertingHyperlink
Protection property. Represents if the insertion of hyperlinks is allowed on a protected worksheet
## Protection.AllowInsertingHyperlink property
Represents if the insertion of hyperlinks is allowed on a protected worksheet
```csharp
public bool AllowInsertingHyperlink { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectionPropertyAllowInsertingHyperlinkDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Protection protection = worksheet.Protection;
protection.AllowInsertingHyperlink = true;
protection.Password = "password123";
// Add a hyperlink to demonstrate the functionality
worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
workbook.Save("AllowInsertingHyperlinkDemo.xlsx");
}
}
}
```
### See Also
* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
