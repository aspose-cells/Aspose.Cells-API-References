##Workbook.VbaProject
Workbook property. Gets the VbaProject in a spreadsheet
## Workbook.VbaProject property
Gets the `VbaProject` in a spreadsheet.
```csharp
public VbaProject VbaProject { get; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class WorkbookPropertyVbaProjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the VBA project (VbaProject is read-only, we can only check if it exists)
if (workbook.VbaProject == null)
{
// Create VBA project by saving as macro-enabled workbook
workbook.Save("temp.xlsm", SaveFormat.Xlsm);
workbook = new Workbook("temp.xlsm");
File.Delete("temp.xlsm");
}
// Add a new module to the VBA project
int moduleIndex = workbook.VbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
// Get the added module and set its code
VbaModule module = workbook.VbaProject.Modules[moduleIndex];
module.Codes = "Sub Test()\r\n    MsgBox \"Hello from VBA!\"\r\nEnd Sub";
// Save the workbook
string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "VbaProjectDemo.xlsm");
workbook.Save(outputPath, SaveFormat.Xlsm);
}
}
}
```
### See Also
* class [VbaProject](../../../aspose.cells.vba/vbaproject/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
