##WorkbookSettings.IsProtected
WorkbookSettings property. Gets a value that indicates whether the structure or window of the Workbook is protected
## WorkbookSettings.IsProtected property
Gets a value that indicates whether the structure or window of the Workbook is protected.
```csharp
public bool IsProtected { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyIsProtectedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access workbook settings
WorkbookSettings settings = workbook.Settings;
// Check if workbook is protected
Console.WriteLine("Workbook is protected: " + settings.IsProtected);
// Protect the workbook with a password
settings.Password = "password123";
// Verify protection status
Console.WriteLine("Workbook is protected: " + settings.IsProtected);
// Save the protected workbook
workbook.Save("ProtectedWorkbook.xlsx", SaveFormat.Xlsx);
// Open the protected workbook
Workbook protectedWorkbook = new Workbook("ProtectedWorkbook.xlsx");
// Check protection status of loaded workbook
Console.WriteLine("Loaded workbook is protected: " + protectedWorkbook.Settings.IsProtected);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
