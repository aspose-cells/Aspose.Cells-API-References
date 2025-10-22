##Worksheet.Protection
Worksheet property. Represents the various types of protection options available for a worksheet. Supports advanced protection options in ExcelXP and above version
## Worksheet.Protection property
Represents the various types of protection options available for a worksheet. Supports advanced protection options in ExcelXP and above version.
```csharp
public Protection Protection { get; }
```
### Remarks
This property can protect worksheet in all versions of Excel file and support advanced protection options in ExcelXP and above version.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyProtectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Access protection properties
Protection protection = sheet.Protection;
// Set protection properties
protection.AllowEditingObject = false;
protection.AllowEditingScenario = false;
// Protect the worksheet (using Protect method instead of setting IsProtectedWithPassword directly)
sheet.Protect(ProtectionType.All, "password123", null);
// Save the workbook
workbook.Save("WorksheetProtectionDemo.xlsx");
// Verify protection settings
Console.WriteLine("AllowEditingObject: " + protection.AllowEditingObject);
Console.WriteLine("AllowEditingScenario: " + protection.AllowEditingScenario);
}
}
}
```
### See Also
* class [Protection](../../protection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
