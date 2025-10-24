##Aspose::Cells::WriteProtection class
'Aspose::Cells::WriteProtection class. Specifies write protection settings for a workbook in C++.'
## WriteProtection class
Specifies write protection settings for a workbook.
```cpp
class WriteProtection
```
## Methods
| Method | Description |
| --- | --- |
| [GetAuthor()](./getauthor/) | Gets and sets the author. |
| [GetPassword()](./getpassword/) | Sets the protected password to modify the file. |
| [GetRecommendReadOnly()](./getrecommendreadonly/) | Indicates if the Read Only Recommended option is selected. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsWriteProtected()](./iswriteprotected/) | Indicates whether this workbook is write protected. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const WriteProtection\& src)](./operator_asm/) | operator= |
| [SetAuthor(const U16String\& value)](./setauthor/) | Gets and sets the author. |
| [SetAuthor(const char16_t* value)](./setauthor/) | Gets and sets the author. |
| [SetPassword(const U16String\& value)](./setpassword/) | Sets the protected password to modify the file. |
| [SetPassword(const char16_t* value)](./setpassword/) | Sets the protected password to modify the file. |
| [SetRecommendReadOnly(bool value)](./setrecommendreadonly/) | Indicates if the Read Only Recommended option is selected. |
| [ValidatePassword(const U16String\& password)](./validatepassword/) | Returns true if the specified password is the same as the write-protection password the file was protected with. |
| [ValidatePassword(const char16_t* password)](./validatepassword/) | Returns true if the specified password is the same as the write-protection password the file was protected with. |
| [WriteProtection(WriteProtection_Impl* impl)](./writeprotection/) | Constructs from an implementation object. |
| [WriteProtection(const WriteProtection\& src)](./writeprotection/) | Copy constructor. |
| [~WriteProtection()](./~writeprotection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
