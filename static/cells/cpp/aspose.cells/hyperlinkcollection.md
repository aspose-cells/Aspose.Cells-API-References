##Aspose::Cells::HyperlinkCollection class
'Aspose::Cells::HyperlinkCollection class. Encapsulates a collection of Hyperlink objects in C++.'
## HyperlinkCollection class
Encapsulates a collection of [Hyperlink](../hyperlink/) objects.
```cpp
class HyperlinkCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(int32_t firstRow, int32_t firstColumn, int32_t totalRows, int32_t totalColumns, const U16String\& address)](./add/) | Adds a hyperlink to a specified cell or a range of cells. |
| [Add(int32_t firstRow, int32_t firstColumn, int32_t totalRows, int32_t totalColumns, const char16_t* address)](./add/) | Adds a hyperlink to a specified cell or a range of cells. |
| [Add(const U16String\& cellName, int32_t totalRows, int32_t totalColumns, const U16String\& address)](./add/) | Adds a hyperlink to a specified cell or a range of cells. |
| [Add(const char16_t* cellName, int32_t totalRows, int32_t totalColumns, const char16_t* address)](./add/) | Adds a hyperlink to a specified cell or a range of cells. |
| [Add(const U16String\& startCellName, const U16String\& endCellName, const U16String\& address, const U16String\& textToDisplay, const U16String\& screenTip)](./add/) | Adds a hyperlink to a specified cell or a range of cells. |
| [Add(const char16_t* startCellName, const char16_t* endCellName, const char16_t* address, const char16_t* textToDisplay, const char16_t* screenTip)](./add/) | Adds a hyperlink to a specified cell or a range of cells. |
| [Clear()](./clear/) | Clears all hyperlinks. |
| [Get(int32_t index)](./get/) | Gets the [Hyperlink](../hyperlink/) element at the specified index. |
| [GetCount()](./getcount/) |  |
| [HyperlinkCollection(HyperlinkCollection_Impl* impl)](./hyperlinkcollection/) | Constructs from an implementation object. |
| [HyperlinkCollection(const HyperlinkCollection\& src)](./hyperlinkcollection/) | Copy constructor. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const HyperlinkCollection\& src)](./operator_asm/) | operator= |
| [RemoveAt(int32_t index)](./removeat/) | Remove the hyperlink at the specified index in this collection. |
| [~HyperlinkCollection()](./~hyperlinkcollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Get Hyperlinks Collection
HyperlinkCollection hyperlinks = worksheet.GetHyperlinks();
//Adding a hyperlink to a URL at "A1" cell
hyperlinks.Add(u"A1", 1, 1, u"http://www.aspose.com");
//Saving the Excel file
workbook.Save(u"book1.xls");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
