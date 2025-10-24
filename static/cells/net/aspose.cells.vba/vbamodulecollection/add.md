##VbaModuleCollection.Add
VbaModuleCollection method. Adds module for a worksheet
## Add(Worksheet) {#add_1}
Adds module for a worksheet.
```csharp
public int Add(Worksheet sheet)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | Worksheet | The worksheet |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class VbaModuleCollectionMethodAddWithWorksheetDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a VBA module associated with the worksheet
int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
// Add some VBA code to the module
string vbaCode = "Sub Test()\n    MsgBox \"Hello from VBA!\"\nEnd Sub";
workbook.VbaProject.Modules[moduleIndex].Codes = vbaCode;
// Save the workbook with VBA project
workbook.Save("output.xlsm", SaveFormat.Xlsm);
}
}
}
```
### See Also
* class [Worksheet](../../../aspose.cells/worksheet/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
## Add(VbaModuleType, string) {#add}
Adds module.
```csharp
public int Add(VbaModuleType type, string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | VbaModuleType | The type of module. |
| name | String | The name of module. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaModuleCollectionMethodAddWithVbaModuleTypeStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
VbaProject vbaProject = workbook.VbaProject;
int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
VbaModule module = vbaProject.Modules[index];
module.Codes = "Sub Test()\r\nMsgBox \"Hello World\"\r\nEnd Sub";
workbook.Save("VbaModuleAddExample.xlsm");
}
}
}
```
### See Also
* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
