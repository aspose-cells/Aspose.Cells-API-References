##Aspose::Cells::Vba::VbaModule class
'Aspose::Cells::Vba::VbaModule class. Represents the module in VBA project in C++.'
## VbaModule class
Represents the module in VBA project.
```cpp
class VbaModule
```
## Methods
| Method | Description |
| --- | --- |
| [GetBinaryCodes()](./getbinarycodes/) | Gets and sets the binary codes of module. |
| [GetCodes()](./getcodes/) | Gets and sets the codes of module. |
| [GetName()](./getname/) | Gets and sets the name of Module. |
| [GetType()](./gettype/) | Gets the type of module. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const VbaModule\& src)](./operator_asm/) | operator= |
| [SetCodes(const U16String\& value)](./setcodes/) | Gets and sets the codes of module. |
| [SetCodes(const char16_t* value)](./setcodes/) | Gets and sets the codes of module. |
| [SetName(const U16String\& value)](./setname/) | Gets and sets the name of Module. |
| [SetName(const char16_t* value)](./setname/) | Gets and sets the name of Module. |
| [VbaModule(VbaModule_Impl* impl)](./vbamodule/) | Constructs from an implementation object. |
| [VbaModule(const VbaModule\& src)](./vbamodule/) | Copy constructor. |
| [~VbaModule()](./~vbamodule/) | Destructor. |
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
// Add a new module.
int index = vbaProject.GetModules().Add(VbaModuleType::Class, u"test");
// Get vba module
VbaModule vbaModule = vbaProject.GetModules().Get(index);
// Set codes
vbaModule.SetCodes(u"Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub");
//Saving the Excel file
workbook.Save(u"book1.xlsm");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Vba](../)
* Library [Aspose.Cells for C++](../../)
