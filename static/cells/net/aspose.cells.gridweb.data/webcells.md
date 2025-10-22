##Class WebCells
Aspose.Cells.GridWeb.Data.WebCells class.
## WebCells class
```csharp
[Obsolete("This class is obsolete; use  GridCells instead")]
public class WebCells
```
## Properties
| Name | Description |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/webcells/count/) { get; } | Gets the number of cells. |
| [Item](../../aspose.cells.gridweb.data/webcells/item/) { get; } | Gets the Cell element at the specified cell row index and column index. (2 indexers) |
| [MaxColumn](../../aspose.cells.gridweb.data/webcells/maxcolumn/) { get; } |  |
| [MaxRow](../../aspose.cells.gridweb.data/webcells/maxrow/) { get; } |  |
| [MergedCells](../../aspose.cells.gridweb.data/webcells/mergedcells/) { get; } | Gets the collection of merged cells. |
| [MinColumn](../../aspose.cells.gridweb.data/webcells/mincolumn/) { get; } | Min column number of cell which contains data or style. |
| [MinRow](../../aspose.cells.gridweb.data/webcells/minrow/) { get; } | Min row number of cell which contains data or style. |
| [StandardHeight](../../aspose.cells.gridweb.data/webcells/standardheight/) { get; set; } | Gets or sets the default row height in this worksheet,in unit of points. |
| [StandardWidth](../../aspose.cells.gridweb.data/webcells/standardwidth/) { get; set; } | Gets or sets the default column width in the worksheet,in unit of characters. |
## Methods
| Name | Description |
| --- | --- |
| [Clear](../../aspose.cells.gridweb.data/webcells/clear/)() |  |
| [ClearContents](../../aspose.cells.gridweb.data/webcells/clearcontents/)(int, int, int, int) | Clears contents of a range. |
| [DeleteColumn](../../aspose.cells.gridweb.data/webcells/deletecolumn/)(int) | Deletes a column. |
| [DeleteRow](../../aspose.cells.gridweb.data/webcells/deleterow/)(int) | Deletes a row. |
| [DeleteRows](../../aspose.cells.gridweb.data/webcells/deleterows/)(int, int) | Deletes a number of rows. This method is much faster than DeleteRow when doing a batch row deleting. |
| [Export](../../aspose.cells.gridweb.data/webcells/export/)(int, int, int, int, bool, bool) | Exports data in the Cells collection of a WebWorksheet to a new DataTable object |
| [ExportArray](../../aspose.cells.gridweb.data/webcells/exportarray/)(int, int, int, int) | Exports data in the Cells collection to a two-dimension array object. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/webcells/getcolumncaption/)(int) | Gets the column caption. If the caption is not set, returns empty string. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/webcells/getcolumnreadonly/)(int) | Gets if a column is readonly. this is extended method of GridWeb specifically,it will not keep and take affect in actual excel file |
| [GetColumnWidth](../../aspose.cells.gridweb.data/webcells/getcolumnwidth/)(int) | Gets the width of the specified column |
| [GetEnumerator](../../aspose.cells.gridweb.data/webcells/getenumerator/)() | Gets the cells enumerator |
| [GetRowCaption](../../aspose.cells.gridweb.data/webcells/getrowcaption/)(int) | Gets the row caption. If the caption is not set, returns empty string. |
| [GetRowHeight](../../aspose.cells.gridweb.data/webcells/getrowheight/)(int) | Gets the height of a specified row. |
| [GetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/getrowhiddenstatus/)(int) | Get hidden status of a specified row. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/getrowoutlinelevel/)(int) | Gets the outline level of the row. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/webcells/getrowreadonly/)(int) | Gets if a row is readonly. this is extended method of GridWeb specifically,it will not keep and take affect in actual excel file |
| [InsertColumn](../../aspose.cells.gridweb.data/webcells/insertcolumn/)(int) | Inserts a new column into the worksheet. |
| [InsertRow](../../aspose.cells.gridweb.data/webcells/insertrow/)(int) | Inserts a new row into the worksheet. |
| [InsertRows](../../aspose.cells.gridweb.data/webcells/insertrows/)(int, int) | Inserts multiple rows into the worksheet. |
| [Merge](../../aspose.cells.gridweb.data/webcells/merge/)(int, int, int, int) |  |
| [SetBorders](../../aspose.cells.gridweb.data/webcells/setborders/)(int, int, int, int, SetBorderPosition, WebBorderStyle) | Sets borders for a cells range. |
| [SetColumnCaption](../../aspose.cells.gridweb.data/webcells/setcolumncaption/)(int, string) | Sets the caption for the column.please note this is an extension attribute and can not keep in excel file |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/webcells/setcolumnreadonly/)(int, bool) | Sets a column to readonly so user can't delete it from client side. this is extended method of GridWeb specifically,it will not keep and take affect in actual excel file |
| [SetColumnWidth](../../aspose.cells.gridweb.data/webcells/setcolumnwidth/)(int, Unit) | Sets the width of the specified column.the accepted width type is Point,Pixel or Inch |
| [SetRowCaption](../../aspose.cells.gridweb.data/webcells/setrowcaption/)(int, string) | Sets the caption for the row. |
| [SetRowHeight](../../aspose.cells.gridweb.data/webcells/setrowheight/)(int, Unit) | Sets the height of the specified row.the accepted width type is Point,Pixel or Inch |
| [SetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/setrowhiddenstatus/)(int, bool) | Set hidden status of a specified row. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevel/)(int, int) | Sets the outline level of the row. |
| [SetRowOutlineLevelAndStatus](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevelandstatus/)(int, int, bool) | Sets the outline level of the row. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/webcells/setrowreadonly/)(int, bool) | Sets a row to readonly so user can't delete it from client side. this is extended method of GridWeb specifically,it will not keep and take affect in actual excel file |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle_1)(string, TableItemStyle) | Sets the style to a specified range of cells. |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle)(int, int, int, int, TableItemStyle) | Sets the style to a specified range of cells. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort)(int, int, int, int, int) | Sorts the datas ascend top to bottom in a range of a WebWorksheet by specified column index. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_2)(int, int, int, int, int[]) | Sorts the datas ascend top to bottom in a range of a WebWorksheet by some field that are specifed by column indexes array. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_1)(int, int, int, int, int, SortByOrder, SortOrientation, bool) | Sorts the datas ascend top to bottom in a range of a WebWorksheet by specified column index. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_3)(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) | Sorts the datas ascend in a range of a WebWorksheet by some field that are specifed by indexes array. |
| [UnMerge](../../aspose.cells.gridweb.data/webcells/unmerge/)(int, int, int, int) | Unmerges a specified range of merged cells. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/webcells/cellindextoname/)(int, int) | Gets cell name according to its row and column indexes. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/webcells/cellnametoindex/)(string, out int, out int) | Gets the cell row and column indexes according to its name |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/webcells/columnindextoname/)(int) | Gets column name according to column index. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/webcells/columnnametoindex/)(string) | Gets column index according to column name. |
### Remarks
NOTE: This class is now obsolete. please use GridCells Instead. This class will be removed after 6 months since Aug. 2014. Aspose apologizes for any inconvenience you may have experienced.
### See Also
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)
