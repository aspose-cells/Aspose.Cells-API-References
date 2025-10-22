##VbaProjectReferenceCollection.Item
VbaProjectReferenceCollection property. Get the reference in the list by the index
## VbaProjectReferenceCollection indexer
Get the reference in the list by the index.
```csharp
public VbaProjectReference this[int i] { get; }
```
| Parameter | Description |
| --- | --- |
| i | The index. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaProjectReferenceCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Initialize VBA project
VbaProject vbaProject = workbook.VbaProject;
// Add references to the VBA project
vbaProject.References.AddRegisteredReference("stdole",
"*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
vbaProject.References.AddControlRefrernce("MSForms",
"*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library",
"twiddledLibid", "extendedLibid");
// Get references collection
VbaProjectReferenceCollection references = vbaProject.References;
// Access references using Item property
VbaProjectReference firstRef = references[0];
VbaProjectReference secondRef = references[1];
Console.WriteLine("First Reference: " + firstRef.Name);
Console.WriteLine("Second Reference: " + secondRef.Name);
// Save the workbook
workbook.Save("VbaProjectReferences.xlsm");
}
}
}
```
### See Also
* class [VbaProjectReference](../../vbaprojectreference/)
* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
