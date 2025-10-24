##Worksheet.IsProtected
Worksheet property. Indicates if the worksheet is protected
## Worksheet.IsProtected property
Indicates if the worksheet is protected.
```csharp
public bool IsProtected { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyIsProtectedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Protect the workbook and first worksheet
workbook.Protect(ProtectionType.All, "password");
workbook.Worksheets[0].Protect(ProtectionType.All, "password", null);
// Check if the worksheet is protected
bool isProtected = workbook.Worksheets[0].IsProtected;
Console.WriteLine($"Worksheet is protected: {isProtected}");
// Save the workbook
workbook.Save("protected_worksheet.xlsx");
// Load the saved workbook and verify protection
Workbook loadedWorkbook = new Workbook("protected_worksheet.xlsx");
Console.WriteLine($"Loaded worksheet is protected: {loadedWorkbook.Worksheets[0].IsProtected}");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
