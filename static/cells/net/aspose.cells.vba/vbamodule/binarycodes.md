##VbaModule.BinaryCodes
VbaModule property. Gets and sets the binary codes of module
## VbaModule.BinaryCodes property
Gets and sets the binary codes of module.
```csharp
public byte[] BinaryCodes { get; }
```
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaModulePropertyBinaryCodesDemo
{
public static void Run()
{
// Load the workbook with VBA project
Workbook workbook = new Workbook("example.xlsm");
// Access the VBA project
VbaProject vbaProject = workbook.VbaProject;
// Get binary codes from the first module
byte[] binaryCodes = vbaProject.Modules[0].BinaryCodes;
// Convert to string using Chinese encoding (936)
string codeContent = Encoding.GetEncoding(936).GetString(binaryCodes);
// Output the content containing Chinese characters
Console.WriteLine("VBA Module Content:");
Console.WriteLine(codeContent);
}
}
}
```
### See Also
* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
