##VbaProjectReference.RelativeLibid
VbaProjectReference property. Gets and sets the referenced VBA projects identifier with an relative path
## VbaProjectReference.RelativeLibid property
Gets and sets the referenced VBA project's identifier with an relative path.
```csharp
public string RelativeLibid { get; set; }
```
### Remarks
Only for project reference.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Vba;
using System;
public class VbaProjectReferencePropertyRelativeLibidDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
VbaProject vbaProject = workbook.VbaProject;
int referenceIndex = vbaProject.References.AddProjectRefrernce("MyReference", null, "..\\lib\\OriginalReference.xlam");
VbaProjectReference reference = vbaProject.References[referenceIndex];
Console.WriteLine("Current RelativeLibid value: " + reference.RelativeLibid);
reference.RelativeLibid = "..\\new_lib\\ModifiedReference.xlam";
Console.WriteLine("Updated RelativeLibid value: " + reference.RelativeLibid);
workbook.Save("PropertyRelativeLibidDemo.xlsx");
}
}
}
```
### See Also
* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
