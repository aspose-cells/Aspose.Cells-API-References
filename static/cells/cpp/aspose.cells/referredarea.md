##Aspose::Cells::ReferredArea class
'Aspose::Cells::ReferredArea class. Represents a referred area by the formula in C++.'
## ReferredArea class
Represents a referred area by the formula.
```cpp
class ReferredArea
```
## Methods
| Method | Description |
| --- | --- |
| [GetEndColumn()](./getendcolumn/) | The end column of the area. |
| [GetEndRow()](./getendrow/) | The end row of the area. |
| [GetExternalFileName()](./getexternalfilename/) | Get the external file name if this is an external reference. |
| [GetSheetName()](./getsheetname/) | Indicates which sheet this reference is in. |
| [GetSheetNames()](./getsheetnames/) | Names of all the worksheets this instance references to. |
| [GetStartColumn()](./getstartcolumn/) | The start column of the area. |
| [GetStartRow()](./getstartrow/) | The start row of the area. |
| [GetValue(int32_t rowOffset, int32_t colOffset)](./getvalue/) | Gets cell value with given offset from the top-left of this area. |
| [GetValue(int32_t rowOffset, int32_t colOffset, bool calculateFormulas)](./getvalue/) | Gets cell value with given offset from the top-left of this area. |
| [GetValues()](./getvalues/) | Gets cell values in this area. |
| [GetValues(bool calculateFormulas)](./getvalues/) | Gets cell values in this area. |
| [IsArea()](./isarea/) | Indicates whether this is an area. |
| [IsEntireColumn()](./isentirecolumn/) | Indicates whether this area contains all rows(entire column). |
| [IsEntireRow()](./isentirerow/) | Indicates whether this area contains all columns(entire row). |
| [IsExternalLink()](./isexternallink/) | Indicates whether this is an external link. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ReferredArea\& src)](./operator_asm/) | operator= |
| [ReferredArea(ReferredArea_Impl* impl)](./referredarea/) | Constructs from an implementation object. |
| [ReferredArea(const ReferredArea\& src)](./referredarea/) | Copy constructor. |
| [ToString()](./tostring/) | Returns the reference address of this area. Generally it is the address of the reference which may be used in formula, such as "Sheet1!A1:C3". |
| [~ReferredArea()](./~referredarea/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
