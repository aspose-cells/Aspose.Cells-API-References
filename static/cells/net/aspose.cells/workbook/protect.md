##Workbook.Protect
Workbook method. Protects a workbook
## Workbook.Protect method
Protects a workbook.
```csharp
public void Protect(ProtectionType protectionType, string password)
```
| Parameter | Type | Description |
| --- | --- | --- |
| protectionType | ProtectionType | Protection type. |
| password | String | Password to protect the workbook. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodProtectWithProtectionTypeStringDemo
{
public static void Run()
{
Workbook wbk = new Workbook();
wbk.Protect(ProtectionType.Structure, "password123");
wbk.Save("protected_workbook.xlsx", SaveFormat.Xlsx);
wbk.Dispose();
}
}
}
```
### See Also
* enum [ProtectionType](../../protectiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
