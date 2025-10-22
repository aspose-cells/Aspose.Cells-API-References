##Workbook.UnprotectSharedWorkbook
Workbook method. Unprotects a shared workbook
## Workbook.UnprotectSharedWorkbook method
Unprotects a shared workbook.
```csharp
public void UnprotectSharedWorkbook(string password)
```
| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Password to unprotect the workbook. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodUnprotectSharedWorkbookWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Protect the shared workbook with password
wb.ProtectSharedWorkbook("abcd");
// Save the protected workbook
wb.Save("ProtectedSharedWorkbook.xlsx");
// Reopen the workbook
wb = new Workbook("ProtectedSharedWorkbook.xlsx");
// Unprotect the shared workbook with password
wb.UnprotectSharedWorkbook("abcd");
// Save the unprotected workbook
wb.Save("UnprotectedSharedWorkbook.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
