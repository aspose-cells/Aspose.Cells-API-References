##Workbook.ProtectSharedWorkbook
Workbook method. Protects a shared workbook
## Workbook.ProtectSharedWorkbook method
Protects a shared workbook.
```csharp
public void ProtectSharedWorkbook(string password)
```
| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Password to protect the workbook. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodProtectSharedWorkbookWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Protect the shared workbook with password
wb.ProtectSharedWorkbook("abcd");
// Save the protected workbook
wb.Save("ProtectedSharedWorkbook.xlsx");
// Load the protected workbook
Workbook wbProtected = new Workbook("ProtectedSharedWorkbook.xlsx");
// Verify protection status
Console.WriteLine("Workbook is protected: " + wbProtected.Settings.IsProtected);
// Unprotect the workbook
wbProtected.UnprotectSharedWorkbook("abcd");
// Save the unprotected workbook
wbProtected.Save("UnprotectedSharedWorkbook.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
