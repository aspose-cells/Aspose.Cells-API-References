##VbaProject.Protect
VbaProject method. Protects or unprotects this VBA project
## VbaProject.Protect method
Protects or unprotects this VBA project.
```csharp
public void Protect(bool islockedForViewing, string password)
```
| Parameter | Type | Description |
| --- | --- | --- |
| islockedForViewing | Boolean | indicates whether locks project for viewing. |
| password | String | If the value is null, unprotects this VBA project, otherwise projects the this VBA project. |
### Remarks
If islockedForViewing is true, the password could not be null.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class VbaProjectMethodProtectWithBooleanStringDemo
{
public static void Run()
{
// Create a workbook with VBA project
Workbook workbook = new Workbook();
workbook.VbaProject.Protect(false, "password123");
// Save the workbook
workbook.Save("output.xlsm", SaveFormat.Xlsm);
}
}
}
```
### See Also
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
