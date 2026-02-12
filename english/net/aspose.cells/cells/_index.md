---
title: Class Cells
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Cells class. Encapsulates a collection of cell relevant objects such as Cell Row ...etc
type: docs
url: /net/aspose.cells/cells/
---
## Cells class

Encapsulates a collection of cell relevant objects, such as [`Cell`](../cell/), [`Row`](../row/), ...etc.

```csharp
public class Cells : IDisposable, IEnumerable
```

## Properties

| Name | Description |
| --- | --- |
| [Columns](../../aspose.cells/cells/columns/) { get; } | Gets the collection of [`Column`](../column/) objects that represents the individual columns in this worksheet. |
| [Count](../../aspose.cells/cells/count/) { get; } | Gets the total count of instantiated Cell objects. |
| [CountLarge](../../aspose.cells/cells/countlarge/) { get; } | Gets the total count of instantiated Cell objects. |
| [FirstCell](../../aspose.cells/cells/firstcell/) { get; } | Gets the first cell in this worksheet. |
| [IsDefaultColumnHidden](../../aspose.cells/cells/isdefaultcolumnhidden/) { get; set; } |  |
| [IsDefaultRowHeightMatched](../../aspose.cells/cells/isdefaultrowheightmatched/) { get; set; } | Indicates that row height and default font height matches |
| [IsDefaultRowHidden](../../aspose.cells/cells/isdefaultrowhidden/) { get; set; } | Indicates whether the row is default hidden. |
| [Item](../../aspose.cells/cells/item/) { get; } | Gets the [`Cell`](../cell/) element at the specified cell row index and column index. (2 indexers) |
| [LastCell](../../aspose.cells/cells/lastcell/) { get; } | Gets the last cell in this worksheet. |
| [MaxColumn](../../aspose.cells/cells/maxcolumn/) { get; } | Maximum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it). |
| [MaxDataColumn](../../aspose.cells/cells/maxdatacolumn/) { get; } | Maximum column index of cell which contains data. |
| [MaxDataRow](../../aspose.cells/cells/maxdatarow/) { get; } | Maximum row index of cell which contains data. |
| [MaxDisplayRange](../../aspose.cells/cells/maxdisplayrange/) { get; } | Gets the max range which includes data, merged cells and shapes. |
| [MaxRow](../../aspose.cells/cells/maxrow/) { get; } | Maximum row index of cell which contains data or style. |
| [MemorySetting](../../aspose.cells/cells/memorysetting/) { get; set; } | Gets or sets the memory usage option for this cells. |
| [MergedCells](../../aspose.cells/cells/mergedcells/) { get; } | (**Obsolete.**) Gets the collection of merged cells. |
| [MinColumn](../../aspose.cells/cells/mincolumn/) { get; } | Minimum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it). |
| [MinDataColumn](../../aspose.cells/cells/mindatacolumn/) { get; } | Minimum column index of cell which contains data. |
| [MinDataRow](../../aspose.cells/cells/mindatarow/) { get; } | Minimum row index of cell which contains data. |
| [MinRow](../../aspose.cells/cells/minrow/) { get; } | Minimum row index of cell which contains data or style. |
| [MultiThreadReading](../../aspose.cells/cells/multithreadreading/) { get; set; } | Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false. |
| [OdsCellFields](../../aspose.cells/cells/odscellfields/) { get; } | Gets the list of fields of ods. |
| [PreserveString](../../aspose.cells/cells/preservestring/) { get; set; } | Gets or sets a value indicating whether all worksheet values are preserved as strings. Default is false. |
| [Ranges](../../aspose.cells/cells/ranges/) { get; } | Gets the collection of [`Range`](../range/) objects created at run time. |
| [Rows](../../aspose.cells/cells/rows/) { get; } | Gets the collection of [`Row`](../row/) objects that represents the individual rows in this worksheet. |
| [StandardHeight](../../aspose.cells/cells/standardheight/) { get; set; } | Gets or sets the default row height in this worksheet, in unit of points. |
| [StandardHeightInch](../../aspose.cells/cells/standardheightinch/) { get; set; } | Gets or sets the default row height in this worksheet, in unit of inches. |
| [StandardHeightPixels](../../aspose.cells/cells/standardheightpixels/) { get; set; } | Gets or sets the default row height in this worksheet, in unit of pixels. |
| [StandardWidth](../../aspose.cells/cells/standardwidth/) { get; set; } | Gets or sets the default column width in the worksheet, in unit of characters. |
| [StandardWidthInch](../../aspose.cells/cells/standardwidthinch/) { get; set; } | Gets or sets the default column width in the worksheet, in unit of inches. |
| [StandardWidthPixels](../../aspose.cells/cells/standardwidthpixels/) { get; set; } | Gets or sets the default column width in the worksheet, in unit of pixels. |
| [Style](../../aspose.cells/cells/style/) { get; set; } | Gets and sets the default style of the worksheet. |

## Methods

| Name | Description |
| --- | --- |
| [AddRange](../../aspose.cells/cells/addrange/)(Range) | Adds a range object reference to cells |
| [ApplyColumnStyle](../../aspose.cells/cells/applycolumnstyle/)(int, Style, StyleFlag) | Applies formats for a whole column. |
| [ApplyRowStyle](../../aspose.cells/cells/applyrowstyle/)(int, Style, StyleFlag) | Applies formats for a whole row. |
| [ApplyStyle](../../aspose.cells/cells/applystyle/)(Style, StyleFlag) | Applies formats for a whole worksheet. |
| [CheckCell](../../aspose.cells/cells/checkcell/)(int, int) | Gets the [`Cell`](../cell/) element or null at the specified cell row index and column index. |
| [CheckColumn](../../aspose.cells/cells/checkcolumn/)(int) | Gets the [`Column`](../column/) element or null at the specified column index. |
| [CheckRow](../../aspose.cells/cells/checkrow/)(int) | Gets the [`Row`](../row/) element or null at the specified cell row index. |
| [Clear](../../aspose.cells/cells/clear/)() | Clears all data of the worksheet. |
| [ClearContents](../../aspose.cells/cells/clearcontents/#clearcontents)(CellArea) | Clears contents of a range. |
| [ClearContents](../../aspose.cells/cells/clearcontents/#clearcontents_1)(int, int, int, int) | Clears contents of a range. |
| [ClearFormats](../../aspose.cells/cells/clearformats/#clearformats)(CellArea) | Clears formatting of a range. |
| [ClearFormats](../../aspose.cells/cells/clearformats/#clearformats_1)(int, int, int, int) | Clears formatting of a range. |
| [ClearMergedCells](../../aspose.cells/cells/clearmergedcells/)() | Clears all merged ranges. |
| [ClearRange](../../aspose.cells/cells/clearrange/#clearrange)(CellArea) | Clears contents and formatting of a range. |
| [ClearRange](../../aspose.cells/cells/clearrange/#clearrange_1)(int, int, int, int) | Clears contents and formatting of a range. |
| [ConvertStringToNumericValue](../../aspose.cells/cells/convertstringtonumericvalue/)() | Converts all string data in the worksheet to numeric value if possible. |
| [CopyColumn](../../aspose.cells/cells/copycolumn/)(Cells, int, int) | Copies data and formats of a whole column. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns)(Cells, int, int, int) | Copies data and formats of whole columns. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns_2)(Cells, int, int, int, int) | Copies data and formats of the whole columns. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns_1)(Cells, int, int, int, PasteOptions) | Copies data and formats of a whole column. |
| [CopyRow](../../aspose.cells/cells/copyrow/)(Cells, int, int) | Copies data and formats of a whole row. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows)(Cells, int, int, int) | Copies data and formats of some whole rows. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows_1)(Cells, int, int, int, CopyOptions) | Copies data and formats of some whole rows. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows_2)(Cells, int, int, int, CopyOptions, PasteOptions) | Copies data and formats of some whole rows. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_2)(string) | Creates a [`Range`](../range/) object from an address of the range. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_3)(string, string) | Creates a [`Range`](../range/) object from a range of cells. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange)(int, int, bool) | Creates a [`Range`](../range/) object from rows of cells or columns of cells. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_1)(int, int, int, int) | Creates a [`Range`](../range/) object from a range of cells. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns/#deleteblankcolumns)() | Delete all blank columns which do not contain any data. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns/#deleteblankcolumns_1)(DeleteOptions) | Delete all blank columns which do not contain any data. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows/#deleteblankrows)() | Delete all blank rows which do not contain any data or other object. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows/#deleteblankrows_1)(DeleteOptions) | Delete all blank rows which do not contain any data or some special objects such as visible comment, pivot table. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn/#deletecolumn)(int) | Deletes a column. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn/#deletecolumn_1)(int, bool) | Deletes a column. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns/#deletecolumns_1)(int, int, bool) | Deletes several columns. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns/#deletecolumns)(int, int, DeleteOptions) | Deletes several columns. |
| [DeleteRange](../../aspose.cells/cells/deleterange/)(int, int, int, int, ShiftType) | Deletes a range of cells and shift cells according to the shift option. |
| [DeleteRow](../../aspose.cells/cells/deleterow/#deleterow)(int) | Deletes a row. |
| [DeleteRow](../../aspose.cells/cells/deleterow/#deleterow_1)(int, bool) | Deletes a row. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows)(int, int) | Deletes multiple rows. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows_2)(int, int, bool) | Deletes multiple rows in the worksheet. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows_1)(int, int, DeleteOptions) | Deletes multiple rows in the worksheet. |
| [Dispose](../../aspose.cells/cells/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn/#endcellincolumn)(int) | Gets the last cell in this column. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn/#endcellincolumn_1)(int, int, int, int) | Gets the last cell with maximum column index in this range. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow/#endcellinrow)(int) | Gets the last cell in this row. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow/#endcellinrow_1)(int, int, int, int) | Gets the last cell with maximum row index in this range. |
| [ExportArray](../../aspose.cells/cells/exportarray/)(int, int, int, int) | Exports data in the `Cells` collection to a two-dimension array object. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable)(int, int, int, int) | Exports data in the `Cells` collection to a DataTable object. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable_2)(int, int, int, int, bool) | Exports data in the `Cells` collection to a DataTable object. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable_1)(int, int, int, int, ExportTableOptions) | Exports data in the `Cells` collection to a DataTable object. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring/#exportdatatableasstring)(int, int, int, int) | Exports data in the `Cells` collection to a DataTable object. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring/#exportdatatableasstring_1)(int, int, int, int, bool) | Exports data in the `Cells` collection to a DataTable object. |
| [ExportList&lt;T&gt;](../../aspose.cells/cells/exportlist/)(int, int, int, int, ExportTableOptions) |  |
| [ExportTypeArray](../../aspose.cells/cells/exporttypearray/)(int, int, int, int) | Exports cell value type in the `Cells` collection to a two-dimension array object. |
| [Find](../../aspose.cells/cells/find/#find)(object, Cell) | Finds the cell containing with the input object. |
| [Find](../../aspose.cells/cells/find/#find_1)(object, Cell, FindOptions) | Finds the cell containing with the input object. |
| [GetCell](../../aspose.cells/cells/getcell/)(int, int) | (**Obsolete.**) Gets the [`Cell`](../cell/) element or null at the specified cell row index and column index. |
| [GetCellDisplayStyle](../../aspose.cells/cells/getcelldisplaystyle/#getcelldisplaystyle)(int, int) | Get the display style of given cell. |
| [GetCellDisplayStyle](../../aspose.cells/cells/getcelldisplaystyle/#getcelldisplaystyle_1)(int, int, BorderType) | Get the display style of given cell. |
| [GetCellStyle](../../aspose.cells/cells/getcellstyle/)(int, int) | Get the style of given cell. |
| [GetCellsWithPlaceInCellPicture](../../aspose.cells/cells/getcellswithplaceincellpicture/)() | Gets all cells that contain embedded picture. |
| [GetColumnOriginalWidthPoint](../../aspose.cells/cells/getcolumnoriginalwidthpoint/)(int) | (**Obsolete.**) Gets original column's height in unit of point if the column is hidden |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth/#getcolumnwidth)(int) | Gets the width(in unit of characters) of the specified column in normal view |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth/#getcolumnwidth_1)(int, bool, CellsUnitType) | Gets the column width. |
| [GetColumnWidthInch](../../aspose.cells/cells/getcolumnwidthinch/)(int) | (**Obsolete.**) Gets the width of the specified column in normal view, in units of inches. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel/#getcolumnwidthpixel)(int) | Gets the width of the specified column in normal view, in units of pixel. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel/#getcolumnwidthpixel_1)(int, bool) | (**Obsolete.**) Gets the width of the specified column in normal view, in units of pixel. |
| [GetDependents](../../aspose.cells/cells/getdependents/)(bool, int, int) | Get all cells which refer to the specific cell. |
| [GetDependentsInCalculation](../../aspose.cells/cells/getdependentsincalculation/)(int, int, bool) | Gets all cells whose calculated result depends on specific cell. |
| [GetEnumerator](../../aspose.cells/cells/getenumerator/)() | Gets the cells enumerator. |
| [GetFirstDataRow](../../aspose.cells/cells/getfirstdatarow/)(int) | Gets the first row index of cell which contains data in the specified column. |
| [GetGroupedColumnOutlineLevel](../../aspose.cells/cells/getgroupedcolumnoutlinelevel/)(int) | Gets the outline level (zero-based) of the column. |
| [GetGroupedRowOutlineLevel](../../aspose.cells/cells/getgroupedrowoutlinelevel/)(int) | Gets the outline level (zero-based) of the row. |
| [GetLastDataRow](../../aspose.cells/cells/getlastdatarow/)(int) | Gets the last row index of cell which contains data in the specified column. |
| [GetMaxGroupedColumnOutlineLevel](../../aspose.cells/cells/getmaxgroupedcolumnoutlinelevel/)() | Gets the max grouped column outline level (zero-based). |
| [GetMaxGroupedRowOutlineLevel](../../aspose.cells/cells/getmaxgroupedrowoutlinelevel/)() | Gets the max grouped row outline level (zero-based). |
| [GetMergedAreas](../../aspose.cells/cells/getmergedareas/)() | Gets all merged cells. |
| [GetRow](../../aspose.cells/cells/getrow/)(int) | (**Obsolete.**) Gets the [`Row`](../row/) element at the specified cell row index. |
| [GetRowEnumerator](../../aspose.cells/cells/getrowenumerator/)() | (**Obsolete.**) Gets the rows enumerator. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight/#getrowheight)(int) | Gets the height of a specified row, in unit of points. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight/#getrowheight_1)(int, bool, CellsUnitType) | Gets row's height. |
| [GetRowHeightInch](../../aspose.cells/cells/getrowheightinch/)(int) | Gets the height of a specified row in unit of inches. |
| [GetRowHeightPixel](../../aspose.cells/cells/getrowheightpixel/)(int) | Gets the height of a specified row in unit of pixel. |
| [GetRowOriginalHeightPoint](../../aspose.cells/cells/getroworiginalheightpoint/)(int) | (**Obsolete.**) Gets original row's height in unit of point if the row is hidden |
| [GetViewColumnWidthPixel](../../aspose.cells/cells/getviewcolumnwidthpixel/)(int) | Get the width in different view type. |
| [GetViewRowHeight](../../aspose.cells/cells/getviewrowheight/)(int) | Gets the height of a specified row. |
| [GetViewRowHeightInch](../../aspose.cells/cells/getviewrowheightinch/)(int) | Gets the height of a specified row in unit of inches. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns/#groupcolumns)(int, int) | Groups columns. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns/#groupcolumns_1)(int, int, bool) | Groups columns. |
| [GroupRows](../../aspose.cells/cells/grouprows/#grouprows)(int, int) | Groups rows. |
| [GroupRows](../../aspose.cells/cells/grouprows/#grouprows_1)(int, int, bool) | Groups rows. |
| [HideColumn](../../aspose.cells/cells/hidecolumn/)(int) | Hides a column. |
| [HideColumns](../../aspose.cells/cells/hidecolumns/)(int, int) | Hide multiple columns. |
| [HideGroupDetail](../../aspose.cells/cells/hidegroupdetail/)(bool, int) | Collapses the grouped rows/columns. |
| [HideRow](../../aspose.cells/cells/hiderow/)(int) | Hides a row. |
| [HideRows](../../aspose.cells/cells/hiderows/)(int, int) | Hides multiple rows. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray)(double[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_2)(int[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_4)(string[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_1)(double[], int, int, bool) | Imports an array of double into a worksheet. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_3)(int[], int, int, bool) | Imports an array of integer into a worksheet. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_5)(string[], int, int, bool) | Imports an array of string into a worksheet. |
| [ImportArrayList](../../aspose.cells/cells/importarraylist/)(ArrayList, int, int, bool) | Imports an arraylist of data into a worksheet. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv)(Stream, TxtLoadOptions, int, int) | Import a CSV file to the cells. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_2)(string, TxtLoadOptions, int, int) | Import a CSV file to the cells. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_1)(Stream, string, bool, int, int) | Import a CSV file to the cells. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_3)(string, string, bool, int, int) | Import a CSV file to the cells. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects/#importcustomobjects)(ICollection, int, int, ImportTableOptions) | Imports custom objects. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects/#importcustomobjects_1)(ICollection, string[], bool, int, int, int, bool, string, bool) | Imports custom objects. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_3)(IDataReader, int, int) | Imports data from a IDataReader object. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_1)(DataTable, int, int, ImportTableOptions) | Import data from custom data table. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_2)(DataView, int, int, ImportTableOptions) | Import data from data view. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata)(ICellsDataTable, int, int, ImportTableOptions) | Import data from custom data table. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_4)(IDataReader, int, int, ImportTableOptions) | Imports data from a IDataReader object. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid)(DataGrid, int, int, bool) | Imports a DataGrid into a worksheet. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid_1)(DataGrid, int, int, int, int, bool) | Imports a DataGrid into a worksheet. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid_2)(DataGrid, int, int, int, int, bool, bool) | Imports a DataGrid into a worksheet. |
| [ImportDataGridAsString](../../aspose.cells/cells/importdatagridasstring/)(DataGrid, int, int, bool) | Imports a DataGrid into a worksheet. This method doesn't try to convert text into numeric values. |
| [ImportDataRow](../../aspose.cells/cells/importdatarow/)(DataRow, int, int) | Imports a DataRow into the Excel file. |
| [ImportDataView](../../aspose.cells/cells/importdataview/)(DataView, int, int) | Imports a DataView into a worksheet. |
| [ImportFormulaArray](../../aspose.cells/cells/importformulaarray/)(string[], int, int, bool) | Imports an array of formula into a worksheet. |
| [ImportGridView](../../aspose.cells/cells/importgridview/)(GridView, int, int, ImportTableOptions) | Imports a grid view to this cells. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray/#importobjectarray)(object[], int, int, bool) | Imports an array of data into a worksheet. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray/#importobjectarray_1)(object[], int, int, bool, int) | Imports an array of data into a worksheet. |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray)(object[], int, int) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_1)(object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_3)(object[], object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_2)(object[], object[], int, int, TxtLoadOptions) |  |
| [InsertColumn](../../aspose.cells/cells/insertcolumn/#insertcolumn)(int) | Inserts a new column into the worksheet. |
| [InsertColumn](../../aspose.cells/cells/insertcolumn/#insertcolumn_1)(int, bool) | Inserts a new column into the worksheet. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns)(int, int) | Inserts some columns into the worksheet. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns_2)(int, int, bool) | Inserts some columns into the worksheet. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns_1)(int, int, InsertOptions) | Inserts some columns into the worksheet. |
| [InsertCutCells](../../aspose.cells/cells/insertcutcells/)(Range, int, int, ShiftType) | Insert cut range. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange)(CellArea, ShiftType) | Inserts a range of cells and shift cells according to the shift option. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange_1)(CellArea, int, ShiftType) | Inserts a range of cells and shift cells according to the shift option. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange_2)(CellArea, int, ShiftType, bool) | Inserts a range of cells and shift cells according to the shift option. |
| [InsertRow](../../aspose.cells/cells/insertrow/)(int) | Inserts a new row into the worksheet. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows)(int, int) | Inserts multiple rows into the worksheet. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows_2)(int, int, bool) | Inserts multiple rows into the worksheet. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows_1)(int, int, InsertOptions) | Inserts multiple rows into the worksheet. |
| [IsBlankColumn](../../aspose.cells/cells/isblankcolumn/)(int) | Checks whether given column is blank(does not contain any data). |
| [IsColumnHidden](../../aspose.cells/cells/iscolumnhidden/)(int) | Checks whether a column at given index is hidden. |
| [IsDeletingRangeEnabled](../../aspose.cells/cells/isdeletingrangeenabled/)(int, int, int, int) | Check whether the range could be deleted. |
| [IsRowHidden](../../aspose.cells/cells/isrowhidden/)(int) | Checks whether a row at given index is hidden. |
| [LinkToXmlMap](../../aspose.cells/cells/linktoxmlmap/)(string, int, int, string) | Link to a xml map. |
| [Merge](../../aspose.cells/cells/merge/#merge)(int, int, int, int) | Merges a specified range of cells into a single cell. |
| [Merge](../../aspose.cells/cells/merge/#merge_1)(int, int, int, int, bool) | Merges a specified range of cells into a single cell. |
| [Merge](../../aspose.cells/cells/merge/#merge_2)(int, int, int, int, bool, bool) | Merges a specified range of cells into a single cell. |
| [MoveRange](../../aspose.cells/cells/moverange/)(CellArea, int, int) | Moves the range. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates)() | Removes duplicate rows in the sheet. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates_1)(int, int, int, int) | Removes duplicate values in the range. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates_2)(int, int, int, int, bool, int[]) | Removes duplicate data of the range. |
| [RemoveFormulas](../../aspose.cells/cells/removeformulas/)() | Removes all formula and replaces with the value of the formula. |
| [RetrieveSubtotalSetting](../../aspose.cells/cells/retrievesubtotalsetting/)(CellArea) | Retrieves subtotals setting of the range. |
| [SetColumnWidth](../../aspose.cells/cells/setcolumnwidth/)(int, double) | Sets the width of the specified column in normal view. |
| [SetColumnWidthInch](../../aspose.cells/cells/setcolumnwidthinch/)(int, double) | Sets column width in unit of inches in normal view. |
| [SetColumnWidthPixel](../../aspose.cells/cells/setcolumnwidthpixel/)(int, int) | Sets column width in unit of pixels in normal view. |
| [SetRowHeight](../../aspose.cells/cells/setrowheight/)(int, double) | Sets the height of the specified row. |
| [SetRowHeightInch](../../aspose.cells/cells/setrowheightinch/)(int, double) | Sets row height in unit of inches. |
| [SetRowHeightPixel](../../aspose.cells/cells/setrowheightpixel/)(int, int) | Sets row height in unit of pixels. |
| [SetViewColumnWidthPixel](../../aspose.cells/cells/setviewcolumnwidthpixel/)(int, int) | Sets the width of the column in different view. |
| [ShowGroupDetail](../../aspose.cells/cells/showgroupdetail/)(bool, int) | Expands the grouped rows/columns. |
| [Subtotal](../../aspose.cells/cells/subtotal/#subtotal)(CellArea, int, ConsolidationFunction, int[]) | Creates subtotals for the range. |
| [Subtotal](../../aspose.cells/cells/subtotal/#subtotal_1)(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) | Creates subtotals for the range. |
| [TextToColumns](../../aspose.cells/cells/texttocolumns/)(int, int, int, TxtLoadOptions) | Splits content in specified column into multiple columns.. |
| [UngroupColumns](../../aspose.cells/cells/ungroupcolumns/)(int, int) | Ungroups columns. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows/#ungrouprows)(int, int) | Ungroups rows. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows/#ungrouprows_1)(int, int, bool) | Ungroups rows. |
| [UnhideColumn](../../aspose.cells/cells/unhidecolumn/)(int, double) | Unhides a column |
| [UnhideColumns](../../aspose.cells/cells/unhidecolumns/)(int, int, double) | Unhide multiple columns. |
| [UnhideRow](../../aspose.cells/cells/unhiderow/)(int, double) | Unhides a row. |
| [UnhideRows](../../aspose.cells/cells/unhiderows/)(int, int, double) | Unhides the hidden rows. |
| [UnMerge](../../aspose.cells/cells/unmerge/)(int, int, int, int) | Unmerges a specified range of merged cells. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsDemo
    {
        public static void CellsExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Set default row height
            cells.StandardHeight = 20;
            // Set row height
            cells.SetRowHeight(2, 20.5);

            // Set default column width
            cells.StandardWidth = 15;
            // Set column width
            cells.SetColumnWidth(3, 12.57);

            // Merge cells
            cells.Merge(5, 4, 2, 2);

            // Put values to cells
            cells[0, 0].PutValue(true);
            cells[0, 1].PutValue(1);
            cells[0, 2].PutValue("abc");

            // Export data
            object[,] arr = cells.ExportArray(0, 0, 10, 10);

            // Demonstrate some properties
            Console.WriteLine("Total Cells Count: " + cells.Count);
            Console.WriteLine("Total Cells Count (Large): " + cells.CountLarge);
            Console.WriteLine("Min Row with Data: " + cells.MinDataRow);
            Console.WriteLine("Max Row with Data: " + cells.MaxDataRow);
            Console.WriteLine("Min Column with Data: " + cells.MinDataColumn);
            Console.WriteLine("Max Column with Data: " + cells.MaxDataColumn);

            // Iterate through cells
            IEnumerator enumerator = cells.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }

            // Save the workbook
            workbook.Save("CellsExample.xlsx");
            workbook.Save("CellsExample.pdf");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


