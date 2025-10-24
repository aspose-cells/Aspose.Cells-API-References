##VbaProject.References
VbaProject property. Gets all references of VBA project
## VbaProject.References property
Gets all references of VBA project.
```csharp
public VbaProjectReferenceCollection References { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaProjectPropertyReferencesDemo
{
public static void Run()
{
// Create a workbook (VBA project is created automatically for .xlsm files)
Workbook workbook = new Workbook();
// Access the VBA project references (only available if workbook has VBA project)
if (workbook.VbaProject != null)
{
VbaProjectReferenceCollection references = workbook.VbaProject.References;
// Add different types of references
references.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
references.AddControlRefrernce("MSForms", "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", "", "");
references.AddProjectRefrernce("MyProject", "C:\\Projects\\MyProject.xlam", "..\\MyProject.xlam");
// Display reference count
Console.WriteLine($"Total references: {references.Count}");
}
// Save as macro-enabled workbook
workbook.Save("VbaProjectWithReferences.xlsm", SaveFormat.Xlsm);
}
}
}
```
### See Also
* class [VbaProjectReferenceCollection](../../vbaprojectreferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
