##Protection.AllowFormattingRow
Protection property. Represents if the formatting of rows is allowed on a protected worksheet
## Protection.AllowFormattingRow property
Represents if the formatting of rows is allowed on a protected worksheet
```csharp
public bool AllowFormattingRow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectionPropertyAllowFormattingRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Enable worksheet protection
worksheet.Protect(ProtectionType.All);
// Access protection settings
Protection protection = worksheet.Protection;
// Allow formatting rows while keeping other protections
protection.AllowFormattingRow = true;
// Save the workbook
workbook.Save("Protection_AllowFormattingRow.xlsx");
}
}
}
```
### See Also
* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
