##VbaProject.Encoding
VbaProject property. Gets and sets the encoding of VBA project
## VbaProject.Encoding property
Gets and sets the encoding of VBA project.
```csharp
public Encoding Encoding { get; set; }
```
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;
using System.Security.Cryptography.X509Certificates;
namespace AsposeCellsExamples
{
public class VbaProjectPropertyEncodingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Initialize VBA project
VbaProject vbaProject = workbook.VbaProject;
// Set VBA project properties including Encoding
vbaProject.Name = "TestVbaProject";
vbaProject.Encoding = Encoding.UTF8;
// Add a module to the VBA project
vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
// Save the workbook with VBA project
workbook.Save("VbaProjectEncodingDemo.xlsm");
}
}
}
```
### See Also
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
