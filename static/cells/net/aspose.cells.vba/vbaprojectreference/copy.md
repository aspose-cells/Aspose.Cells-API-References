##VbaProjectReference.Copy
VbaProjectReference method.
## VbaProjectReference.Copy method
```csharp
public void Copy(VbaProjectReference source)
```
| Parameter | Type | Description |
| --- | --- | --- |
| source | VbaProjectReference |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Vba;
using System;
public class VbaProjectReferenceMethodCopyWithVbaProjectReferenceDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
VbaProject vbaProject = workbook.VbaProject;
int sourceIndex = vbaProject.References.AddRegisteredReference("SourceLib", "LIBID:12345678-1234-1234-1234-123456789ABC");
VbaProjectReference sourceRef = vbaProject.References[sourceIndex];
sourceRef.Name = "SourceReference";
sourceRef.Twiddledlibid = "Twiddled123";
sourceRef.ExtendedLibid = "Extended456";
int targetIndex = vbaProject.References.AddRegisteredReference("TargetLib", "LIBID:00000000-0000-0000-0000-000000000000");
VbaProjectReference targetRef = vbaProject.References[targetIndex];
targetRef.Name = "OriginalTargetName";
try
{
Console.WriteLine("Before Copy - Target Reference:");
Console.WriteLine($"Name: {targetRef.Name}, Libid: {targetRef.Libid}");
targetRef.Copy(sourceRef);
Console.WriteLine("\nAfter Copy - Target Reference:");
Console.WriteLine($"Name: {targetRef.Name}, Libid: {targetRef.Libid}");
Console.WriteLine($"Twiddledlibid: {targetRef.Twiddledlibid}, ExtendedLibid: {targetRef.ExtendedLibid}");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
workbook.Save("VbaProjectReferenceCopyDemo.xlsx");
}
}
}
```
### See Also
* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
