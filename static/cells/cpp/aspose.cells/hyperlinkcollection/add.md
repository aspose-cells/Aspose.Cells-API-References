##Aspose::Cells::HyperlinkCollection::Add method
'Aspose::Cells::HyperlinkCollection::Add method. Adds a hyperlink to a specified cell or a range of cells in C++.'
## HyperlinkCollection::Add(int32_t, int32_t, int32_t, int32_t, const U16String\&) method
Adds a hyperlink to a specified cell or a range of cells.
```cpp
int32_t Aspose::Cells::HyperlinkCollection::Add(int32_t firstRow, int32_t firstColumn, int32_t totalRows, int32_t totalColumns, const U16String &address)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int32_t | First row of the hyperlink range. |
| firstColumn | int32_t | First column of the hyperlink range. |
| totalRows | int32_t | Number of rows in this hyperlink range. |
| totalColumns | int32_t | Number of columns of this hyperlink range. |
| address | const U16String\& | Address of the hyperlink. |
## ReturnValue
[Hyperlink](../../hyperlink/) object index.
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [HyperlinkCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## HyperlinkCollection::Add(int32_t, int32_t, int32_t, int32_t, const char16_t*) method
Adds a hyperlink to a specified cell or a range of cells.
```cpp
int32_t Aspose::Cells::HyperlinkCollection::Add(int32_t firstRow, int32_t firstColumn, int32_t totalRows, int32_t totalColumns, const char16_t *address)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | int32_t | First row of the hyperlink range. |
| firstColumn | int32_t | First column of the hyperlink range. |
| totalRows | int32_t | Number of rows in this hyperlink range. |
| totalColumns | int32_t | Number of columns of this hyperlink range. |
| address | const char16_t* | Address of the hyperlink. |
## ReturnValue
[Hyperlink](../../hyperlink/) object index.
## See Also
* Class [Vector](../../vector/)
* Class [HyperlinkCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## HyperlinkCollection::Add(const U16String\&, int32_t, int32_t, const U16String\&) method
Adds a hyperlink to a specified cell or a range of cells.
```cpp
int32_t Aspose::Cells::HyperlinkCollection::Add(const U16String &cellName, int32_t totalRows, int32_t totalColumns, const U16String &address)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | const U16String\& | [Cell](../../cell/) name. |
| totalRows | int32_t | Number of rows in this hyperlink range. |
| totalColumns | int32_t | Number of columns of this hyperlink range. |
| address | const U16String\& | Address of the hyperlink. |
## ReturnValue
[Hyperlink](../../hyperlink/) object index.
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook excel;
Worksheet worksheet = excel.GetWorksheets().Get(0);
U16String val_1 = u"A4";
U16String val_2 = u"http://www.aspose.com";
worksheet.GetHyperlinks().Add(val_1, 1, 1, val_2);
val_1 = u"A5";
val_2 = u"c:\\book1.xls";
worksheet.GetHyperlinks().Add(val_1, 1, 1, val_2);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [HyperlinkCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## HyperlinkCollection::Add(const char16_t*, int32_t, int32_t, const char16_t*) method
Adds a hyperlink to a specified cell or a range of cells.
```cpp
int32_t Aspose::Cells::HyperlinkCollection::Add(const char16_t *cellName, int32_t totalRows, int32_t totalColumns, const char16_t *address)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | const char16_t* | [Cell](../../cell/) name. |
| totalRows | int32_t | Number of rows in this hyperlink range. |
| totalColumns | int32_t | Number of columns of this hyperlink range. |
| address | const char16_t* | Address of the hyperlink. |
## ReturnValue
[Hyperlink](../../hyperlink/) object index.
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook excel;
Worksheet worksheet = excel.GetWorksheets().Get(0);
worksheet.GetHyperlinks().Add(u"A4", 1, 1, u"http://www.aspose.com");
worksheet.GetHyperlinks().Add(u"A5", 1, 1, u"c:\\book1.xls");
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [HyperlinkCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## HyperlinkCollection::Add(const U16String\&, const U16String\&, const U16String\&, const U16String\&, const U16String\&) method
Adds a hyperlink to a specified cell or a range of cells.
```cpp
int32_t Aspose::Cells::HyperlinkCollection::Add(const U16String &startCellName, const U16String &endCellName, const U16String &address, const U16String &textToDisplay, const U16String &screenTip)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startCellName | const U16String\& | The top-left cell of the range. |
| endCellName | const U16String\& | The bottom-right cell of the range. |
| address | const U16String\& | Address of the hyperlink. |
| textToDisplay | const U16String\& | The text to be displayed for the specified hyperlink. |
| screenTip | const U16String\& | The screenTip text for the specified hyperlink. |
## ReturnValue
[Hyperlink](../../hyperlink/) object index.
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [HyperlinkCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## HyperlinkCollection::Add(const char16_t*, const char16_t*, const char16_t*, const char16_t*, const char16_t*) method
Adds a hyperlink to a specified cell or a range of cells.
```cpp
int32_t Aspose::Cells::HyperlinkCollection::Add(const char16_t *startCellName, const char16_t *endCellName, const char16_t *address, const char16_t *textToDisplay, const char16_t *screenTip)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startCellName | const char16_t* | The top-left cell of the range. |
| endCellName | const char16_t* | The bottom-right cell of the range. |
| address | const char16_t* | Address of the hyperlink. |
| textToDisplay | const char16_t* | The text to be displayed for the specified hyperlink. |
| screenTip | const char16_t* | The screenTip text for the specified hyperlink. |
## ReturnValue
[Hyperlink](../../hyperlink/) object index.
## See Also
* Class [Vector](../../vector/)
* Class [HyperlinkCollection](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
