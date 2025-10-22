##Aspose::Cells::VerticalPageBreak class
'Aspose::Cells::VerticalPageBreak class. Encapsulates the object that represents a vertical page break in C++.'
## VerticalPageBreak class
Encapsulates the object that represents a vertical page break.
```cpp
class VerticalPageBreak
```
## Methods
| Method | Description |
| --- | --- |
| [GetColumn()](./getcolumn/) | Gets the column index of the vertical page break. |
| [GetEndRow()](./getendrow/) | Gets the end row index of the vertical page break. |
| [GetStartRow()](./getstartrow/) | Gets the start row index of the vertical page break. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const VerticalPageBreak\& src)](./operator_asm/) | operator= |
| [VerticalPageBreak(VerticalPageBreak_Impl* impl)](./verticalpagebreak/) | Constructs from an implementation object. |
| [VerticalPageBreak(const VerticalPageBreak\& src)](./verticalpagebreak/) | Copy constructor. |
| [~VerticalPageBreak()](./~verticalpagebreak/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook excel;
//Add a pagebreak at G5
excel.GetWorksheets().Get(0).GetHorizontalPageBreaks().Add(u"G5");
excel.GetWorksheets().Get(0).GetVerticalPageBreaks().Add(u"G5");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
