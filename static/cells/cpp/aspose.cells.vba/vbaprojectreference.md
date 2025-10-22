##Aspose::Cells::Vba::VbaProjectReference class
'Aspose::Cells::Vba::VbaProjectReference class. Represents the reference of VBA project in C++.'
## VbaProjectReference class
Represents the reference of VBA project.
```cpp
class VbaProjectReference
```
## Methods
| Method | Description |
| --- | --- |
| [Copy(const VbaProjectReference\& source)](./copy/) |  |
| [GetExtendedLibid()](./getextendedlibid/) | Gets and sets the extended Libid of the reference. |
| [GetLibid()](./getlibid/) | Gets and sets the Libid of the reference. |
| [GetName()](./getname/) | Gets and sets the name of the reference. |
| [GetRelativeLibid()](./getrelativelibid/) | Gets and sets the referenced VBA project's identifier with an relative path. |
| [GetTwiddledlibid()](./gettwiddledlibid/) | Gets and sets the twiddled Libid of the reference. |
| [GetType()](./gettype/) | Gets the type of this reference. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const VbaProjectReference\& src)](./operator_asm/) | operator= |
| [SetExtendedLibid(const U16String\& value)](./setextendedlibid/) | Gets and sets the extended Libid of the reference. |
| [SetExtendedLibid(const char16_t* value)](./setextendedlibid/) | Gets and sets the extended Libid of the reference. |
| [SetLibid(const U16String\& value)](./setlibid/) | Gets and sets the Libid of the reference. |
| [SetLibid(const char16_t* value)](./setlibid/) | Gets and sets the Libid of the reference. |
| [SetName(const U16String\& value)](./setname/) | Gets and sets the name of the reference. |
| [SetName(const char16_t* value)](./setname/) | Gets and sets the name of the reference. |
| [SetRelativeLibid(const U16String\& value)](./setrelativelibid/) | Gets and sets the referenced VBA project's identifier with an relative path. |
| [SetRelativeLibid(const char16_t* value)](./setrelativelibid/) | Gets and sets the referenced VBA project's identifier with an relative path. |
| [SetTwiddledlibid(const U16String\& value)](./settwiddledlibid/) | Gets and sets the twiddled Libid of the reference. |
| [SetTwiddledlibid(const char16_t* value)](./settwiddledlibid/) | Gets and sets the twiddled Libid of the reference. |
| [VbaProjectReference(VbaProjectReference_Impl* impl)](./vbaprojectreference/) | Constructs from an implementation object. |
| [VbaProjectReference(const VbaProjectReference\& src)](./vbaprojectreference/) | Copy constructor. |
| [~VbaProjectReference()](./~vbaprojectreference/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
// Init VBA project.
VbaProject vbaProject = workbook.GetVbaProject();
// Add vba project reference
vbaProject.GetReferences().AddRegisteredReference(u"stdole", u"*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
//Saving the Excel file
workbook.Save(u"book1.xlsm");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Vba](../)
* Library [Aspose.Cells for C++](../../)
