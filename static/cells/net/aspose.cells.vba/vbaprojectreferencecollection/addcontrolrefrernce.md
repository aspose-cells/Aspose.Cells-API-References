##VbaProjectReferenceCollection.AddControlRefrernce
VbaProjectReferenceCollection method. Add a reference to a twiddled type library and its extended type library
## VbaProjectReferenceCollection.AddControlRefrernce method
Add a reference to a twiddled type library and its extended type library.
```csharp
public int AddControlRefrernce(string name, string libid, string twiddledlibid,
string extendedLibid)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of reference. |
| libid | String | The identifier of an Automation type library. |
| twiddledlibid | String | The identifier of a twiddled type library |
| extendedLibid | String | The identifier of an extended type library |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaProjectReferenceCollectionMethodAddControlRefrernceWithStringStringStringStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
VbaProject vbaProject = workbook.VbaProject;
// Add control reference with all string parameters
vbaProject.References.AddControlRefrernce(
"MSForms",
"*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library",
"twiddledLibid",
"extendedLibid");
Console.WriteLine("Control reference added successfully. Total references: " + vbaProject.References.Count);
workbook.Save("VbaProjectWithControlReference.xlsm");
}
}
}
```
### See Also
* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
