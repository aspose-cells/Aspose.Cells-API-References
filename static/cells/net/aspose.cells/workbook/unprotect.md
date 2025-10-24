##Workbook.Unprotect
Workbook method. Unprotects a workbook
## Workbook.Unprotect method
Unprotects a workbook.
```csharp
public void Unprotect(string password)
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
public class WorkbookMethodUnprotectWithStringDemo
{
public static void Run()
{
// Create a workbook with protection
Workbook workbook = new Workbook();
workbook.Protect(ProtectionType.All, "book");
// Unprotect the workbook with correct password
workbook.Unprotect("book");
// Save the unprotected workbook
workbook.Save("unprotected_workbook.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
