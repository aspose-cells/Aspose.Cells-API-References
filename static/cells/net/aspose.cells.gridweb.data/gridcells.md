##Class GridCells
Aspose.Cells.GridWeb.Data.GridCells class. Encapsulates a collection of GridCell objects
## GridCells class
Encapsulates a collection of [`GridCell`](../gridcell/) objects.
```csharp
public class GridCells : IEnumerable
```
## Properties
| Name | Description |
| --- | --- |
| [Columns](../../aspose.cells.gridweb.data/gridcells/columns/) { get; } | Gets the collection of [`GridColumn`](../gridcolumn/) objects that represents the individual columns in this worksheet. |
| [Count](../../aspose.cells.gridweb.data/gridcells/count/) { get; } | Gets the number of cells. |
| [FirstCell](../../aspose.cells.gridweb.data/gridcells/firstcell/) { get; } | Gets the first cell in this worksheet. |
| [Item](../../aspose.cells.gridweb.data/gridcells/item/) { get; } | Gets the [`GridCell`](../gridcell/) element at the specified cell row index and column index. (2 indexers) |
| [LastCell](../../aspose.cells.gridweb.data/gridcells/lastcell/) { get; } | Gets the last cell in this worksheet. |
| [MaxColumn](../../aspose.cells.gridweb.data/gridcells/maxcolumn/) { get; } | Maximum column index of cell which contains data or style. |
| [MaxDataColumn](../../aspose.cells.gridweb.data/gridcells/maxdatacolumn/) { get; } | Maximum column index of cell which contains data. |
| [MaxDataRow](../../aspose.cells.gridweb.data/gridcells/maxdatarow/) { get; } | Maximum row index of cell which contains data. |
| [MaxRow](../../aspose.cells.gridweb.data/gridcells/maxrow/) { get; } | Maximum row index of cell which contains data or style. |
| [MergedCells](../../aspose.cells.gridweb.data/gridcells/mergedcells/) { get; } | Gets the collection of merged cells. |
| [MinColumn](../../aspose.cells.gridweb.data/gridcells/mincolumn/) { get; } | Minimum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it). |
| [MinDataColumn](../../aspose.cells.gridweb.data/gridcells/mindatacolumn/) { get; } | Minimum column index of cell which contains data. |
| [MinDataRow](../../aspose.cells.gridweb.data/gridcells/mindatarow/) { get; } | Minimum row index of cell which contains data. |
| [MinRow](../../aspose.cells.gridweb.data/gridcells/minrow/) { get; } | Minimum row index of cell which contains data or style. |
| [RowEnumerator](../../aspose.cells.gridweb.data/gridcells/rowenumerator/) { get; } | Gets the rows enumerator |
| [Rows](../../aspose.cells.gridweb.data/gridcells/rows/) { get; } | Gets the collection of [`GridRow`](../gridrow/) objects that represents the individual rows in this worksheet. |
| [StandardHeight](../../aspose.cells.gridweb.data/gridcells/standardheight/) { get; set; } | Gets or sets the default row height in this worksheet,in unit of points. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridcells/standardheightpixels/) { get; set; } | Gets or sets the default row height in this worksheet,in unit of pixels. |
| [StandardWidth](../../aspose.cells.gridweb.data/gridcells/standardwidth/) { get; set; } | Gets or sets the default column width in the worksheet,in unit of characters. |
| [StandardWidthInch](../../aspose.cells.gridweb.data/gridcells/standardwidthinch/) { get; set; } | Gets or sets the default column width in the worksheet, in unit of inches. |
| [StandardWidthPixels](../../aspose.cells.gridweb.data/gridcells/standardwidthpixels/) { get; set; } | Gets or sets the default column width in the worksheet, in unit of pixels. |
## Methods
| Name | Description |
| --- | --- |
| [CheckCell](../../aspose.cells.gridweb.data/gridcells/checkcell/)(int, int) | Gets the [`GridCell`](../gridcell/) element or null at the specified cell row index and column index. |
| [CheckColumn](../../aspose.cells.gridweb.data/gridcells/checkcolumn/)(int) | Gets the [`GridColumn`](../gridcolumn/) element or null at the specified column index. |
| [CheckRow](../../aspose.cells.gridweb.data/gridcells/checkrow/)(int) | Gets the [`GridRow`](../gridrow/) element or null at the specified cell row index. |
| [Clear](../../aspose.cells.gridweb.data/gridcells/clear/)() | Clear all cells in the collection. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents/#clearcontents)(GridCellArea) | Clears contents of a range. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents/#clearcontents_1)(int, int, int, int) | Clears contents of a range. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats/#clearformats)(GridCellArea) | Clears formatting of a range. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats/#clearformats_1)(int, int, int, int) | Clears formatting of a range. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange/#clearrange)(GridCellArea) | Clears contents and formatting of a range. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange/#clearrange_1)(int, int, int, int) | Clears contents and formatting of a range. |
| [CopyColumn](../../aspose.cells.gridweb.data/gridcells/copycolumn/)(GridCells, int, int) | Copies data and formattings of a whole column. |
| [CopyColumns](../../aspose.cells.gridweb.data/gridcells/copycolumns/)(GridCells, int, int, int) | Copies data and formattings of a whole column. |
| [CopyRow](../../aspose.cells.gridweb.data/gridcells/copyrow/)(GridCells, int, int) | Copies data and formattings of a whole row. |
| [CopyRows](../../aspose.cells.gridweb.data/gridcells/copyrows/)(GridCells, int, int, int) | Copies data and formattings of some whole rows. |
| [DeleteBlankColumns](../../aspose.cells.gridweb.data/gridcells/deleteblankcolumns/)() | Delete all blank columns which do not contain any data. |
| [DeleteBlankRows](../../aspose.cells.gridweb.data/gridcells/deleteblankrows/)() | Delete all blank rows which do not contain any data. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn/#deletecolumn)(int) | Deletes a column. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn/#deletecolumn_1)(int, bool) | Deletes a column. |
| [DeleteColumns](../../aspose.cells.gridweb.data/gridcells/deletecolumns/)(int, int, bool) | Deletes several columns. |
| [DeleteRange](../../aspose.cells.gridweb.data/gridcells/deleterange/)(int, int, int, int, GridShiftType) | Deletes a range of cells and shift cells according to the shift option. |
| [DeleteRow](../../aspose.cells.gridweb.data/gridcells/deleterow/)(int) | Deletes a row. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows/#deleterows)(int, int) | Deletes several rows. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows/#deleterows_1)(int, int, bool) | Deletes multiple rows in the worksheet. |
| [Export](../../aspose.cells.gridweb.data/gridcells/export/)(int, int, int, int, bool, bool) | Exports data in the Cells collection of a WebWorksheet to a new DataTable object |
| [ExportArray](../../aspose.cells.gridweb.data/gridcells/exportarray/)(int, int, int, int) | Exports data in the `GridCells` collection to a two-dimension array object. |
| [GetCell](../../aspose.cells.gridweb.data/gridcells/getcell/)(int, int) | Gets the [`GridCell`](../gridcell/) element at the specified cell row index and column index. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/gridcells/getcolumnwidth/)(int) | Gets the width of the specified column |
| [GetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthinch/)(int) | Gets the width of the specified column, in units of inches. |
| [GetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthpixel/)(int) | Gets the width of the specified column, in units of pixel. |
| [GetEnumerator](../../aspose.cells.gridweb.data/gridcells/getenumerator/)() | Gets the rows enumerator |
| [GetRow](../../aspose.cells.gridweb.data/gridcells/getrow/)(int) | Gets the [`GridRow`](../gridrow/) element or at the specified cell row index. |
| [GetRowHeight](../../aspose.cells.gridweb.data/gridcells/getrowheight/)(int) | Gets the height of a specified row. |
| [GetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/getrowheightinch/)(int) | Gets the height of a specified row in unit of inches. |
| [GetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/getrowheightpixel/)(int) | Gets the height of a specified row in unit of pixel. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/getrowoutlinelevel/)(int) | Gets the outline level of the row. |
| [GetViewColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getviewcolumnwidthpixel/)(int) | Get the width in different view type. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns/#groupcolumns)(int, int) | Groups columns. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns/#groupcolumns_1)(int, int, bool) | Groups columns. |
| [GroupRows](../../aspose.cells.gridweb.data/gridcells/grouprows/)(int, int) | Groups rows. |
| [HideColumn](../../aspose.cells.gridweb.data/gridcells/hidecolumn/)(int) | Hides a column. |
| [HideRow](../../aspose.cells.gridweb.data/gridcells/hiderow/)(int) | Hides a row. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn/#insertcolumn)(int) | Inserts a new column into the worksheet. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn/#insertcolumn_1)(int, bool) | Inserts a new column into the worksheet. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns/#insertcolumns)(int, int) | Inserts some columns into the worksheet. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns/#insertcolumns_1)(int, int, bool) | Inserts some columns into the worksheet. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange/#insertrange)(GridCellArea, GridShiftType) | Inserts a range of cells and shift cells according to the shift option. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange/#insertrange_1)(GridCellArea, int, GridShiftType, bool) | Inserts a range of cells and shift cells according to the shift option. |
| [InsertRow](../../aspose.cells.gridweb.data/gridcells/insertrow/)(int) | Inserts a new row into the worksheet. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows/#insertrows)(int, int) | Inserts multiple rows into the worksheet. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows/#insertrows_1)(int, int, bool) | Inserts multiple rows into the worksheet. |
| [IsBlankColumn](../../aspose.cells.gridweb.data/gridcells/isblankcolumn/)(int) | Checks whether given column is blank(does not contain any data). |
| [IsColumnHidden](../../aspose.cells.gridweb.data/gridcells/iscolumnhidden/)(int) | Checks whether a column at given index is hidden. |
| [IsRowHidden](../../aspose.cells.gridweb.data/gridcells/isrowhidden/)(int) | Checks whether a row at given index is hidden. |
| [Merge](../../aspose.cells.gridweb.data/gridcells/merge/)(int, int, int, int) | Merges a specified range of cells into a single cell. |
| [MoveRange](../../aspose.cells.gridweb.data/gridcells/moverange/)(GridCellArea, int, int) | Moves the range. |
| [RemoveDuplicates](../../aspose.cells.gridweb.data/gridcells/removeduplicates/)(int, int, int, int) | Remove duplicate values in the range. |
| [RemoveFormulas](../../aspose.cells.gridweb.data/gridcells/removeformulas/)() | Removes all formula and replaces with the value of the formula. |
| [SetBorders](../../aspose.cells.gridweb.data/gridcells/setborders/)(int, int, int, int, SetBorderPosition, WebBorderStyle) | Sets borders for a cells range. |
| [SetColumnWidth](../../aspose.cells.gridweb.data/gridcells/setcolumnwidth/)(int, double) | Sets the width of the specified column. |
| [SetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthinch/)(int, double) | Sets column width in unit of inches. |
| [SetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthpixel/)(int, int) | Sets column width in unit of pixels. |
| [SetRowHeight](../../aspose.cells.gridweb.data/gridcells/setrowheight/)(int, double) | Sets the height of the specified row. |
| [SetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/setrowheightinch/)(int, double) | Sets row height in unit of inches. |
| [SetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/setrowheightpixel/)(int, int) | Sets row height in unit of pixels. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/setrowoutlinelevel/)(int, int) | Sets the outline level of the row. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle/#setstyle_1)(string, GridTableItemStyle) | Sets the style to a specified range of cells. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle/#setstyle)(int, int, int, int, GridTableItemStyle) | Sets the style to a specified range of cells. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort/#sort)(int, int, int, int, int, bool, bool, bool) | Sorts the datas ascend/decend top to bottom in a range of a Worksheet by specified column index. Sorts the datas ascend/decend left to right in a range of a Worksheet by specified row index. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort/#sort_1)(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) | Sorts the datas ascend/decend top to bottom in a range of a Worksheet by specified column index. Sorts the datas ascend/decend left to right in a range of a Worksheet by specified row index. |
| [UngroupColumns](../../aspose.cells.gridweb.data/gridcells/ungroupcolumns/)(int, int) | Ungroups columns. |
| [UngroupRows](../../aspose.cells.gridweb.data/gridcells/ungrouprows/)(int, int) | Ungroups rows. |
| [UnhideColumn](../../aspose.cells.gridweb.data/gridcells/unhidecolumn/)(int, double) | Unhides a column |
| [UnhideRow](../../aspose.cells.gridweb.data/gridcells/unhiderow/)(int) | Unhides a row. |
| [UnMerge](../../aspose.cells.gridweb.data/gridcells/unmerge/)(int, int, int, int) | Unmerges a specified range of merged cells. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/gridcells/cellindextoname/)(int, int) | Gets cell name according to its row and column indexes. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/gridcells/cellnametoindex/)(string, out int, out int) | Gets the cell row and column indexes according to its name |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/gridcells/columnindextoname/)(int) | Gets column name according to column index. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/gridcells/columnnametoindex/)(string) | Gets column index according to column name. |
### See Also
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)
