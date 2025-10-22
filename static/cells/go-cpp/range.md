##Range Class
'Range class. Encapsulates the object that represents range in Go.'
## Range class
Encapsulates the object that represents a range of cells within a spreadsheet.
```go
type Range struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[AutoFill_Range](./autofill_range/) | Automaticall fill the target range. |
|[AutoFill_Range_AutoFillType](./autofill_range_autofilltype/) | Automaticall fill the target range. |
|[GetCurrentRegion](./getcurrentregion/) | Returns a Range object that represents the current region.The current region is a range bounded by any combination of blank rows and blank columns. |
|[GetHyperlinks](./gethyperlinks/) | Gets all hyperlink in the range. |
|[AddHyperlink](./addhyperlink/) | Adds a hyperlink to a specified cell or a range of cells. |
|[GetEnumerator](./getenumerator/) | Gets the enumerator for cells in this Range. |
|[IsIntersect](./isintersect/) | Indicates whether the range is intersect. |
|[Intersect](./intersect/) | Returns a Range object that represents the rectangular intersection of two ranges. |
|[UnionRanges](./unionranges/) | Returns the union result of two ranges. |
|[GetRowCount](./getrowcount/) | Gets the count of rows in the range. |
|[GetColumnCount](./getcolumncount/) | Gets the count of columns in the range. |
|[GetName](./getname/) | Gets or sets the name of the range. |
|[SetName](./setname/) | Gets or sets the name of the range. |
|[GetRefersTo](./getrefersto/) | Gets the range's refers to. |
|[GetAddress](./getaddress/) | Gets address of the range. |
|[IsBlank](./isblank/) | Indicates whether the range contains values. |
|[GetLeft](./getleft/) | Gets the distance, in points, from the left edge of column A to the left edge of the range. |
|[GetTop](./gettop/) | Gets the distance, in points, from the top edge of row 1 to the top edge of the range. |
|[GetWidth](./getwidth/) | Gets the width of a range in points. |
|[GetHeight](./getheight/) | Gets the width of a range in points. |
|[GetFirstRow](./getfirstrow/) | Gets the index of the first row of the range. |
|[GetFirstColumn](./getfirstcolumn/) | Gets the index of the first column of the range. |
|[Merge](./merge/) | Combines a range of cells into a single cell. |
|[UnMerge](./unmerge/) | Unmerges merged cells of this range. |
|[PutValue](./putvalue/) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset. |
|[GetValue](./getvalue/) | Gets and sets the value of the range. |
|[SetValue](./setvalue/) | Gets and sets the value of the range. |
|[SetStyle_Style_Bool](./setstyle_style_bool/) | Apply the cell style. |
|[ApplyStyle](./applystyle/) | Applies formats for a whole range. |
|[SetStyle_Style](./setstyle_style/) | Sets the style of the range. |
|[SetOutlineBorders_CellBorderType_CellsColor](./setoutlineborders_cellbordertype_cellscolor/) | Sets the outline borders around a range of cells with same border style and color. |
|[SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Sets the outline borders around a range of cells with same border style and color. |
|[SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | Sets out line borders around a range of cells. |
|[SetOutlineBorder_BorderType_CellBorderType_CellsColor](./setoutlineborder_bordertype_cellbordertype_cellscolor/) | Sets outline border around a range of cells. |
|[SetOutlineBorder_BorderType_CellBorderType_Color](./setoutlineborder_bordertype_cellbordertype_color/) | Sets outline border around a range of cells. |
|[SetInsideBorders](./setinsideborders/) | Set inside borders of the range. |
|[GetColumnWidth](./getcolumnwidth/) | Sets or gets the column width of this range |
|[SetColumnWidth](./setcolumnwidth/) | Sets or gets the column width of this range |
|[GetRowHeight](./getrowheight/) | Sets or gets the height of rows in this range |
|[SetRowHeight](./setrowheight/) | Sets or gets the height of rows in this range |
|[MoveTo](./moveto/) | Move the current range to the dest range. |
|[CopyData](./copydata/) | Copies cell data (including formulas) from a source range. |
|[CopyValue](./copyvalue/) | Copies cell value from a source range. |
|[CopyStyle](./copystyle/) | Copies style settings from a source range. |
|[Copy_Range_PasteOptions](./copy_range_pasteoptions/) | Copying the range with paste special options. |
|[Transpose](./transpose/) | Transpose (rotate) data from rows to columns or vice versa. |
|[Copy_Range](./copy_range/) | Copies data (including formulas), formatting, drawing objects etc. from a source range. |
|[Get](./get/) | Gets Cell object in this range. |
|[GetCellOrNull](./getcellornull/) | Gets Cell object or null in this range. |
|[GetOffset](./getoffset/) | Gets Range range by offset. |
|[GetEntireColumn](./getentirecolumn/) | Gets a Range object that represents the entire column (or columns) that contains the specified range. |
|[GetEntireRow](./getentirerow/) | Gets a Range object that represents the entire row (or rows) that contains the specified range. |
|[GetWorksheet](./getworksheet/) | Gets the Worksheetobject which contains this range. |
|[ToString](./tostring/) | Returns a string represents the current Range object. |
|[ToImage](./toimage/) | Converts the range to image. |
|[ToJson](./tojson/) | Convert the range to JSON value. |
|[ToHtml](./tohtml/) | Convert the range to html . |
|[Clear](./clear/) | Clears this range. |
|[ClearContents](./clearcontents/) | Clears the contents of this range. |
|[ClearFormats](./clearformats/) | Clears the formats of this range. |
|[ClearComments](./clearcomments/) | Clears the comments of this range. |
|[ClearHyperlinks](./clearhyperlinks/) | Only removes hyperlinks. |
