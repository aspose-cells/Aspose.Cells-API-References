##VbaProjectReference.Name
VbaProjectReference property. Gets and sets the name of the reference
## VbaProjectReference.Name property
Gets and sets the name of the reference.
```csharp
public string Name { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaProjectReferencePropertyNameDemo
{
public static void Run()
{
// Create a workbook (VBA project is automatically created for .xlsm files)
Workbook workbook = new Workbook(FileFormatType.Xlsm);
// Add a reference to the VBA project
string referenceName = "MyReference";
string referencePath = @"C:\Temp\MyLibrary.dll";
workbook.VbaProject.References.AddRegisteredReference(referenceName, referencePath);
// Access and verify the reference by Name property
VbaProjectReferenceCollection references = workbook.VbaProject.References;
for (int i = 0; i < references.Count; i++)
{
if (references[i].Name.Equals(referenceName))
{
Console.WriteLine($"Found reference: {references[i].Name}");
break;
}
}
// Save the workbook
workbook.Save("VbaProjectReferenceDemo.xlsm");
}
}
}
```
### See Also
* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
