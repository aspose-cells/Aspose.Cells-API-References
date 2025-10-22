##VbaProjectReference.Libid
VbaProjectReference property. Gets and sets the Libid of the reference
## VbaProjectReference.Libid property
Gets and sets the Libid of the reference.
```csharp
public string Libid { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaProjectReferencePropertyLibidDemo
{
public static void Run()
{
// Create a new workbook
Workbook targetWorkbook = new Workbook();
// Load source workbook with VBA project
Workbook sourceWorkbook = new Workbook("source.xlsm");
// Clear existing references in target
targetWorkbook.VbaProject.References.Clear();
// Copy references from source to target
foreach (VbaProjectReference reference in sourceWorkbook.VbaProject.References)
{
if (reference.Type == VbaProjectReferenceType.Registered)
{
// Demonstrate Libid property usage
targetWorkbook.VbaProject.References.AddRegisteredReference(reference.Name, reference.Libid);
}
else if (reference.Type == VbaProjectReferenceType.Control)
{
targetWorkbook.VbaProject.References.AddControlRefrernce(
reference.Name,
reference.Libid,
reference.Twiddledlibid,
reference.ExtendedLibid);
}
}
// Save the result
targetWorkbook.Save("output.xlsm");
}
}
}
```
### See Also
* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
