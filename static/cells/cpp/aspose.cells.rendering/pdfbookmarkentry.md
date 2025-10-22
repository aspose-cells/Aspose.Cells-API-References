##Aspose::Cells::Rendering::PdfBookmarkEntry class
'Aspose::Cells::Rendering::PdfBookmarkEntry class. PdfBookmarkEntry is an entry in pdf bookmark. if Text property of current instance is null or "", current instance will be hidden and children will be inserted on current level in C++.'
## PdfBookmarkEntry class
[PdfBookmarkEntry](./) is an entry in pdf bookmark. if Text property of current instance is null or "", current instance will be hidden and children will be inserted on current level.
```cpp
class PdfBookmarkEntry
```
## Methods
| Method | Description |
| --- | --- |
| [GetDestination()](./getdestination/) | The cell to which the bookmark link. |
| [GetDestinationName()](./getdestinationname/) | Gets or sets name of destination. |
| [GetText()](./gettext/) | Title of a bookmark. |
| [IsCollapse()](./iscollapse/) | When this property is true, the bookmarkentry will collapse, otherwise it will expand. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsOpen()](./isopen/) | When this property is true, the bookmarkentry will expand, otherwise it will collapse. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PdfBookmarkEntry\& src)](./operator_asm/) | operator= |
| [PdfBookmarkEntry()](./pdfbookmarkentry/) | Default constructor. |
| [PdfBookmarkEntry(PdfBookmarkEntry_Impl* impl)](./pdfbookmarkentry/) | Constructs from an implementation object. |
| [PdfBookmarkEntry(const PdfBookmarkEntry\& src)](./pdfbookmarkentry/) | Copy constructor. |
| [SetDestination(const Cell\& value)](./setdestination/) | The cell to which the bookmark link. |
| [SetDestinationName(const U16String\& value)](./setdestinationname/) | Gets or sets name of destination. |
| [SetDestinationName(const char16_t* value)](./setdestinationname/) | Gets or sets name of destination. |
| [SetIsCollapse(bool value)](./setiscollapse/) | When this property is true, the bookmarkentry will collapse, otherwise it will expand. |
| [SetIsOpen(bool value)](./setisopen/) | When this property is true, the bookmarkentry will expand, otherwise it will collapse. |
| [SetText(const U16String\& value)](./settext/) | Title of a bookmark. |
| [SetText(const char16_t* value)](./settext/) | Title of a bookmark. |
| [~PdfBookmarkEntry()](./~pdfbookmarkentry/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
workbook.GetWorksheets().Add();
workbook.GetWorksheets().Add();
Cell cellInPage1 = workbook.GetWorksheets().Get(0).GetCells().Get(u"A1");
Cell cellInPage2 = workbook.GetWorksheets().Get(1).GetCells().Get(u"A1");
Cell cellInPage3 = workbook.GetWorksheets().Get(2).GetCells().Get(u"A1");
cellInPage1.PutValue(u"page1");
cellInPage2.PutValue(u"page2");
cellInPage3.PutValue(u"page3");
PdfBookmarkEntry pbeRoot;
pbeRoot.SetText(u"root");  // if pbeRoot.Text = null, all children of pbeRoot will be inserted on the top level in the bookmark.
pbeRoot.SetDestination(cellInPage1);
pbeRoot.SetIsOpen(false);
PdfBookmarkEntry subPbe1;
subPbe1.SetText(u"section1");
subPbe1.SetDestination(cellInPage2);
PdfBookmarkEntry subPbe2;
subPbe2.SetText(u"section2");
subPbe2.SetDestination(cellInPage3);
PdfSaveOptions saveOptions;
saveOptions.SetBookmark(pbeRoot);
workbook.Save(u"output_bookmark.pdf", saveOptions);
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Rendering](../)
* Library [Aspose.Cells for C++](../../)
