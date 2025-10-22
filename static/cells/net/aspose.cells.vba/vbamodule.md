##Class VbaModule
Aspose.Cells.Vba.VbaModule class. Represents the module in VBA project
## VbaModule class
Represents the module in VBA project.
```csharp
public class VbaModule
```
## Properties
| Name | Description |
| --- | --- |
| [BinaryCodes](../../aspose.cells.vba/vbamodule/binarycodes/) { get; } | Gets and sets the binary codes of module. |
| [Codes](../../aspose.cells.vba/vbamodule/codes/) { get; set; } | Gets and sets the codes of module. |
| [Name](../../aspose.cells.vba/vbamodule/name/) { get; set; } | Gets and sets the name of Module. |
| [Type](../../aspose.cells.vba/vbamodule/type/) { get; } | Gets the type of module. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Vba;
using System;
public class VbaModuleDemo
{
public static void VbaModuleExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Initialize VBA project
VbaProject vbaProject = workbook.VbaProject;
// Add a new module
int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");
// Get the VBA module
VbaModule vbaModule = vbaProject.Modules[index];
// Set the codes for the module
vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";
// Saving the Excel file
workbook.Save("VbaModuleExample.xlsm");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)
