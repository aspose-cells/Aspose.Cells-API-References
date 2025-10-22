##Aspose::Cells::Vba::VbaProjectReferenceCollection class
'Aspose::Cells::Vba::VbaProjectReferenceCollection class. Represents all references of VBA project in C++.'
## VbaProjectReferenceCollection class
Represents all references of VBA project.
```cpp
class VbaProjectReferenceCollection
```
## Methods
| Method | Description |
| --- | --- |
| [AddControlRefrernce(const U16String\& name, const U16String\& libid, const U16String\& twiddledlibid, const U16String\& extendedLibid)](./addcontrolrefrernce/) | Add a reference to a twiddled type library and its extended type library. |
| [AddControlRefrernce(const char16_t* name, const char16_t* libid, const char16_t* twiddledlibid, const char16_t* extendedLibid)](./addcontrolrefrernce/) | Add a reference to a twiddled type library and its extended type library. |
| [AddProjectRefrernce(const U16String\& name, const U16String\& absoluteLibid, const U16String\& relativeLibid)](./addprojectrefrernce/) | Adds a reference to an external VBA project. |
| [AddProjectRefrernce(const char16_t* name, const char16_t* absoluteLibid, const char16_t* relativeLibid)](./addprojectrefrernce/) | Adds a reference to an external VBA project. |
| [AddRegisteredReference(const U16String\& name, const U16String\& libid)](./addregisteredreference/) | Add a reference to an Automation type library. |
| [AddRegisteredReference(const char16_t* name, const char16_t* libid)](./addregisteredreference/) | Add a reference to an Automation type library. |
| [Copy(const VbaProjectReferenceCollection\& source)](./copy/) | Copies references from other VBA project. |
| [Get(int32_t i)](./get/) | Get the reference in the list by the index. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const VbaProjectReferenceCollection\& src)](./operator_asm/) | operator= |
| [VbaProjectReferenceCollection(VbaProjectReferenceCollection_Impl* impl)](./vbaprojectreferencecollection/) | Constructs from an implementation object. |
| [VbaProjectReferenceCollection(const VbaProjectReferenceCollection\& src)](./vbaprojectreferencecollection/) | Copy constructor. |
| [~VbaProjectReferenceCollection()](./~vbaprojectreferencecollection/) | Destructor. |
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
