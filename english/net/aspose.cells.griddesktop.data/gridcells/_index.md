---
title: GridCells
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 410
url: /net/aspose.cells.griddesktop.data/gridcells/
---
## GridCells class

Encapsulates a collection of Cell objects.

```csharp
public class GridCells : IEnumerable
```

## Properties

| Name | Description |
| --- | --- |
| [Columns](../../aspose.cells.griddesktop.data/gridcells/columns) { get; } |  |
| [Count](../../aspose.cells.griddesktop.data/gridcells/count) { get; } | Gets the number of cells. |
| [FirstCell](../../aspose.cells.griddesktop.data/gridcells/firstcell) { get; } |  |
| [Item](../../aspose.cells.griddesktop.data/gridcells/item) { get; } | Gets Cell item within the worksheet (3 indexers) |
| [LastCell](../../aspose.cells.griddesktop.data/gridcells/lastcell) { get; } |  |
| [MaxColumn](../../aspose.cells.griddesktop.data/gridcells/maxcolumn) { get; } | Maximum column index of cell which contains data or style. |
| [MaxDataColumn](../../aspose.cells.griddesktop.data/gridcells/maxdatacolumn) { get; } |  |
| [MaxDataRow](../../aspose.cells.griddesktop.data/gridcells/maxdatarow) { get; } |  |
| [MaxRow](../../aspose.cells.griddesktop.data/gridcells/maxrow) { get; } | Maximum row index of cell which contains data or style. |
| [MergedCells](../../aspose.cells.griddesktop.data/gridcells/mergedcells) { get; } | Gets the collection of merged cells. |
| [MinColumn](../../aspose.cells.griddesktop.data/gridcells/mincolumn) { get; } |  |
| [MinDataColumn](../../aspose.cells.griddesktop.data/gridcells/mindatacolumn) { get; } |  |
| [MinDataRow](../../aspose.cells.griddesktop.data/gridcells/mindatarow) { get; } |  |
| [MinRow](../../aspose.cells.griddesktop.data/gridcells/minrow) { get; } |  |
| [RowEnumerator](../../aspose.cells.griddesktop.data/gridcells/rowenumerator) { get; } | Gets the rows enumerator |
| [Rows](../../aspose.cells.griddesktop.data/gridcells/rows) { get; } | Gets the collection of [`GridRow`](../gridrow) objects that represents the individual rows in this worksheet. |
| [StandardHeight](../../aspose.cells.griddesktop.data/gridcells/standardheight) { get; set; } | Gets or sets the default row height in this worksheet,in unit of points. |
| [StandardHeightPixels](../../aspose.cells.griddesktop.data/gridcells/standardheightpixels) { get; set; } | Gets or sets the default row height in this worksheet,in unit of pixels. |
| [StandardWidth](../../aspose.cells.griddesktop.data/gridcells/standardwidth) { get; set; } | Gets or sets the default column width in the worksheet,in unit of characters. |
| [StandardWidthInch](../../aspose.cells.griddesktop.data/gridcells/standardwidthinch) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.griddesktop.data/gridcells/standardwidthpixels) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [CheckCell](../../aspose.cells.griddesktop.data/gridcells/checkcell)(int, int) | Gets the Cell element or null at the specified cell row index and column index. |
| [Clear](../../aspose.cells.griddesktop.data/gridcells/clear)() | Clear all cells in the collection. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents)(GridCellArea) | Clears contents of a range. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents)(int, int, int, int) | Clears contents of a range. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats)(GridCellArea) | Clears formatting of a range. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats)(int, int, int, int) | Clears formatting of a range. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange)(GridCellArea) | Clears contents and formatting of a range. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange)(int, int, int, int) | Clears contents and formatting of a range. |
| [CopyColumn](../../aspose.cells.griddesktop.data/gridcells/copycolumn)(GridCells, int, int) | Copies data and formattings of a whole column. |
| [CopyColumns](../../aspose.cells.griddesktop.data/gridcells/copycolumns)(GridCells, int, int, int) | Copies data and formattings of a whole column. |
| [CopyRow](../../aspose.cells.griddesktop.data/gridcells/copyrow)(GridCells, int, int) | Copies data and formattings of a whole row. |
| [CopyRows](../../aspose.cells.griddesktop.data/gridcells/copyrows)(GridCells, int, int, int) | Copies data and formattings of some whole rows. |
| [DeleteBlankColumns](../../aspose.cells.griddesktop.data/gridcells/deleteblankcolumns)() | Delete all blank columns which do not contain any data. |
| [DeleteBlankRows](../../aspose.cells.griddesktop.data/gridcells/deleteblankrows)() | Delete all blank rows which do not contain any data. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn)(int) | Deletes a column. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn)(int, bool) | Deletes a column. |
| [DeleteColumns](../../aspose.cells.griddesktop.data/gridcells/deletecolumns)(int, int, bool) | Deletes several columns. |
| [DeleteRow](../../aspose.cells.griddesktop.data/gridcells/deleterow)(int) | Deletes a row. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows)(int, int) | Deletes several rows. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows)(int, int, bool) | Deletes multiple rows in the worksheet. |
| [GetCell](../../aspose.cells.griddesktop.data/gridcells/getcell)(int, int) | Gets the Cell element or null at the specified cell row index and column index. |
| [GetCellStyle](../../aspose.cells.griddesktop.data/gridcells/getcellstyle)(int, int) | Get the style of given cell. |
| [GetColumn](../../aspose.cells.griddesktop.data/gridcells/getcolumn)(int) | Gets the [`GridColumn`](../gridcolumn) element or at the specified cell column index. |
| [GetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidth)(int) | Gets the width of the specified column |
| [GetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthinch)(int) | Gets the width of the specified column, in units of inches. |
| [GetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthpixel)(int) | Gets the width of the specified column, in units of pixel. |
| [GetEnumerator](../../aspose.cells.griddesktop.data/gridcells/getenumerator)() | Gets the rows enumerator |
| [GetRow](../../aspose.cells.griddesktop.data/gridcells/getrow)(int) | Gets the [`GridRow`](../gridrow) element or at the specified cell row index. |
| [GetRowHeight](../../aspose.cells.griddesktop.data/gridcells/getrowheight)(int) | Gets the height of a specified row. |
| [GetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/getrowheightinch)(int) | Gets the height of a specified row in unit of inches. |
| [GetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/getrowheightpixel)(int) | Gets the height of a specified row in unit of pixel. |
| [GetViewColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getviewcolumnwidthpixel)(int) | Get the width in different view type. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns)(int, int) | Groups columns. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns)(int, int, bool) | Groups columns. |
| [GroupRows](../../aspose.cells.griddesktop.data/gridcells/grouprows)(int, int) | Groups rows. |
| [HideColumn](../../aspose.cells.griddesktop.data/gridcells/hidecolumn)(int) | Hides a column. |
| [HideRow](../../aspose.cells.griddesktop.data/gridcells/hiderow)(int) | Hides a row. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn)(int) | Inserts a new column into the worksheet. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn)(int, bool) | Inserts a new column into the worksheet. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns)(int, int) | Inserts some columns into the worksheet. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns)(int, int, bool) | Inserts some columns into the worksheet. |
| [InsertRow](../../aspose.cells.griddesktop.data/gridcells/insertrow)(int) | Inserts a new row into the worksheet. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows)(int, int) | Inserts multiple rows into the worksheet. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows)(int, int, bool) | Inserts multiple rows into the worksheet. |
| [IsBlankColumn](../../aspose.cells.griddesktop.data/gridcells/isblankcolumn)(int) | Checks whether given column is blank(does not contain any data). |
| [IsColumnHidden](../../aspose.cells.griddesktop.data/gridcells/iscolumnhidden)(int) | Checks whether a column at given index is hidden. |
| [IsRowHidden](../../aspose.cells.griddesktop.data/gridcells/isrowhidden)(int) | Checks whether a row at given index is hidden. |
| [Merge](../../aspose.cells.griddesktop.data/gridcells/merge)(int, int, int, int) | Merges a specified range of cells into a single cell. |
| [RemoveFormulas](../../aspose.cells.griddesktop.data/gridcells/removeformulas)() | Removes all formula and replaces with the value of the formula. |
| [SetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidth)(int, double) | Sets the width of the specified column. |
| [SetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthinch)(int, double) | Sets column width in unit of inches. |
| [SetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthpixel)(int, int) | Sets column width in unit of pixels. |
| [SetRowHeight](../../aspose.cells.griddesktop.data/gridcells/setrowheight)(int, double) | Sets the height of the specified row. |
| [SetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/setrowheightinch)(int, double) | Sets row height in unit of inches. |
| [SetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/setrowheightpixel)(int, int) | Sets row height in unit of pixels. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle)(string, Style) | Sets the style to a specified range of cells. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle)(int, int, int, int, Style) | Sets the style to a specified range of cells. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort)(int, int, int, int, int, bool, bool, bool) | Sorts the datas ascend/decend top to bottom in a range of a Worksheet by specified column index. Sorts the datas ascend/decend left to right in a range of a Worksheet by specified row index. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) |  |
| [UngroupColumns](../../aspose.cells.griddesktop.data/gridcells/ungroupcolumns)(int, int) | Ungroups columns. |
| [UngroupRows](../../aspose.cells.griddesktop.data/gridcells/ungrouprows)(int, int) | Ungroups rows. |
| [UnhideColumn](../../aspose.cells.griddesktop.data/gridcells/unhidecolumn)(int, double) | Unhides a column |
| [UnhideRow](../../aspose.cells.griddesktop.data/gridcells/unhiderow)(int) | Unhides a row. |
| [UnMerge](../../aspose.cells.griddesktop.data/gridcells/unmerge)(int, int, int, int) | Unmerges a specified range of merged cells. |
| static [CellIndexToName](../../aspose.cells.griddesktop.data/gridcells/cellindextoname)(int, int) | Gets cell name according to its row and column indexes. |
| static [CellNameToIndex](../../aspose.cells.griddesktop.data/gridcells/cellnametoindex)(string, out int, out int) | Gets the cell row and column indexes according to its name |
| static [ColumnIndexToName](../../aspose.cells.griddesktop.data/gridcells/columnindextoname)(int) | Gets column name according to column index. |
| static [ColumnNameToIndex](../../aspose.cells.griddesktop.data/gridcells/columnnametoindex)(string) | Gets column index according to column name. |

### See Also

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data)
* assembly [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->