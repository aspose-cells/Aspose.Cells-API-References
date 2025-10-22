##Enum VbaModuleType
Aspose.Cells.Vba.VbaModuleType enum. Represents the type of VBA module
## VbaModuleType enumeration
Represents the type of VBA module.
```csharp
public enum VbaModuleType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Procedural | `0` | Represents a procedural module. |
| Document | `1` | Represents a document module. |
| Class | `2` | Represents a class module. |
| Designer | `3` | Represents a designer module. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Vba;
using System;
public class VbaModuleTypeDemo
{
public static void VbaModuleTypeExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Init VBA project
VbaProject vbaProject = workbook.VbaProject;
// Add a new class module
int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");
// Get the VBA module
VbaModule vbaModule = vbaProject.Modules[index];
// Set codes for the module
vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";
// Save the Excel file
workbook.Save("VbaModuleTypeExample.xlsm");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)
