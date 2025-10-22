##Class VbaProjectReference
Aspose.Cells.Vba.VbaProjectReference class. Represents the reference of VBA project
## VbaProjectReference class
Represents the reference of VBA project.
```csharp
public class VbaProjectReference
```
## Properties
| Name | Description |
| --- | --- |
| [ExtendedLibid](../../aspose.cells.vba/vbaprojectreference/extendedlibid/) { get; set; } | Gets and sets the extended Libid of the reference. |
| [Libid](../../aspose.cells.vba/vbaprojectreference/libid/) { get; set; } | Gets and sets the Libid of the reference. |
| [Name](../../aspose.cells.vba/vbaprojectreference/name/) { get; set; } | Gets and sets the name of the reference. |
| [RelativeLibid](../../aspose.cells.vba/vbaprojectreference/relativelibid/) { get; set; } | Gets and sets the referenced VBA project's identifier with an relative path. |
| [Twiddledlibid](../../aspose.cells.vba/vbaprojectreference/twiddledlibid/) { get; set; } | Gets and sets the twiddled Libid of the reference. |
| [Type](../../aspose.cells.vba/vbaprojectreference/type/) { get; } | Gets the type of this reference. |
## Methods
| Name | Description |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaprojectreference/copy/)(VbaProjectReference) |  |
### Examples
```csharp
[C#]
//Instantiating a Workbook object
Workbook workbook = new Workbook();
// Init VBA project.
VbaProject vbaProject = workbook.VbaProject;
// Add vba project reference
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
//Saving the Excel file
workbook.Save("book1.xlsm");
[Visual Basic]
'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Init VBA project.
Dim vbaProject as VbaProject  = workbook.VbaProject
'Add vba project reference
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
'Saving the Excel file
workbook.Save("book1.xlsm")
```
### See Also
* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)
