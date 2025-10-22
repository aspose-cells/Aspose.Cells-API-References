##Aspose::Cells::Vba::VbaProject class
'Aspose::Cells::Vba::VbaProject class. Represents the VBA project in C++.'
## VbaProject class
Represents the VBA project.
```cpp
class VbaProject
```
## Methods
| Method | Description |
| --- | --- |
| [Copy(const VbaProject\& source)](./copy/) | Copy VBA project from other file. |
| [GetCertRawData()](./getcertrawdata/) | Gets certificate raw data if this VBA project is signed. |
| [GetEncoding()](./getencoding/) | Gets and sets the encoding of VBA project. |
| [GetIslockedForViewing()](./getislockedforviewing/) | Indicates whether this VBA project is locked for viewing. |
| [GetModules()](./getmodules/) | Gets all [VbaModule](../vbamodule/) objects. |
| [GetName()](./getname/) | Gets and sets the name of the VBA project. |
| [GetReferences()](./getreferences/) | Gets all references of VBA project. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsProtected()](./isprotected/) | Indicates whether this VBA project is protected. |
| [IsSigned()](./issigned/) | Indicates whether VBAcode is signed or not. |
| [IsValidSigned()](./isvalidsigned/) | Indicates whether the signature of VBA project is valid or not. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const VbaProject\& src)](./operator_asm/) | operator= |
| [Protect(bool islockedForViewing, const U16String\& password)](./protect/) | Protects or unprotects this VBA project. |
| [Protect(bool islockedForViewing, const char16_t* password)](./protect/) | Protects or unprotects this VBA project. |
| [SetEncoding(EncodingType value)](./setencoding/) | Gets and sets the encoding of VBA project. |
| [SetName(const U16String\& value)](./setname/) | Gets and sets the name of the VBA project. |
| [SetName(const char16_t* value)](./setname/) | Gets and sets the name of the VBA project. |
| [Sign(const DigitalSignature\& digitalSignature)](./sign/) | Sign this VBA project by a DigitalSignature. |
| [ValidatePassword(const U16String\& password)](./validatepassword/) | Validates protection password. |
| [ValidatePassword(const char16_t* password)](./validatepassword/) | Validates protection password. |
| [VbaProject(VbaProject_Impl* impl)](./vbaproject/) | Constructs from an implementation object. |
| [VbaProject(const VbaProject\& src)](./vbaproject/) | Copy constructor. |
| [~VbaProject()](./~vbaproject/) | Destructor. |
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
//Saving the Excel file
workbook.Save(u"book1.xlsm");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Vba](../)
* Library [Aspose.Cells for C++](../../)
