##Class Worksheet
Aspose.Cells.GridDesktop.Worksheet class. Encapsulates the object that represents a single worksheet
## Worksheet class
Encapsulates the object that represents a single worksheet.
```csharp
public class Worksheet
```
## Properties
| Name | Description |
| --- | --- |
| [ActiveCell](../../aspose.cells.griddesktop/worksheet/activecell/) { get; set; } |  |
| [AllowSelectingLockedCell](../../aspose.cells.griddesktop/worksheet/allowselectinglockedcell/) { get; set; } | Represents if the user is allowed to select locked cells on a protected worksheet. |
| [BackgroundImage](../../aspose.cells.griddesktop/worksheet/backgroundimage/) { get; set; } | Gets and sets worksheet background image. |
| [Cells](../../aspose.cells.griddesktop/worksheet/cells/) { get; } |  |
| [CodeName](../../aspose.cells.griddesktop/worksheet/codename/) { get; } | Represents worksheet code name. |
| [Columns](../../aspose.cells.griddesktop/worksheet/columns/) { get; } |  |
| [ColumnsCount](../../aspose.cells.griddesktop/worksheet/columnscount/) { get; set; } | Gets/Sets Sheet's columns number . |
| [Comments](../../aspose.cells.griddesktop/worksheet/comments/) { get; } |  |
| [Controls](../../aspose.cells.griddesktop/worksheet/controls/) { get; } | Gets the cell control collection. |
| [CustomColumnCaption](../../aspose.cells.griddesktop/worksheet/customcolumncaption/) { get; set; } | Gets or sets the custom column caption for the worksheet. |
| [CustomRowCaption](../../aspose.cells.griddesktop/worksheet/customrowcaption/) { get; set; } | Gets or sets the custom row caption for the worksheet. |
| [DataMember](../../aspose.cells.griddesktop/worksheet/datamember/) { get; } | Gets the data source that the Worksheet object is displaying data for. |
| [DataSource](../../aspose.cells.griddesktop/worksheet/datasource/) { get; } | Gets the specific list in a DataSource for Worksheet object. |
| [DisplayRightToLeft](../../aspose.cells.griddesktop/worksheet/displayrighttoleft/) { get; set; } |  |
| [DisplayZeros](../../aspose.cells.griddesktop/worksheet/displayzeros/) { get; set; } | True if zero values are displayed. |
| [FirstVisibleColumn](../../aspose.cells.griddesktop/worksheet/firstvisiblecolumn/) { get; set; } |  |
| [FirstVisibleRow](../../aspose.cells.griddesktop/worksheet/firstvisiblerow/) { get; set; } | Represents first visible row index. |
| [FrozenCols](../../aspose.cells.griddesktop/worksheet/frozencols/) { get; set; } | Gets or sets Worksheet's frozen column count. Frozen will start at first column. |
| [FrozenRows](../../aspose.cells.griddesktop/worksheet/frozenrows/) { get; set; } | Gets or sets Worksheet's frozen row count. Frozen will start at first row. |
| [GridDesktop](../../aspose.cells.griddesktop/worksheet/griddesktop/) { get; } | Gets Sheet's GridDesktop object. |
| [GridlinesVisible](../../aspose.cells.griddesktop/worksheet/gridlinesvisible/) { get; set; } | Gets or sets a value indicating whether the gridelines are visible.Default is true. |
| [HasAutofilter](../../aspose.cells.griddesktop/worksheet/hasautofilter/) { get; } | Indicates whether this worksheet has auto filter. |
| [Hyperlinks](../../aspose.cells.griddesktop/worksheet/hyperlinks/) { get; } | Gets the HyperlinkCollection collection. |
| [Index](../../aspose.cells.griddesktop/worksheet/index/) { get; } | Gets the index of sheet in the worksheets collection. |
| [IsVeryHidden](../../aspose.cells.griddesktop/worksheet/isveryhidden/) { get; set; } | Indicates wether the sheet is hidden and cannot be shown in the user interface (UI). |
| [IsVisible](../../aspose.cells.griddesktop/worksheet/isvisible/) { get; set; } |  |
| [MergesCount](../../aspose.cells.griddesktop/worksheet/mergescount/) { get; } | Gets the count of the merges |
| [Name](../../aspose.cells.griddesktop/worksheet/name/) { get; set; } | Gets or sets the name of the worksheet. |
| [OutlineShown](../../aspose.cells.griddesktop/worksheet/outlineshown/) { get; set; } | Indicates whether show outline. |
| [Pictures](../../aspose.cells.griddesktop/worksheet/pictures/) { get; } | Gets a [`Pictures`](./pictures/) collection. |
| [PivotTables](../../aspose.cells.griddesktop/worksheet/pivottables/) { get; } | Gets the pivotTables in the worksheet. |
| [Protected](../../aspose.cells.griddesktop/worksheet/protected/) { get; set; } | Indicates if the worksheet is protected. |
| [RowFilter](../../aspose.cells.griddesktop/worksheet/rowfilter/) { get; } | Gets the RowFilterSettings object of the sheet. |
| [Rows](../../aspose.cells.griddesktop/worksheet/rows/) { get; } |  |
| [RowsCount](../../aspose.cells.griddesktop/worksheet/rowscount/) { get; set; } | Gets/Sets Sheet's rows number . |
| [Selected](../../aspose.cells.griddesktop/worksheet/selected/) { get; set; } | Indicates whether this worksheet is selected when the workbook is opened. |
| [Shapes](../../aspose.cells.griddesktop/worksheet/shapes/) { get; } | Gets a [`Shape`](../shape/) collection. |
| [ShowGridlines](../../aspose.cells.griddesktop/worksheet/showgridlines/) { get; set; } |  |
| [TabColor](../../aspose.cells.griddesktop/worksheet/tabcolor/) { get; set; } | Represents worksheet tab color. |
| [Validations](../../aspose.cells.griddesktop/worksheet/validations/) { get; } | Gets the data validation setting collection in the worksheet. |
| [Visible](../../aspose.cells.griddesktop/worksheet/visible/) { get; set; } | Represents if the worksheet is visible. |
| [Workbook](../../aspose.cells.griddesktop/worksheet/workbook/) { get; } |  |
| [Zoom](../../aspose.cells.griddesktop/worksheet/zoom/) { get; set; } | Represents the scaling factor in percent. It should be between 10 and 400. |
## Methods
| Name | Description |
| --- | --- |
| [AddAutoFilter](../../aspose.cells.griddesktop/worksheet/addautofilter/)(int, int, int) | Sets the range to which the specified AutoFilter applies. |
| [AddColumn](../../aspose.cells.griddesktop/worksheet/addcolumn/)() | Adds a new column. |
| [AddCustomFilter](../../aspose.cells.griddesktop/worksheet/addcustomfilter/#addcustomfilter_1)(int, string) | Add custom filter for the specified row. |
| [AddCustomFilter](../../aspose.cells.griddesktop/worksheet/addcustomfilter/#addcustomfilter)(int, int, object[], GridFilterOperatorType[]) | Add custom filter for the specified row range from start row to end row. |
| [AddRow](../../aspose.cells.griddesktop/worksheet/addrow/)() | Adds a new row. |
| [AddSelectedRange](../../aspose.cells.griddesktop/worksheet/addselectedrange/)(CellRange) | Add a new selected range to the worksheet. |
| [AutoFitColumn](../../aspose.cells.griddesktop/worksheet/autofitcolumn/#autofitcolumn)(int) | Autofits the column width. |
| [AutoFitColumn](../../aspose.cells.griddesktop/worksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Autofits the column width. |
| [AutoFitColumns](../../aspose.cells.griddesktop/worksheet/autofitcolumns/#autofitcolumns)() | Autofits all columns in this worksheet. |
| [AutoFitColumns](../../aspose.cells.griddesktop/worksheet/autofitcolumns/#autofitcolumns_1)(int, int) | Autofits the columns width. |
| [AutoFitColumns](../../aspose.cells.griddesktop/worksheet/autofitcolumns/#autofitcolumns_2)(int, int, int, int) | Autofits the columns width. |
| [AutoFitRow](../../aspose.cells.griddesktop/worksheet/autofitrow/#autofitrow)(int) | Autofits the row height. |
| [AutoFitRow](../../aspose.cells.griddesktop/worksheet/autofitrow/#autofitrow_1)(int, int, int) | Autofits the row height. |
| [AutoFitRow](../../aspose.cells.griddesktop/worksheet/autofitrow/#autofitrow_2)(int, int, int, int) | Autofits row height in a rectangle range. |
| [AutoFitRows](../../aspose.cells.griddesktop/worksheet/autofitrows/#autofitrows)() | Autofits all rows in this worksheet. |
| [AutoFitRows](../../aspose.cells.griddesktop/worksheet/autofitrows/#autofitrows_1)(int, int) | Autofits row height in a range. |
| [AutoFitRowsMerged](../../aspose.cells.griddesktop/worksheet/autofitrowsmerged/)() | Autofits all rows in this worksheet.It will also auto fit row height when the cells is merged in a row. |
| [CalculateFormula](../../aspose.cells.griddesktop/worksheet/calculateformula/)(string) | Calculates a formula. |
| [CellInMerged](../../aspose.cells.griddesktop/worksheet/cellinmerged/)(CellLocation) | Gets a value whether the specified cell location is in merges. |
| [CellRangeInMerge](../../aspose.cells.griddesktop/worksheet/cellrangeinmerge/)(CellRange) | Gets a value that indicates whether the specified cell range in merges. |
| [ClearComments](../../aspose.cells.griddesktop/worksheet/clearcomments/)() | Clears all comments in designer spreadsheet. |
| [ClearMerges](../../aspose.cells.griddesktop/worksheet/clearmerges/)() | Clear all merges. |
| [ClearSelection](../../aspose.cells.griddesktop/worksheet/clearselection/)() | Clear the selection in Worksheet. |
| [ColInMerged](../../aspose.cells.griddesktop/worksheet/colinmerged/)(int) | Gets a value that indicates whether the specified column in merges. |
| [ColInSelection](../../aspose.cells.griddesktop/worksheet/colinselection/)(int) | Determines whether the specified column at index is in selected. |
| [Copy](../../aspose.cells.griddesktop/worksheet/copy/)(Worksheet) | Copies contents and formats from another worksheet. |
| [CreateRange](../../aspose.cells.griddesktop/worksheet/createrange/#createrange_1)(string, string) | create CellRange . |
| [CreateRange](../../aspose.cells.griddesktop/worksheet/createrange/#createrange)(int, int, int, int) | create CellRange . |
| [DataBind](../../aspose.cells.griddesktop/worksheet/databind/)(object, string) | Binds data from data source object with Worksheet object. |
| [DataUnbind](../../aspose.cells.griddesktop/worksheet/dataunbind/)() | Unbind data from data source object with Worksheet object. |
| [ExportDataTable](../../aspose.cells.griddesktop/worksheet/exportdatatable/#exportdatatable_1)(int, int, int, int, bool) | Exports data in the Cells collection of a Worksheet to a specifed DataTable object. |
| [ExportDataTable](../../aspose.cells.griddesktop/worksheet/exportdatatable/#exportdatatable)(int, int, int, int, GridExportTableOptions) | Exports data in the [`Cells`](./cells/) collection to a DataTable object. |
| [ExportDataTable](../../aspose.cells.griddesktop/worksheet/exportdatatable/#exportdatatable_2)(int, int, int, int, bool, bool) | Exports data in the Cells collection of a Worksheet to a new DataTable object. |
| [FilterString](../../aspose.cells.griddesktop/worksheet/filterstring/)(int, string) | Sets the filter for the column.notice we shall call AddAutoFilter before calling of filterString The filter criteria string. notice we use comma-&gt;"," as split char,so the cell value you want to filter shall not contains with comma filterString(10,"123,456") means column 10 shall contain 123 or 456, filterString(10,"123") means column10 shall contain 123 value split with comma,eg. 123,456,789 or abc |
| [FreezePanes](../../aspose.cells.griddesktop/worksheet/freezepanes/#freezepanes_1)(string, int, int) | Freezes panes at the specified cell in the worksheet. |
| [FreezePanes](../../aspose.cells.griddesktop/worksheet/freezepanes/#freezepanes)(int, int, int, int) | Freezes panes at the specified cell in the worksheet. |
| [GetAllSelectedRanges](../../aspose.cells.griddesktop/worksheet/getallselectedranges/)() | Gets all selected ranges of this worksheet. |
| [GetCellLocationByClientPoint](../../aspose.cells.griddesktop/worksheet/getcelllocationbyclientpoint/)(Point) | Gets the cell location by client coordinates point. |
| [GetColumnCaption](../../aspose.cells.griddesktop/worksheet/getcolumncaption/)(int) | Gets the column caption. If the caption is not set, returns empty string. |
| [GetFirstVisibleColumn](../../aspose.cells.griddesktop/worksheet/getfirstvisiblecolumn/)() | Get the first visible column index of sheet view. |
| [GetFirstVisibleRow](../../aspose.cells.griddesktop/worksheet/getfirstvisiblerow/)() | Get the first visible row index of sheet view. |
| [GetFocusedCell](../../aspose.cells.griddesktop/worksheet/getfocusedcell/)() | Gets the focused cell. |
| [GetFocusedCellLocation](../../aspose.cells.griddesktop/worksheet/getfocusedcelllocation/)() | Gets a cell location which is focused. |
| [GetFreezedPanes](../../aspose.cells.griddesktop/worksheet/getfreezedpanes/)(out int, out int, out int, out int) | Gets the freeze panes. |
| [GetIsReadonly](../../aspose.cells.griddesktop/worksheet/getisreadonly/)(int, int) | Gets whether the cell is readonly.this is an extended attribute of GridWeb ,it will not keep in actual excel file |
| [GetLastSelection](../../aspose.cells.griddesktop/worksheet/getlastselection/)() | Gets the cell range of last selected. |
| [GetMerge](../../aspose.cells.griddesktop/worksheet/getmerge/)(int) | Gets the cell range of the merge at the specified index. |
| [GetMergeByCell](../../aspose.cells.griddesktop/worksheet/getmergebycell/)(int, int) | get the the merge area that contains the cell at row,column location ,return null if all the merge areas does not include this cell location |
| [GroupColumns](../../aspose.cells.griddesktop/worksheet/groupcolumns/#groupcolumns)(int, int) | Groups columns. |
| [GroupColumns](../../aspose.cells.griddesktop/worksheet/groupcolumns/#groupcolumns_1)(int, int, bool, bool) | Groups columns. |
| [GroupColumns](../../aspose.cells.griddesktop/worksheet/groupcolumns/#groupcolumns_2)(int, int, int, bool) | Groups columns. |
| [GroupRows](../../aspose.cells.griddesktop/worksheet/grouprows/#grouprows)(int, int) | Groups rows. |
| [GroupRows](../../aspose.cells.griddesktop/worksheet/grouprows/#grouprows_1)(int, int, bool) | Groups rows. |
| [GroupRows](../../aspose.cells.griddesktop/worksheet/grouprows/#grouprows_2)(int, int, bool, bool) | Groups rows. |
| [GroupRows](../../aspose.cells.griddesktop/worksheet/grouprows/#grouprows_3)(int, int, int, bool) | Groups rows. |
| [GroupRows](../../aspose.cells.griddesktop/worksheet/grouprows/#grouprows_4)(int, int, int, bool, bool) | Groups rows. |
| [ImportData](../../aspose.cells.griddesktop/worksheet/importdata/)(DataTable, int, int, GridImportTableOptions) | Import data from custom data table. |
| [ImportDataTable](../../aspose.cells.griddesktop/worksheet/importdatatable/)(DataTable, bool, int, int) | Imports a DataTable object into a worksheet. |
| [InSelection](../../aspose.cells.griddesktop/worksheet/inselection/)(CellLocation) | Determines whether the specified cell location is in selected. |
| [InsertColumn](../../aspose.cells.griddesktop/worksheet/insertcolumn/)(int) | Inserts a new column. |
| [InsertRow](../../aspose.cells.griddesktop/worksheet/insertrow/)(int) | Inserts a new row. |
| [IsCellFocused](../../aspose.cells.griddesktop/worksheet/iscellfocused/)() | Determines whether the cell is focused. |
| [IsProtected](../../aspose.cells.griddesktop/worksheet/isprotected/)() | Indicates if the worksheet is protected. |
| [Merge](../../aspose.cells.griddesktop/worksheet/merge/)(CellRange) | Merges a specified range of cells into a single cell. |
| [MergeFocused](../../aspose.cells.griddesktop/worksheet/mergefocused/)(CellLocation) | Gets the index of the focused merge. |
| [MoveTo](../../aspose.cells.griddesktop/worksheet/moveto/)(int) | Moves the sheet to another location in the spreadsheet. |
| [RefreshFilter](../../aspose.cells.griddesktop/worksheet/refreshfilter/)() | Refresh auto filters to hide or unhide the rows. |
| [RemoveAutoFilter](../../aspose.cells.griddesktop/worksheet/removeautofilter/)() | Remove the auto filter of the worksheet. |
| [RemoveColumn](../../aspose.cells.griddesktop/worksheet/removecolumn/)(int) | Removes a column at the specified index. |
| [RemoveRow](../../aspose.cells.griddesktop/worksheet/removerow/)(int) | Removes a row at the specified index. |
| [ResetFilter](../../aspose.cells.griddesktop/worksheet/resetfilter/)(int) | reset filter type to none |
| [ResetFilters](../../aspose.cells.griddesktop/worksheet/resetfilters/)(int, int) | reset filter type to none |
| [RowInMerged](../../aspose.cells.griddesktop/worksheet/rowinmerged/)(int) | Gets a value that indicates whether the specified row in merges. |
| [RowInSelection](../../aspose.cells.griddesktop/worksheet/rowinselection/)(int) | Determines whether the specified row at index is in selected. |
| [SetAllCellsEditable](../../aspose.cells.griddesktop/worksheet/setallcellseditable/)() | Makes all cells editable.this is extended attribute |
| [SetAllCellsReadonly](../../aspose.cells.griddesktop/worksheet/setallcellsreadonly/)() | Makes all cells readonly.this is extended attribute notice this attribute can not keep in actual cell,if you want to keep protect please use setProtect |
| [SetColumnCaption](../../aspose.cells.griddesktop/worksheet/setcolumncaption/)(int, string) | Sets the caption for the column.please note this is an extension attribute and can not keep in excel file |
| [SetFirstVisibleColumn](../../aspose.cells.griddesktop/worksheet/setfirstvisiblecolumn/)(int) | Set the first visible column index of sheet view. |
| [SetFirstVisibleRow](../../aspose.cells.griddesktop/worksheet/setfirstvisiblerow/)(int) | Set the first visible row index of sheet view. |
| [SetFocusedCell](../../aspose.cells.griddesktop/worksheet/setfocusedcell/#setfocusedcell)(CellLocation) | Sets the cell focus at the specified location. |
| [SetFocusedCell](../../aspose.cells.griddesktop/worksheet/setfocusedcell/#setfocusedcell_1)(int, int) | Sets the cell focus at the specified column and row. |
| [SetFont](../../aspose.cells.griddesktop/worksheet/setfont/)(CellRange, Font) | Sets font object to cellRange. |
| [SetFontColor](../../aspose.cells.griddesktop/worksheet/setfontcolor/)(CellRange, Color) | Sets font color to cellRange. |
| [SetIsReadonly](../../aspose.cells.griddesktop/worksheet/setisreadonly/)(int, int, bool) | Sets whether the cell is readonly.this is an extended attribute ,it will not keep in actual excel file |
| [SetProtect](../../aspose.cells.griddesktop/worksheet/setprotect/)() | Protects worksheet. |
| [SetProtected](../../aspose.cells.griddesktop/worksheet/setprotected/)(CellRange, bool) | Sets cellRange whether it is protected.this is an extended method used only in Grid. This method has nothing to do with the cell.Style.CellLocked property It will not take affect after save to excel file. |
| [SetStyle](../../aspose.cells.griddesktop/worksheet/setstyle/#setstyle)(CellRange, Style) | Sets style object to cellRange. |
| [SetStyle](../../aspose.cells.griddesktop/worksheet/setstyle/#setstyle_1)(GridCellArea, Style) | Sets style object to cellRange. |
| [UnFreezePanes](../../aspose.cells.griddesktop/worksheet/unfreezepanes/)() | Unfreezes panes in the worksheet. |
| [UngroupColumns](../../aspose.cells.griddesktop/worksheet/ungroupcolumns/#ungroupcolumns)(int, int) | Ungroups columns. |
| [UngroupColumns](../../aspose.cells.griddesktop/worksheet/ungroupcolumns/#ungroupcolumns_1)(int, int, bool) | Ungroups columns. |
| [UngroupRows](../../aspose.cells.griddesktop/worksheet/ungrouprows/#ungrouprows)(int, int) | Ungroups rows. |
| [UngroupRows](../../aspose.cells.griddesktop/worksheet/ungrouprows/#ungrouprows_1)(int, int, bool) | Ungroups rows. |
| [Unmerge](../../aspose.cells.griddesktop/worksheet/unmerge/#unmerge)(CellLocation) | Remove the specified cell location from merges. |
| [Unmerge](../../aspose.cells.griddesktop/worksheet/unmerge/#unmerge_1)(CellRange) | Unmerges a specified range of cells into a single cell. |
| [Unmerge](../../aspose.cells.griddesktop/worksheet/unmerge/#unmerge_2)(int, int) | Remove the specified cell row column index from merges. |
| [UnProtect](../../aspose.cells.griddesktop/worksheet/unprotect/)() | unProtects worksheet. |
| static [CellIndexToR1C1](../../aspose.cells.griddesktop/worksheet/cellindextor1c1/)(int, int) | Gets cell r1c1 style name according to its row and column indexes. |
## Fields
| Name | Description |
| --- | --- |
| static [DEFAULT_COLUMNSCOUNT](../../aspose.cells.griddesktop/worksheet/default_columnscount/) | Default columns count of worksheet. |
| static [DEFAULT_ROWSCOUNT](../../aspose.cells.griddesktop/worksheet/default_rowscount/) | Default rows count of worksheet. |
### See Also
* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)
