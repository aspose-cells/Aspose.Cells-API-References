##Aspose::Cells::LowCode::AbstractLowCodeProtectionProvider class
'Aspose::Cells::LowCode::AbstractLowCodeProtectionProvider class. Implementation to provide protection settings in C++.'
## AbstractLowCodeProtectionProvider class
Implementation to provide protection settings.
```cpp
class AbstractLowCodeProtectionProvider
```
## Methods
| Method | Description |
| --- | --- |
| [AbstractLowCodeProtectionProvider()](./abstractlowcodeprotectionprovider/) | Default constructor. |
| [AbstractLowCodeProtectionProvider(AbstractLowCodeProtectionProvider_Impl* impl)](./abstractlowcodeprotectionprovider/) | Constructs from an implementation object. |
| [AbstractLowCodeProtectionProvider(const AbstractLowCodeProtectionProvider\& src)](./abstractlowcodeprotectionprovider/) | Copy constructor. |
| [GetOpenPassword()](./getopenpassword/) | Gets the password to open spread sheet file. |
| [GetWorkbookPassword()](./getworkbookpassword/) | Gets the password to protect the workbook with specified protection type. |
| [GetWorkbookProtectionType()](./getworkbookprotectiontype/) | Gets the protection type to protect the workbook. |
| [GetWorksheetPassword(const U16String\& sheetName)](./getworksheetpassword/) | Gets the password to protect the specified worksheet. |
| [GetWorksheetPassword(const char16_t* sheetName)](./getworksheetpassword/) | Gets the password to protect the specified worksheet. |
| [GetWorksheetProtectionType(const U16String\& sheetName)](./getworksheetprotectiontype/) | Gets the protection type to protect the specified worksheet. |
| [GetWorksheetProtectionType(const char16_t* sheetName)](./getworksheetprotectiontype/) | Gets the protection type to protect the specified worksheet. |
| [GetWritePassword()](./getwritepassword/) | Gets the password to modify spread sheet file. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const AbstractLowCodeProtectionProvider\& src)](./operator_asm/) | operator= |
| [~AbstractLowCodeProtectionProvider()](./~abstractlowcodeprotectionprovider/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells::LowCode](../)
* Library [Aspose.Cells for C++](../../)
