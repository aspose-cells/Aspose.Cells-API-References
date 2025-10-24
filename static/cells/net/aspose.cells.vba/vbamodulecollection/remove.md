##VbaModuleCollection.Remove
VbaModuleCollection method. Removes module for a worksheet
## Remove(Worksheet) {#remove}
Removes module for a worksheet.
```csharp
public void Remove(Worksheet sheet)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | Worksheet | The worksheet |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Vba;
using System;
public class VbaModuleCollectionMethodRemoveWithWorksheetDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a VBA module to the worksheet
int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
// Get the VBA module collection
VbaModuleCollection modules = workbook.VbaProject.Modules;
try
{
// Call the Remove method with the worksheet parameter
modules.Remove(worksheet);
Console.WriteLine("VBA module removed successfully for the specified worksheet.");
// Verify the module was removed
if (modules.Count == 0)
{
Console.WriteLine("No VBA modules remain in the collection.");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Remove method: {ex.Message}");
}
// Save the result
workbook.Save("VbaModuleRemoveWithWorksheetDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../../../aspose.cells/worksheet/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
## Remove(string) {#remove_1}
Remove the module by the name
```csharp
public void Remove(string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String |  |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaModuleCollectionMethodRemoveWithStringDemo
{
public static void Run()
{
// Create a workbook with macro
Workbook workbook = new Workbook();
// Access VBA project
VbaProject vbaProject = workbook.VbaProject;
// Add a new module
int index = vbaProject.Modules.Add(VbaModuleType.Procedural, "TestModule");
// Add some code to the module
vbaProject.Modules[index].Codes = "Sub Test()\r\nMsgBox \"Hello World\"\r\nEnd Sub";
// Save the workbook
workbook.Save("output_with_module.xlsm");
// Remove the module by name
vbaProject.Modules.Remove("TestModule");
// Save the workbook after removal
workbook.Save("output_after_removal.xlsm");
}
}
}
```
### See Also
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
