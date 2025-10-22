##VbaProjectReferenceCollection.AddRegisteredReference
VbaProjectReferenceCollection method. Add a reference to an Automation type library
## VbaProjectReferenceCollection.AddRegisteredReference method
Add a reference to an Automation type library.
```csharp
public int AddRegisteredReference(string name, string libid)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of reference. |
| libid | String | The identifier of an Automation type library. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaProjectReferenceCollectionMethodAddRegisteredReferenceWithStringStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the VBA project
VbaProject vbaProject = workbook.VbaProject;
// Add a registered reference to stdole
vbaProject.References.AddRegisteredReference(
"stdole",
"*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
// Save the workbook
workbook.Save("output.xlsm");
}
}
}
```
### See Also
* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
