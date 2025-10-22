##VbaModuleCollection.Item
VbaModuleCollection property. Gets VbaModule in the list by the index
## VbaModuleCollection indexer (1 of 2)
Gets [`VbaModule`](../../vbamodule/) in the list by the index.
```csharp
public VbaModule this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaModuleCollectionPropertyItemDemo1
{
public static void Run()
{
// Create a new workbook with VBA project
Workbook workbook = new Workbook("sample.xlsm");
// Get existing VBA project (VbaProject is read-only)
VbaProject vbaProject = workbook.VbaProject;
// Add a module to the VBA project
int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
// Access the module using Item property
VbaModule module = vbaProject.Modules[index];
// Add some VBA code to the module
module.Codes = "Sub TestMacro()\n    MsgBox \"Hello from VBA!\"\nEnd Sub";
// Save the workbook
workbook.Save("VbaModuleDemo.xlsm", SaveFormat.Xlsm);
}
}
}
```
### See Also
* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
## VbaModuleCollection indexer (2 of 2)
Gets [`VbaModule`](../../vbamodule/) in the list by the name.
```csharp
public VbaModule this[string name] { get; }
```
| Parameter | Description |
| --- | --- |
| name | The name of module. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaModuleCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add VBA module to the workbook
int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
// Access the module using Item property by name
VbaModule module = workbook.VbaProject.Modules[worksheet.CodeName];
// Set VBA code
module.Codes = "Sub Test()\r\n    MsgBox \"Hello World!\"\r\nEnd Sub";
// Save the workbook
workbook.Save("output.xlsm", SaveFormat.Xlsm);
// Verify by loading back
Workbook verifyWorkbook = new Workbook("output.xlsm");
VbaModule verifyModule = verifyWorkbook.VbaProject.Modules[worksheet.CodeName];
Console.WriteLine("VBA Code in saved file:");
Console.WriteLine(verifyModule.Codes);
}
}
}
```
### See Also
* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
