##Aspose::Cells::Range class
'Aspose::Cells::Range class. Encapsulates the object that represents a range of cells within a spreadsheet in C++.'
## Range class
Encapsulates the object that represents a range of cells within a spreadsheet.
```cpp
class Range
```
## Methods
| Method | Description |
| --- | --- |
| [AddHyperlink(const U16String\& address, const U16String\& textToDisplay, const U16String\& screenTip)](./addhyperlink/) | Adds a hyperlink to a specified cell or a range of cells. |
| [AddHyperlink(const char16_t* address, const char16_t* textToDisplay, const char16_t* screenTip)](./addhyperlink/) | Adds a hyperlink to a specified cell or a range of cells. |
| [ApplyStyle(const Style\& style, const StyleFlag\& flag)](./applystyle/) | Applies formats for a whole range. |
| [AutoFill(const Range\& target)](./autofill/) | Automaticall fill the target range. |
| [AutoFill(const Range\& target, AutoFillType autoFillType)](./autofill/) | Automaticall fill the target range. |
| [Clear()](./clear/) | Clears this range. |
| [ClearComments()](./clearcomments/) | Clears the comments of this range. |
| [ClearContents()](./clearcontents/) | Clears the contents of this range. |
| [ClearFormats()](./clearformats/) | Clears the formats of this range. |
| [ClearHyperlinks(bool clearFormat)](./clearhyperlinks/) | Only removes hyperlinks. |
| [Copy(const Range\& range, const PasteOptions\& options)](./copy/) | Copying the range with paste special options. |
| [Copy(const Range\& range)](./copy/) | Copies data (including formulas), formatting, drawing objects etc. from a source range. |
| [CopyData(const Range\& range)](./copydata/) | Copies cell data (including formulas) from a source range. |
| [CopyStyle(const Range\& range)](./copystyle/) | Copies style settings from a source range. |
| [CopyValue(const Range\& range)](./copyvalue/) | Copies cell value from a source range. |
| [Get(int32_t rowOffset, int32_t columnOffset)](./get/) | Gets [Cell](../cell/) object in this range. |
| [GetAddress()](./getaddress/) | Gets address of the range. |
| [GetCellOrNull(int32_t rowOffset, int32_t columnOffset)](./getcellornull/) | Gets [Cell](../cell/) object or null in this range. |
| [GetColumnCount()](./getcolumncount/) | Gets the count of columns in the range. |
| [GetColumnWidth()](./getcolumnwidth/) | Sets or gets the column width of this range. |
| [GetCurrentRegion()](./getcurrentregion/) | Returns a [Range](./) object that represents the current region. The current region is a range bounded by any combination of blank rows and blank columns. |
| [GetEntireColumn()](./getentirecolumn/) | Gets a [Range](./) object that represents the entire column (or columns) that contains the specified range. |
| [GetEntireRow()](./getentirerow/) | Gets a [Range](./) object that represents the entire row (or rows) that contains the specified range. |
| [GetEnumerator()](./getenumerator/) | Gets the enumerator for cells in this [Range](./). |
| [GetFirstColumn()](./getfirstcolumn/) | Gets the index of the first column of the range. |
| [GetFirstRow()](./getfirstrow/) | Gets the index of the first row of the range. |
| [GetHeight()](./getheight/) | Gets the width of a range in points. |
| [GetHyperlinks()](./gethyperlinks/) | Gets all hyperlink in the range. |
| [GetLeft()](./getleft/) | Gets the distance, in points, from the left edge of column A to the left edge of the range. |
| [GetName()](./getname/) | Gets or sets the name of the range. |
| [GetOffset(int32_t rowOffset, int32_t columnOffset)](./getoffset/) | Gets [Range](./) range by offset. |
| [GetRefersTo()](./getrefersto/) | Gets the range's refers to. |
| [GetRowCount()](./getrowcount/) | Gets the count of rows in the range. |
| [GetRowHeight()](./getrowheight/) | Sets or gets the height of rows in this range. |
| [GetTop()](./gettop/) | Gets the distance, in points, from the top edge of row 1 to the top edge of the range. |
| [GetValue()](./getvalue/) | Gets and sets the value of the range. |
| [GetWidth()](./getwidth/) | Gets the width of a range in points. |
| [GetWorksheet()](./getworksheet/) | Gets the [Worksheet](../worksheet/)object which contains this range. |
| [Intersect(const Range\& range)](./intersect/) | Returns a [Range](./) object that represents the rectangular intersection of two ranges. |
| [IsBlank()](./isblank/) | Indicates whether the range contains values. |
| [IsIntersect(const Range\& range)](./isintersect/) | Indicates whether the range is intersect. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [Merge()](./merge/) | Combines a range of cells into a single cell. |
| [MoveTo(int32_t destRow, int32_t destColumn)](./moveto/) | Move the current range to the dest range. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Range\& src)](./operator_asm/) | operator= |
| [PutValue(const U16String\& stringValue, bool isConverted, bool setStyle)](./putvalue/) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [PutValue(const char16_t* stringValue, bool isConverted, bool setStyle)](./putvalue/) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [Range(Range_Impl* impl)](./range/) | Constructs from an implementation object. |
| [Range(const Range\& src)](./range/) | Copy constructor. |
| [SetColumnWidth(double value)](./setcolumnwidth/) | Sets or gets the column width of this range. |
| [SetInsideBorders(BorderType borderEdge, CellBorderType lineStyle, const CellsColor\& borderColor)](./setinsideborders/) | Set inside borders of the range. |
| [SetName(const U16String\& value)](./setname/) | Gets or sets the name of the range. |
| [SetName(const char16_t* value)](./setname/) | Gets or sets the name of the range. |
| [SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, const CellsColor\& borderColor)](./setoutlineborder/) | Sets outline border around a range of cells. |
| [SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, const Aspose::Cells::Color\& borderColor)](./setoutlineborder/) | Sets outline border around a range of cells. |
| [SetOutlineBorders(CellBorderType borderStyle, const CellsColor\& borderColor)](./setoutlineborders/) | Sets the outline borders around a range of cells with same border style and color. |
| [SetOutlineBorders(CellBorderType borderStyle, const Aspose::Cells::Color\& borderColor)](./setoutlineborders/) | Sets the outline borders around a range of cells with same border style and color. |
| [SetOutlineBorders(const Vector \<CellBorderType\>\& borderStyles, const Vector \<Aspose::Cells::Color\>\& borderColors)](./setoutlineborders/) | Sets out line borders around a range of cells. |
| [SetRowHeight(double value)](./setrowheight/) | Sets or gets the height of rows in this range. |
| [SetStyle(const Style\& style, bool explicitFlag)](./setstyle/) | Apply the cell style. |
| [SetStyle(const Style\& style)](./setstyle/) | Sets the style of the range. |
| [SetValue(const Aspose::Cells::Object\& value)](./setvalue/) | Gets and sets the value of the range. |
| [ToHtml(const HtmlSaveOptions\& saveOptions)](./tohtml/) | Convert the range to html . |
| [ToImage(const ImageOrPrintOptions\& options)](./toimage/) | Converts the range to image. |
| [ToJson(const JsonSaveOptions\& options)](./tojson/) | Convert the range to JSON value. |
| [ToString()](./tostring/) | Returns a string represents the current [Range](./) object. |
| [Transpose()](./transpose/) | Transpose (rotate) data from rows to columns or vice versa. |
| [UnionRang(const Range\& range)](./unionrang/) |  **(Deprecated)** Returns the union result of two ranges. |
| [UnionRanges(const Vector \<Range\>\& ranges)](./unionranges/) | Returns the union result of two ranges. |
| [UnMerge()](./unmerge/) | Unmerges merged cells of this range. |
| [~Range()](./~range/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Remarks
The [Range](./) class denotes a region of Excel spreadsheet. With this, you can format and set value of the range. And you can simply copy range of Excel too.
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
// Get the first Worksheet Cells.
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
// Create a range (A1:D3).
Range range = cells.CreateRange(u"A1", u"D3");
//Save the Excel file
workbook.Save(u"book1.xlsm");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
