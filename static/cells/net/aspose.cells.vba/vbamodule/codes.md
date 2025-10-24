##VbaModule.Codes
VbaModule property. Gets and sets the codes of module
## VbaModule.Codes property
Gets and sets the codes of module.
```csharp
public string Codes { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaModulePropertyCodesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a VBA module
int index = workbook.VbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
Aspose.Cells.Vba.VbaModule module = workbook.VbaProject.Modules[index];
// Set initial code
module.Codes = "Sub TestMacro()\n    MsgBox \"Hello World\"\nEnd Sub";
// Modify the code by appending new lines
module.Codes = module.Codes + "\nSub AnotherMacro()\n    MsgBox \"Second Macro\"\nEnd Sub";
// Save the workbook
workbook.Save("VbaModuleDemo.xlsm", SaveFormat.Xlsm);
}
}
}
```
### See Also
* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
