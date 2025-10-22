##VbaModule.Type
VbaModule property. Gets the type of module
## VbaModule.Type property
Gets the type of module.
```csharp
public VbaModuleType Type { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaModulePropertyTypeDemo
{
public static void Run()
{
// Create workbook with sample macro-enabled file
Workbook wb = new Workbook("example.xlsm");
// Access VBA project and modules
VbaProject vbaProject = wb.VbaProject;
VbaModuleCollection modules = vbaProject.Modules;
// Display module types and names
for (int i = 0; i < modules.Count; i++)
{
Console.WriteLine($"Module Name: {modules[i].Name}");
Console.WriteLine($"Module Type: {modules[i].Type}");
Console.WriteLine();
}
wb.Save("output.xlsm");
}
}
}
```
### See Also
* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
