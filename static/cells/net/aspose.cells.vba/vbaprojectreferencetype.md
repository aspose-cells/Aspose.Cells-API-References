##Enum VbaProjectReferenceType
Aspose.Cells.Vba.VbaProjectReferenceType enum. Represents the type of VBA project reference
## VbaProjectReferenceType enumeration
Represents the type of VBA project reference.
```csharp
public enum VbaProjectReferenceType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Registered | `0` | Specifies a reference to an Automation type library. |
| Control | `1` | Specifies a reference to a twiddled type library and its extended type library. |
| Project | `2` | Specifies a reference to an external VBA project. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Vba;
using System;
public class VbaProjectReferenceTypeDemo
{
public static void VbaProjectReferenceTypeExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Init VBA project
VbaProject vbaProject = workbook.VbaProject;
// Add VBA project reference
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
// Saving the Excel file
workbook.Save("VbaProjectReferenceTypeExample.xlsm");
// Demonstrating the use of VbaProjectReferenceType enum
VbaProjectReference reference = vbaProject.References[0];
Console.WriteLine("Reference Type: " + reference.Type);
Console.WriteLine("Reference Name: " + reference.Name);
Console.WriteLine("Reference Libid: " + reference.Libid);
}
}
}
```
### See Also
* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)
