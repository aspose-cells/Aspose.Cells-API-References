##VbaProjectReference.Type
VbaProjectReference property. Gets the type of this reference
## VbaProjectReference.Type property
Gets the type of this reference.
```csharp
public VbaProjectReferenceType Type { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaProjectReferencePropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Initialize VBA project
VbaProject vbaProject = workbook.VbaProject;
// Add a registered reference to the VBA project
vbaProject.References.AddRegisteredReference("stdole",
"*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
// Get the first reference and demonstrate Type property
VbaProjectReference reference = vbaProject.References[0];
Console.WriteLine("Reference Type: " + reference.Type);
Console.WriteLine("Reference Name: " + reference.Name);
Console.WriteLine("Reference Libid: " + reference.Libid);
// Save the workbook
workbook.Save("VbaProjectReferenceTypeExample.xlsm");
}
}
}
```
### See Also
* enum [VbaProjectReferenceType](../../vbaprojectreferencetype/)
* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
