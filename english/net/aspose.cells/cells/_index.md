---
title: Cells
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 300
url: /net/aspose.cells/cells/
---
## Cells class

Encapsulates a collection of cell relevant objects, such as [`Cell`](../cell), [`Row`](../row), ...etc.

```csharp
public class Cells : IDisposable, IEnumerable
```

## Properties

| Name | Description |
| --- | --- |
| [Columns](columns) { get; } | Gets the collection of [`Column`](../column) objects that represents the individual columns in this worksheet. |
| [Count](count) { get; } | Gets the total count of instantiated Cell objects. |
| [CountLarge](countlarge) { get; } | Gets the total count of instantiated Cell objects. |
| [FirstCell](firstcell) { get; } | Gets the first cell in this worksheet. |
| [IsDefaultRowHeightMatched](isdefaultrowheightmatched) { get; set; } | Indicates that row height and default font height matches |
| [IsDefaultRowHidden](isdefaultrowhidden) { get; set; } | Indicates whether the row is default hidden. |
| [Item](item) { get; } | Gets the [`Cell`](../cell) element at the specified cell row index and column index. (2 indexers) |
| [LastCell](lastcell) { get; } | Gets the last cell in this worksheet. |
| [MaxColumn](maxcolumn) { get; } | Minimum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it). |
| [MaxDataColumn](maxdatacolumn) { get; } | Maximum column index of cell which contains data. |
| [MaxDataRow](maxdatarow) { get; } | Maximum row index of cell which contains data. |
| [MaxDisplayRange](maxdisplayrange) { get; } | Gets the max range which includes data, merged cells and shapes. |
| [MaxRow](maxrow) { get; } | Maximum row index of cell which contains data or style. |
| [MemorySetting](memorysetting) { get; set; } | Gets or sets the memory usage option for this cells. |
| [MergedCells](mergedcells) { get; } | Gets the collection of merged cells. |
| [MinColumn](mincolumn) { get; } | Minimum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it). |
| [MinDataColumn](mindatacolumn) { get; } | Minimum column index of cell which contains data. |
| [MinDataRow](mindatarow) { get; } | Minimum row index of cell which contains data. |
| [MinRow](minrow) { get; } | Minimum row index of cell which contains data or style. |
| [MultiThreadReading](multithreadreading) { get; set; } | Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false. |
| [OdsCellFields](odscellfields) { get; } | Gets the list of fields of ods. |
| [PreserveString](preservestring) { get; set; } | Gets or sets a value indicating whether all worksheet values are preserved as strings. Default is false. |
| [Ranges](ranges) { get; } | Gets the collection of [`Range`](../range) objects created at run time. |
| [Rows](rows) { get; } | Gets the collection of [`Row`](../row) objects that represents the individual rows in this worksheet. |
| [StandardHeight](standardheight) { get; set; } | Gets or sets the default row height in this worksheet, in unit of points. |
| [StandardHeightInch](standardheightinch) { get; set; } | Gets or sets the default row height in this worksheet, in unit of inches. |
| [StandardHeightPixels](standardheightpixels) { get; set; } | Gets or sets the default row height in this worksheet, in unit of pixels. |
| [StandardWidth](standardwidth) { get; set; } | Gets or sets the default column width in the worksheet, in unit of characters. |
| [StandardWidthInch](standardwidthinch) { get; set; } | Gets or sets the default column width in the worksheet, in unit of inches. |
| [StandardWidthPixels](standardwidthpixels) { get; set; } | Gets or sets the default column width in the worksheet, in unit of pixels. |
| [Style](style) { get; set; } | Gets and sets the default style. |

## Methods

| Name | Description |
| --- | --- |
| [AddRange](addrange)(Range) | Adds a range object reference to cells |
| [ApplyColumnStyle](applycolumnstyle)(int, Style, StyleFlag) | Applies formats for a whole column. |
| [ApplyRowStyle](applyrowstyle)(int, Style, StyleFlag) | Applies formats for a whole row. |
| [ApplyStyle](applystyle)(Style, StyleFlag) | Applies formats for a whole worksheet. |
| [CheckCell](checkcell)(int, int) | Gets the [`Cell`](../cell) element or null at the specified cell row index and column index. |
| [CheckColumn](checkcolumn)(int) | Gets the [`Column`](../column) element or null at the specified column index. |
| [CheckRow](checkrow)(int) | Gets the [`Row`](../row) element or at the specified cell row index. |
| [Clear](clear)() | Clears all cell and row objects. |
| [ClearContents](clearcontents)(CellArea) | Clears contents of a range. |
| [ClearContents](clearcontents)(int, int, int, int) | Clears contents of a range. |
| [ClearFormats](clearformats)(CellArea) | Clears formatting of a range. |
| [ClearFormats](clearformats)(int, int, int, int) | Clears formatting of a range. |
| [ClearMergedCells](clearmergedcells)() | Clears all merged ranges. |
| [ClearRange](clearrange)(CellArea) | Clears contents and formatting of a range. |
| [ClearRange](clearrange)(int, int, int, int) | Clears contents and formatting of a range. |
| [ConvertStringToNumericValue](convertstringtonumericvalue)() | Converts string data in cells to numeric value if possible. |
| [CopyColumn](copycolumn)(Cells, int, int) | Copies data and formats of a whole column. |
| [CopyColumns](copycolumns)(Cells, int, int, int) | Copies data and formats of a whole column. |
| [CopyColumns](copycolumns)(Cells, int, int, int, int) | Copies data and formats of the whole columns. |
| [CopyColumns](copycolumns)(Cells, int, int, int, PasteOptions) | Copies data and formats of a whole column. |
| [CopyRow](copyrow)(Cells, int, int) | Copies data and formats of a whole row. |
| [CopyRows](copyrows)(Cells, int, int, int) | Copies data and formats of some whole rows. |
| [CopyRows](copyrows)(Cells, int, int, int, CopyOptions) | Copies data and formats of some whole rows. |
| [CopyRows](copyrows)(Cells, int, int, int, CopyOptions, PasteOptions) | Copies data and formats of some whole rows. |
| [CreateRange](createrange)(string) | Creates a [`Range`](../range) object from an address of the range. |
| [CreateRange](createrange)(string, string) | Creates a [`Range`](../range) object from a range of cells. |
| [CreateRange](createrange)(int, int, bool) | Creates a [`Range`](../range) object from rows of cells or columns of cells. |
| [CreateRange](createrange)(int, int, int, int) | Creates a [`Range`](../range) object from a range of cells. |
| [DeleteBlankColumns](deleteblankcolumns)() | Delete all blank columns which do not contain any data. |
| [DeleteBlankColumns](deleteblankcolumns)(DeleteOptions) | Delete all blank columns which do not contain any data. |
| [DeleteBlankRows](deleteblankrows)() | Delete all blank rows which do not contain any data. |
| [DeleteBlankRows](deleteblankrows)(DeleteOptions) | Delete all blank rows which do not contain any data. |
| [DeleteColumn](deletecolumn)(int) | Deletes a column. |
| [DeleteColumn](deletecolumn)(int, bool) | Deletes a column. |
| [DeleteColumns](deletecolumns)(int, int, bool) | Deletes several columns. |
| [DeleteRange](deleterange)(int, int, int, int, ShiftType) | Deletes a range of cells and shift cells according to the shift option. |
| [DeleteRow](deleterow)(int) | Deletes a row. |
| [DeleteRows](deleterows)(int, int) | Deletes several rows. |
| [DeleteRows](deleterows)(int, int, bool) | Deletes multiple rows in the worksheet. |
| [Dispose](dispose)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [EndCellInColumn](endcellincolumn)(short) | Gets the last cell in this column. |
| [EndCellInColumn](endcellincolumn)(int, int, short, short) | Gets the last cell with maximum column index in this range. |
| [EndCellInRow](endcellinrow)(int) | Gets the last cell in this row. |
| [EndCellInRow](endcellinrow)(int, int, int, int) | Gets the last cell with maximum row index in this range. |
| [ExportArray](exportarray)(int, int, int, int) | Exports data in the [`Cells`](../cells) collection to a two-dimension array object. |
| [ExportDataTable](exportdatatable)(int, int, int, int) | Exports data in the [`Cells`](../cells) collection to a DataTable object. |
| [ExportDataTable](exportdatatable)(int, int, int, int, bool) | Exports data in the [`Cells`](../cells) collection to a DataTable object. |
| [ExportDataTable](exportdatatable)(int, int, int, int, ExportTableOptions) | Exports data in the [`Cells`](../cells) collection to a DataTable object. |
| [ExportDataTableAsString](exportdatatableasstring)(int, int, int, int) | Exports data in the [`Cells`](../cells) collection to a DataTable object. |
| [ExportDataTableAsString](exportdatatableasstring)(int, int, int, int, bool) | Exports data in the [`Cells`](../cells) collection to a DataTable object. |
| [ExportTypeArray](exporttypearray)(int, int, int, int) | Exports cell value type in the [`Cells`](../cells) collection to a two-dimension array object. |
| [Find](find)(object, Cell) | Finds the cell containing with the input object. |
| [Find](find)(object, Cell, FindOptions) | Finds the cell containing with the input object. |
| [GetCell](getcell)(int, int) | Gets the [`Cell`](../cell) element or null at the specified cell row index and column index. |
| [GetCellStyle](getcellstyle)(int, int) | Get the style of given cell. |
| [GetColumnWidth](getcolumnwidth)(int) | Gets the width of the specified column in normal view |
| [GetColumnWidthInch](getcolumnwidthinch)(int) | Gets the width of the specified column in normal view, in units of inches. |
| [GetColumnWidthPixel](getcolumnwidthpixel)(int) | Gets the width of the specified column in normal view, in units of pixel. |
| [GetDependents](getdependents)(bool, int, int) | Get all cells which refer to the specific cell. |
| [GetEnumerator](getenumerator)() | Gets the cells enumerator. |
| [GetGroupedColumnOutlineLevel](getgroupedcolumnoutlinelevel)(int) | Gets the outline level (zero-based) of the column. |
| [GetGroupedRowOutlineLevel](getgroupedrowoutlinelevel)(int) | Gets the outline level (zero-based) of the row. |
| [GetLastDataRow](getlastdatarow)(int) | Gets the last row index of cell which contains data in the specified column. |
| [GetMaxGroupedColumnOutlineLevel](getmaxgroupedcolumnoutlinelevel)() | Gets the max grouped column outline level (zero-based). |
| [GetMaxGroupedRowOutlineLevel](getmaxgroupedrowoutlinelevel)() | Gets the max grouped row outline level (zero-based). |
| [GetRow](getrow)(int) | Gets the [`Row`](../row) element at the specified cell row index. |
| [GetRowEnumerator](getrowenumerator)() | Gets the rows enumerator. |
| [GetRowHeight](getrowheight)(int) | Gets the height of a specified row. |
| [GetRowHeightInch](getrowheightinch)(int) | Gets the height of a specified row in unit of inches. |
| [GetRowHeightPixel](getrowheightpixel)(int) | Gets the height of a specified row in unit of pixel. |
| [GetViewColumnWidthPixel](getviewcolumnwidthpixel)(int) | Get the width in different view type. |
| [GetViewRowHeight](getviewrowheight)(int) | Gets the height of a specified row. |
| [GetViewRowHeightInch](getviewrowheightinch)(int) | Gets the height of a specified row in unit of inches. |
| [GroupColumns](groupcolumns)(int, int) | Groups columns. |
| [GroupColumns](groupcolumns)(int, int, bool) | Groups columns. |
| [GroupRows](grouprows)(int, int) | Groups rows. |
| [GroupRows](grouprows)(int, int, bool) | Groups rows. |
| [HideColumn](hidecolumn)(int) | Hides a column. |
| [HideColumns](hidecolumns)(int, int) | Hide multiple columns. |
| [HideGroupDetail](hidegroupdetail)(bool, int) | Collapses the grouped rows/columns. |
| [HideRow](hiderow)(int) | Hides a row. |
| [HideRows](hiderows)(int, int) | Hides multiple rows. |
| [ImportArray](importarray)(double[], int, int) |  |
| [ImportArray](importarray)(int[], int, int) |  |
| [ImportArray](importarray)(string[], int, int) |  |
| [ImportArray](importarray)(double[], int, int, bool) | Imports an array of double into a worksheet. |
| [ImportArray](importarray)(int[], int, int, bool) | Imports an array of integer into a worksheet. |
| [ImportArray](importarray)(string[], int, int, bool) | Imports an array of string into a worksheet. |
| [ImportArrayList](importarraylist)(ArrayList, int, int, bool) | Imports an arraylist of data into a worksheet. |
| [ImportCSV](importcsv)(Stream, TxtLoadOptions, int, int) | Import a CSV file to the cells. |
| [ImportCSV](importcsv)(string, TxtLoadOptions, int, int) | Import a CSV file to the cells. |
| [ImportCSV](importcsv)(Stream, string, bool, int, int) | Import a CSV file to the cells. |
| [ImportCSV](importcsv)(string, string, bool, int, int) | Import a CSV file to the cells. |
| [ImportCustomObjects](importcustomobjects)(ICollection, int, int, ImportTableOptions) | Imports custom objects. |
| [ImportCustomObjects](importcustomobjects)(ICollection, string[], bool, int, int, int, bool, string, bool) | Imports custom objects. |
| [ImportData](importdata)(IDataReader, int, int) | Imports data from a IDataReader object. |
| [ImportData](importdata)(DataTable, int, int, ImportTableOptions) | Import data from custom data table. |
| [ImportData](importdata)(DataView, int, int, ImportTableOptions) | Import data from data view. |
| [ImportData](importdata)(ICellsDataTable, int, int, ImportTableOptions) | Import data from custom data table. |
| [ImportData](importdata)(IDataReader, int, int, ImportTableOptions) | Imports data from a IDataReader object. |
| [ImportDataRow](importdatarow)(DataRow, int, int) | Imports a DataRow into the Excel file. |
| [ImportDataView](importdataview)(DataView, int, int) | Imports a DataView into a worksheet. |
| [ImportFormulaArray](importformulaarray)(string[], int, int, bool) | Imports an array of formula into a worksheet. |
| [ImportObjectArray](importobjectarray)(object[], int, int, bool) | Imports an array of data into a worksheet. |
| [ImportObjectArray](importobjectarray)(object[], int, int, bool, int) | Imports an array of data into a worksheet. |
| [ImportTwoDimensionArray](importtwodimensionarray)(object[], int, int) |  |
| [ImportTwoDimensionArray](importtwodimensionarray)(object[], int, int, bool) |  |
| [ImportTwoDimensionArray](importtwodimensionarray)(object[], object[], int, int, bool) |  |
| [ImportTwoDimensionArray](importtwodimensionarray)(object[], object[], int, int, TxtLoadOptions) |  |
| [InsertColumn](insertcolumn)(int) | Inserts a new column into the worksheet. |
| [InsertColumn](insertcolumn)(int, bool) | Inserts a new column into the worksheet. |
| [InsertColumns](insertcolumns)(int, int) | Inserts some columns into the worksheet. |
| [InsertColumns](insertcolumns)(int, int, bool) | Inserts some columns into the worksheet. |
| [InsertCutCells](insertcutcells)(Range, int, int, ShiftType) | Insert cut range. |
| [InsertRange](insertrange)(CellArea, ShiftType) | Inserts a range of cells and shift cells according to the shift option. |
| [InsertRange](insertrange)(CellArea, int, ShiftType) | Inserts a range of cells and shift cells according to the shift option. |
| [InsertRange](insertrange)(CellArea, int, ShiftType, bool) | Inserts a range of cells and shift cells according to the shift option. |
| [InsertRow](insertrow)(int) | Inserts a new row into the worksheet. |
| [InsertRows](insertrows)(int, int) | Inserts multiple rows into the worksheet. |
| [InsertRows](insertrows)(int, int, bool) | Inserts multiple rows into the worksheet. |
| [InsertRows](insertrows)(int, int, InsertOptions) | Inserts multiple rows into the worksheet. |
| [IsBlankColumn](isblankcolumn)(int) | Checks whether given column is blank(does not contain any data). |
| [IsColumnHidden](iscolumnhidden)(int) | Checks whether a column at given index is hidden. |
| [IsDeletingRangeEnabled](isdeletingrangeenabled)(int, int, int, int) | Check whether the range could be deleted. |
| [IsRowHidden](isrowhidden)(int) | Checks whether a row at given index is hidden. |
| [LinkToXmlMap](linktoxmlmap)(string, int, int, string) | Link to a xml map. |
| [Merge](merge)(int, int, int, int) | Merges a specified range of cells into a single cell. |
| [Merge](merge)(int, int, int, int, bool) | Merges a specified range of cells into a single cell. |
| [Merge](merge)(int, int, int, int, bool, bool) | Merges a specified range of cells into a single cell. |
| [MoveRange](moverange)(CellArea, int, int) | Moves the range. |
| [RemoveDuplicates](removeduplicates)() | Removes duplicate rows in the sheet. |
| [RemoveDuplicates](removeduplicates)(int, int, int, int) | Removes duplicate values in the range. |
| [RemoveDuplicates](removeduplicates)(int, int, int, int, bool, int[]) | Removes duplicate data of the range. |
| [RemoveFormulas](removeformulas)() | Removes all formula and replaces with the value of the formula. |
| [RetrieveSubtotalSetting](retrievesubtotalsetting)(CellArea) | Retrieves subtotals setting of the range. |
| [SetColumnWidth](setcolumnwidth)(int, double) | Sets the width of the specified column in normal view. |
| [SetColumnWidthInch](setcolumnwidthinch)(int, double) | Sets column width in unit of inches in normal view. |
| [SetColumnWidthPixel](setcolumnwidthpixel)(int, int) | Sets column width in unit of pixels in normal view. |
| [SetRowHeight](setrowheight)(int, double) | Sets the height of the specified row. |
| [SetRowHeightInch](setrowheightinch)(int, double) | Sets row height in unit of inches. |
| [SetRowHeightPixel](setrowheightpixel)(int, int) | Sets row height in unit of pixels. |
| [SetViewColumnWidthPixel](setviewcolumnwidthpixel)(int, int) | Sets the width of the column in different view. |
| [ShowGroupDetail](showgroupdetail)(bool, int) | Expands the grouped rows/columns. |
| [Subtotal](subtotal)(CellArea, int, ConsolidationFunction, int[]) | Creates subtotals for the range. |
| [Subtotal](subtotal)(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) | Creates subtotals for the range. |
| [TextToColumns](texttocolumns)(int, int, int, TxtLoadOptions) | Splits the text in the column to columns. |
| [UngroupColumns](ungroupcolumns)(int, int) | Ungroups columns. |
| [UngroupRows](ungrouprows)(int, int) | Ungroups rows. |
| [UngroupRows](ungrouprows)(int, int, bool) | Ungroups rows. |
| [UnhideColumn](unhidecolumn)(int, double) | Unhides a column |
| [UnhideColumns](unhidecolumns)(int, int, double) | Unhide multiple columns. |
| [UnhideRow](unhiderow)(int, double) | Unhides a row. |
| [UnhideRows](unhiderows)(int, int, double) | Unhides the hidden rows. |
| [UnMerge](unmerge)(int, int, int, int) | Unmerges a specified range of merged cells. |

### Examples

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Set default row height
cells.StandardHeight = 20;
//Set row height
cells.SetRowHeight(2, 20.5);

//Set default colum width
cells.StandardWidth = 15;
//Set column width
cells.SetColumnWidth(3, 12.57);

//Merge cells
cells.Merge(5, 4, 2, 2);

//Put values to cells
cells[0, 0].PutValue(true);
cells[0, 1].PutValue(1);
cells[0, 2].PutValue("abc");

//Export data
object[,] arr = cells.ExportArray(0, 0, 10, 10);

[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = excel.Worksheets(0).Cells

'Set default row height
cells.StandardHeight = 20
'Set row height
cells.SetRowHeight(2, 20.5)

'Set default colum width
cells.StandardWidth = 15
'Set column width
cells.SetColumnWidth(3, 12.57)

'Merge cells
cells.Merge(5, 4, 2, 2)

'Export data
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
