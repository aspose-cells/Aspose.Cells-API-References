##VbaProject.IsValidSigned
VbaProject property. Indicates whether the signature of VBA project is valid or not
## VbaProject.IsValidSigned property
Indicates whether the signature of VBA project is valid or not.
```csharp
public bool IsValidSigned { get; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class VbaProjectPropertyIsValidSignedDemo
{
public static void Run()
{
// Load a sample workbook with signed VBA project
Workbook wb = new Workbook("example.xlsm");
// Check if VBA project is signed and the signature is valid
Console.WriteLine("Is VBA Project Signed: " + wb.VbaProject.IsSigned);
Console.WriteLine("Is Signature Valid: " + wb.VbaProject.IsValidSigned);
// Save and reload to verify signature persists
MemoryStream ms = new MemoryStream();
wb.Save(ms, SaveFormat.Excel97To2003);
Workbook validateWb = new Workbook(ms);
Console.WriteLine("After Reload - Is VBA Project Signed: " + validateWb.VbaProject.IsSigned);
Console.WriteLine("After Reload - Is Signature Valid: " + validateWb.VbaProject.IsValidSigned);
}
}
}
```
### See Also
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
