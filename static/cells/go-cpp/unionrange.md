##UnionRange Class
'UnionRange class. Encapsulates the object that represents unionrange in Go.'
## UnionRange class
Represents union range.
```go
type UnionRange struct  {
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
|[GetFirstRow](./getfirstrow/) | Gets the index of the first row of the range. |
|[GetFirstColumn](./getfirstcolumn/) | Gets the index of the first column of the range. |
|[GetRowCount](./getrowcount/) | Gets the count of rows in the range. |
|[GetColumnCount](./getcolumncount/) | Gets the count of rows in the range. |
|[Merge](./merge/) | Combines a range of cells into a single cell. |
|[UnMerge](./unmerge/) | Unmerges merged cells of this range. |
|[PutValue](./putvalue/) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset. |
|[GetValue](./getvalue/) | Gets and sets the values of the range. |
|[SetValue](./setvalue/) | Gets and sets the values of the range. |
|[GetName](./getname/) | Gets or sets the name of the range. |
|[SetName](./setname/) | Gets or sets the name of the range. |
|[GetRefersTo](./getrefersto/) | Gets the range's refers to. |
|[GetHasRange](./gethasrange/) | Indicates whether this has range. |
|[GetHyperlinks](./gethyperlinks/) | Gets all hyperlink in the range. |
|[SetStyle](./setstyle/) | Sets the style of the range. |
|[ApplyStyle](./applystyle/) | Applies formats for a whole range. |
|[Copy](./copy/) | Copying the range with paste special options. |
|[GetEnumerator](./getenumerator/) | Gets the enumerator for cells in this Range. |
|[GetCellCount](./getcellcount/) | Gets all cell count in the range. |
|[GetRangeCount](./getrangecount/) | Gets the count of the ranges. |
|[GetRanges](./getranges/) | Gets all union ranges. |
|[SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | Sets out line borders around a range of cells. |
|[SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Sets the outline borders around a range of cells with same border style and color. |
|[Intersect_String](./intersect_string/) | Intersects another range. |
|[Intersect_UnionRange](./intersect_unionrange/) | Intersects another range. |
|[Intersect_RangeArray](./intersect_rangearray/) | Intersects another range. |
|[Union_String](./union_string/) | Union another range. |
|[Union_UnionRange](./union_unionrange/) | Union another range. |
|[Union_RangeArray](./union_rangearray/) | Union the ranges. |
