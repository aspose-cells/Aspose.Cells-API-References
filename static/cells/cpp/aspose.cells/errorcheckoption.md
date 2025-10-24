##Aspose::Cells::ErrorCheckOption class
'Aspose::Cells::ErrorCheckOption class. Error check setting applied on certain ranges in C++.'
## ErrorCheckOption class
Error check setting applied on certain ranges.
```cpp
class ErrorCheckOption
```
## Methods
| Method | Description |
| --- | --- |
| [AddRange(const CellArea\& ca)](./addrange/) | Adds one influenced range by this setting. |
| [ErrorCheckOption(ErrorCheckOption_Impl* impl)](./errorcheckoption/) | Constructs from an implementation object. |
| [ErrorCheckOption(const ErrorCheckOption\& src)](./errorcheckoption/) | Copy constructor. |
| [GetCountOfRange()](./getcountofrange/) | Gets the count of ranges that influenced by this setting. |
| [GetRange(int32_t index)](./getrange/) | Gets the influenced range of this setting by given index. |
| [IsErrorCheck(ErrorCheckType errorCheckType)](./iserrorcheck/) | Checks whether given error type will be checked. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ErrorCheckOption\& src)](./operator_asm/) | operator= |
| [RemoveRange(int32_t index)](./removerange/) | Removes one range by given index. |
| [SetErrorCheck(ErrorCheckType errorCheckType, bool isCheck)](./seterrorcheck/) | Sets whether given error type will be checked. |
| [~ErrorCheckOption()](./~errorcheckoption/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
ErrorCheckOptionCollection opts = workbook.GetWorksheets().Get(0).GetErrorCheckOptions();
int optionIdx = opts.Add();
ErrorCheckOption opt = opts.Get(optionIdx);
opt.SetErrorCheck(ErrorCheckType::InconsistFormula, false);
opt.SetErrorCheck(ErrorCheckType::InconsistRange, false);
opt.SetErrorCheck(ErrorCheckType::TextDate, false);
opt.SetErrorCheck(ErrorCheckType::TextNumber, false);
opt.SetErrorCheck(ErrorCheckType::Validation, false);
CellArea ca = CellArea::CreateCellArea(u"A1", u"B10");
opt.AddRange(ca);
workbook.Save(u"Book1.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
