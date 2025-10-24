##VbaProjectReferenceCollection.AddProjectRefrernce
VbaProjectReferenceCollection method. Adds a reference to an external VBA project
## VbaProjectReferenceCollection.AddProjectRefrernce method
Adds a reference to an external VBA project.
```csharp
public int AddProjectRefrernce(string name, string absoluteLibid, string relativeLibid)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of reference. |
| absoluteLibid | String | The referenced VBA project's identifier with an absolute path. |
| relativeLibid | String | The referenced VBA project's identifier with an relative path. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaProjectReferenceCollectionMethodAddProjectRefrernceWithStringStringStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Initialize VBA project
VbaProject vbaProject = workbook.VbaProject;
// Add a project reference with absolute and relative libids
vbaProject.References.AddProjectRefrernce("MyProject", "absoluteLibid", "relativeLibid");
// Display reference count
Console.WriteLine("Total References: " + vbaProject.References.Count);
// Save the workbook
workbook.Save("VbaProjectReferenceExample.xlsm");
}
}
}
```
### See Also
* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
