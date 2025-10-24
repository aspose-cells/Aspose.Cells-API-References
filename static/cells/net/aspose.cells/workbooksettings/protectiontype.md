##WorkbookSettings.ProtectionType
WorkbookSettings property. Gets the protection type of the workbook
## WorkbookSettings.ProtectionType property
Gets the protection type of the workbook.
```csharp
public ProtectionType ProtectionType { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyProtectionTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Protect the workbook with Windows protection type
workbook.Protect(ProtectionType.Windows, "password123");
// Demonstrate ProtectionType property
Console.WriteLine("Workbook protection type: " + workbook.Settings.ProtectionType);
// Save the workbook
workbook.Save("ProtectedWorkbook.xlsx");
// Load the saved workbook to verify protection type persists
Workbook loadedWorkbook = new Workbook("ProtectedWorkbook.xlsx");
Console.WriteLine("Loaded workbook protection type: " + loadedWorkbook.Settings.ProtectionType);
}
}
}
```
### See Also
* enum [ProtectionType](../../protectiontype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
