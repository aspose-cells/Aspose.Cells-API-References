##VbaProject.IsSigned
VbaProject property. Indicates whether VBAcode is signed or not
## VbaProject.IsSigned property
Indicates whether VBAcode is signed or not.
```csharp
public bool IsSigned { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class VbaProjectPropertyIsSignedDemo
{
public static void Run()
{
// Load a sample Excel file with VBA project
Workbook workbook = new Workbook("example.xlsm");
// Check if the VBA project is signed
if (workbook.VbaProject.IsSigned)
{
Console.WriteLine("VBA project is signed.");
Console.WriteLine("Signature is valid: " + workbook.VbaProject.IsValidSigned);
}
else
{
Console.WriteLine("VBA project is not signed.");
}
}
}
}
```
### See Also
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
