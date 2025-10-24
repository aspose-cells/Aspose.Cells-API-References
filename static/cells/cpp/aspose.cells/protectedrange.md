##Aspose::Cells::ProtectedRange class
'Aspose::Cells::ProtectedRange class. A specified range to be allowed to edit when the sheet protection is ON in C++.'
## ProtectedRange class
A specified range to be allowed to edit when the sheet protection is ON.
```cpp
class ProtectedRange
```
## Methods
| Method | Description |
| --- | --- |
| [AddArea(int32_t startRow, int32_t startColumn, int32_t endRow, int32_t endColumn)](./addarea/) | Adds a referred area to this. |
| [GetAreas()](./getareas/) | Gets all referred areas. |
| [GetCellArea()](./getcellarea/) | Gets the [CellArea](../cellarea/) object represents the cell area to be protected. |
| [GetName()](./getname/) | Gets the [Range](../range/) title. This is used as a descriptor, not as a named range definition. |
| [GetPassword()](./getpassword/) | Represents the password to protect the range. |
| [GetSecurityDescriptor()](./getsecuritydescriptor/) | The security descriptor defines user accounts who may edit this range without providing a password to access the range. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsProtectedWithPassword()](./isprotectedwithpassword/) | Indicates whether the worksheets is protected with password. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ProtectedRange\& src)](./operator_asm/) | operator= |
| [ProtectedRange(ProtectedRange_Impl* impl)](./protectedrange/) | Constructs from an implementation object. |
| [ProtectedRange(const ProtectedRange\& src)](./protectedrange/) | Copy constructor. |
| [SetName(const U16String\& value)](./setname/) | Gets the [Range](../range/) title. This is used as a descriptor, not as a named range definition. |
| [SetName(const char16_t* value)](./setname/) | Gets the [Range](../range/) title. This is used as a descriptor, not as a named range definition. |
| [SetPassword(const U16String\& value)](./setpassword/) | Represents the password to protect the range. |
| [SetPassword(const char16_t* value)](./setpassword/) | Represents the password to protect the range. |
| [SetSecurityDescriptor(const U16String\& value)](./setsecuritydescriptor/) | The security descriptor defines user accounts who may edit this range without providing a password to access the range. |
| [SetSecurityDescriptor(const char16_t* value)](./setsecuritydescriptor/) | The security descriptor defines user accounts who may edit this range without providing a password to access the range. |
| [~ProtectedRange()](./~protectedrange/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
