##VbaProject.IsProtected
VbaProject property. Indicates whether this VBA project is protected
## VbaProject.IsProtected property
Indicates whether this VBA project is protected.
```csharp
public bool IsProtected { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaProjectPropertyIsProtectedDemo
{
public static void Run()
{
// Load a sample Excel file with unprotected VBA project
Workbook wb = new Workbook("load.xlsm");
VbaProject vbaProject = wb.VbaProject;
Console.WriteLine("Is VBA Project Protected (load.xlsm): " + vbaProject.IsProtected);
Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);
// Load a sample Excel file with protected VBA project
wb = new Workbook("load_protected.xlsm");
vbaProject = wb.VbaProject;
Console.WriteLine("Is VBA Project Protected (load_protected.xlsm): " + vbaProject.IsProtected);
Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);
// Load a sample Excel file with protected and locked VBA project
wb = new Workbook("load_protected_lockedForView.xlsm");
vbaProject = wb.VbaProject;
Console.WriteLine("Is VBA Project Protected (load_protected_lockedForView.xlsm): " + vbaProject.IsProtected);
Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);
}
}
}
```
### See Also
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
