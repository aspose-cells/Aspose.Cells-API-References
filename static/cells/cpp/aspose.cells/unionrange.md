##Aspose::Cells::UnionRange class
'Aspose::Cells::UnionRange class. Represents union range in C++.'
## UnionRange class
Represents union range.
```cpp
class UnionRange
```
## Methods
| Method | Description |
| --- | --- |
| [ApplyStyle(const Style\& style, const StyleFlag\& flag)](./applystyle/) | Applies formats for a whole range. |
| [Copy(const UnionRange\& range, const PasteOptions\& options)](./copy/) | Copying the range with paste special options. |
| [GetCellCount()](./getcellcount/) | Gets all cell count in the range. |
| [GetColumnCount()](./getcolumncount/) | Gets the count of rows in the range. |
| [GetEnumerator()](./getenumerator/) | Gets the enumerator for cells in this [Range](../range/). |
| [GetFirstColumn()](./getfirstcolumn/) | Gets the index of the first column of the range. |
| [GetFirstRow()](./getfirstrow/) | Gets the index of the first row of the range. |
| [GetHasRange()](./gethasrange/) | Indicates whether this has range. |
| [GetHyperlinks()](./gethyperlinks/) | Gets all hyperlink in the range. |
| [GetName()](./getname/) | Gets or sets the name of the range. |
| [GetRangeCount()](./getrangecount/) | Gets the count of the ranges. |
| [GetRanges()](./getranges/) | Gets all union ranges. |
| [GetRefersTo()](./getrefersto/) | Gets the range's refers to. |
| [GetRowCount()](./getrowcount/) | Gets the count of rows in the range. |
| [GetValue()](./getvalue/) | Gets and sets the values of the range. |
| [Intersect(const U16String\& range)](./intersect/) | Intersects another range. |
| [Intersect(const char16_t* range)](./intersect/) | Intersects another range. |
| [Intersect(const UnionRange\& unionRange)](./intersect/) | Intersects another range. |
| [Intersect(const Vector \<Range\>\& ranges)](./intersect/) | Intersects another range. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [Merge()](./merge/) | Combines a range of cells into a single cell. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const UnionRange\& src)](./operator_asm/) | operator= |
| [PutValue(const U16String\& stringValue, bool isConverted, bool setStyle)](./putvalue/) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [PutValue(const char16_t* stringValue, bool isConverted, bool setStyle)](./putvalue/) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [SetName(const U16String\& value)](./setname/) | Gets or sets the name of the range. |
| [SetName(const char16_t* value)](./setname/) | Gets or sets the name of the range. |
| [SetOutlineBorders(const Vector \<CellBorderType\>\& borderStyles, const Vector \<Aspose::Cells::Color\>\& borderColors)](./setoutlineborders/) | Sets out line borders around a range of cells. |
| [SetOutlineBorders(CellBorderType borderStyle, const Aspose::Cells::Color\& borderColor)](./setoutlineborders/) | Sets the outline borders around a range of cells with same border style and color. |
| [SetStyle(const Style\& style)](./setstyle/) | Sets the style of the range. |
| [SetValue(const Aspose::Cells::Object\& value)](./setvalue/) | Gets and sets the values of the range. |
| [Union(const U16String\& range)](./union/) | Union another range. |
| [Union(const char16_t* range)](./union/) | Union another range. |
| [Union(const UnionRange\& unionRange)](./union/) | Union another range. |
| [Union(const Vector \<Range\>\& ranges)](./union/) | Union the ranges. |
| [UnionRange(UnionRange_Impl* impl)](./unionrange/) | Constructs from an implementation object. |
| [UnionRange(const UnionRange\& src)](./unionrange/) | Copy constructor. |
| [UnMerge()](./unmerge/) | Unmerges merged cells of this range. |
| [~UnionRange()](./~unionrange/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
