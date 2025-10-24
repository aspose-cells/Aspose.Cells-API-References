##VbaProject.Modules
VbaProject property. Gets all VbaModule objects
## VbaProject.Modules property
Gets all [`VbaModule`](../../vbamodule/) objects.
```csharp
public VbaModuleCollection Modules { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaProjectPropertyModulesDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
VbaProject vbaProject = workbook.VbaProject;
// Add a new module and get it using Modules property
int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
VbaModule module = vbaProject.Modules[index];
// Add code to the module
module.Codes = "Sub Test()\r\n    MsgBox \"Module demonstration\"\r\nEnd Sub";
// Save with macro-enabled format
workbook.Save("VbaModulesDemo.xlsm", SaveFormat.Xlsm);
}
}
}
```
### See Also
* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
