##Class GridWorksheet
Aspose.Cells.GridWeb.Data.GridWorksheet class. Encapsulates the object that represents a single worksheet
## GridWorksheet class
Encapsulates the object that represents a single worksheet.
```csharp
public class GridWorksheet : Control, ISerializable
```
## Properties
| Name | Description |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb.data/gridworksheet/activecell/) { get; set; } | Gets or sets the active cell in the worksheet. |
| [BackgroundImage](../../aspose.cells.gridweb.data/gridworksheet/backgroundimage/) { get; set; } | Gets and sets worksheet background image. |
| [BindColumns](../../aspose.cells.gridweb.data/gridworksheet/bindcolumns/) { get; } | Bind columns collection. |
| [BindingSource](../../aspose.cells.gridweb.data/gridworksheet/bindingsource/) { get; } | The actually binding datasource object at run-time. It is a DataView object when the DataSource property is a DataSet, DataTable or DataView object. |
| [BindStartColumn](../../aspose.cells.gridweb.data/gridworksheet/bindstartcolumn/) { get; set; } | In data-binding mode, BindStartRow and BindStartColumn indicate the position of the grid to bind bo the datasource. |
| [BindStartRow](../../aspose.cells.gridweb.data/gridworksheet/bindstartrow/) { get; set; } | In data-binding mode, BindStartRow and BindStartColumn indicate the position of the grid to bind bo the datasource. |
| [Cells](../../aspose.cells.gridweb.data/gridworksheet/cells/) { get; } | Gets the [`GridCell`](../gridcell/) collection. |
| [CodeName](../../aspose.cells.gridweb.data/gridworksheet/codename/) { get; } | Represents worksheet code name. |
| [Comments](../../aspose.cells.gridweb.data/gridworksheet/comments/) { get; } | Gets the [`GridComment`](../gridcomment/) collection. |
| [CurrentBindRows](../../aspose.cells.gridweb.data/gridworksheet/currentbindrows/) { get; set; } | Gets the binding rows number in data-binding mode. |
| [DataMember](../../aspose.cells.gridweb.data/gridworksheet/datamember/) { get; set; } | Gets or sets the DataMember from the multi-member DataSource. Generally it represents a DataTable object of a DataSet. |
| [DataSource](../../aspose.cells.gridweb.data/gridworksheet/datasource/) { get; set; } | Gets or sets the DataSource. Generally it's a DataSet object. |
| [DisplayRightToLeft](../../aspose.cells.gridweb.data/gridworksheet/displayrighttoleft/) { get; set; } | Indicates if the specified worksheet is displayed from right to left instead of from left to right. Default is false. |
| [DisplayZeros](../../aspose.cells.gridweb.data/gridworksheet/displayzeros/) { get; set; } | True if zero values are displayed. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/gridworksheet/enablecreatebindcolumnheader/) { get; set; } | In data-binding mode, indicates whether to create bind column header captions in the sheet. |
| [FirstVisibleColumn](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblecolumn/) { get; set; } | Represents first visible column index. |
| [FirstVisibleRow](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblerow/) { get; set; } | Represents first visible row index. |
| [GridActiveCell](../../aspose.cells.gridweb.data/gridworksheet/gridactivecell/) { get; set; } | Gets or sets the active cell in the worksheet. |
| [Hyperlinks](../../aspose.cells.gridweb.data/gridworksheet/hyperlinks/) { get; } | Gets the [`GridHyperlinkCollection`](../gridhyperlinkcollection/) collection. |
| [Index](../../aspose.cells.gridweb.data/gridworksheet/index/) { get; } | Gets the index of sheet in the worksheet collection. |
| [IsGridlinesVisible](../../aspose.cells.gridweb.data/gridworksheet/isgridlinesvisible/) { get; set; } | Gets or sets a value indicating whether the grid lines are visible.Default is true. |
| [IsSummaryRowBelow](../../aspose.cells.gridweb.data/gridworksheet/issummaryrowbelow/) { get; set; } | Indicates if the summary row will be positioned below the detail rows in the outline. |
| [Name](../../aspose.cells.gridweb.data/gridworksheet/name/) { get; set; } | Gets or sets the name of the worksheet. |
| [OutlineShown](../../aspose.cells.gridweb.data/gridworksheet/outlineshown/) { get; set; } | Indicates whether show outline. |
| [Pictures](../../aspose.cells.gridweb.data/gridworksheet/pictures/) { get; } | Gets a [`Pictures`](./pictures/) collection. |
| [PivotTables](../../aspose.cells.gridweb.data/gridworksheet/pivottables/) { get; } | Gets the pivotTables in the worksheet. |
| [Selected](../../aspose.cells.gridweb.data/gridworksheet/selected/) { get; set; } | Indicates whether this worksheet is selected when the workbook is opened. |
| [Shapes](../../aspose.cells.gridweb.data/gridworksheet/shapes/) { get; } | Gets a [`Pictures`](./pictures/) collection. |
| [StandardHeight](../../aspose.cells.gridweb.data/gridworksheet/standardheight/) { get; set; } | Gets or sets the default row height in this worksheet,in unit of points. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridworksheet/standardheightpixels/) { get; set; } | Gets or sets the default row height in this worksheet,in unit of pixels. |
| [TabColor](../../aspose.cells.gridweb.data/gridworksheet/tabcolor/) { get; set; } | Represents worksheet tab color. |
| [Validations](../../aspose.cells.gridweb.data/gridworksheet/validations/) { get; } | Gets the data validation setting collection in the worksheet. |
| override [Visible](../../aspose.cells.gridweb.data/gridworksheet/visible/) { get; set; } | Indicates whether this sheet's name is shown in the sheet tabs of the control. |
| [Workbook](../../aspose.cells.gridweb.data/gridworksheet/workbook/) { get; } | Gets the [`GridWorkbook`](../gridworkbook/) object of the worksheet collection. |
| [Zoom](../../aspose.cells.gridweb.data/gridworksheet/zoom/) { get; set; } | Represents the scaling factor in percentage. It should be between 10 and 400. |
## Methods
| Name | Description |
| --- | --- |
| [AddAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/addautofilter/)(int, int, int) | Sets the range to which the specified AutoFilter applies. |
| [AddCustomFilter](../../aspose.cells.gridweb.data/gridworksheet/addcustomfilter/)(int, string) | Add custom filter for the specified row. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn/#autofitcolumn)(int) | Autofits the column width. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Autofits the column width. |
| [AutoFitColumns](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumns/)() |  |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow)(int) | Autofits the row height. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow_1)(int, int, int) | Autofits the row height. |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow/#autofitrow_2)(int, int, int, int) | Autofits row height in a rectangle range. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows)() | Autofits all rows in this worksheet. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows_1)(bool) | Autofits all rows in this worksheet. |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows/#autofitrows_2)(int, int) | Autofits row height in a range. |
| [CalculateFormula](../../aspose.cells.gridweb.data/gridworksheet/calculateformula/)(string) | Calculates a formula. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/cancelnewbindrow/)() | Cancels and deletes the new added bind row. |
| [ClearComments](../../aspose.cells.gridweb.data/gridworksheet/clearcomments/)() | Clears all comments in designer spreadsheet. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/commitnewbindrow/)() | Commits the new added bind row and add it to the datasource. |
| [Copy](../../aspose.cells.gridweb.data/gridworksheet/copy/)(GridWorksheet) | Copies contents and formats from another worksheet. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/gridworksheet/createautogenratedcolumns/)() | After setting a datasource for the worksheet, call this method to generate the bind columns automatically. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/createnewbindrow/)() | Creates a new bind row and bind to the datasource. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal/#createsubtotal)(int, int, int, SubtotalFunction, int[]) | Creates subtotal in the sheet. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal/#createsubtotal_1)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Creates subtotal in the sheet. |
| override [DataBind](../../aspose.cells.gridweb.data/gridworksheet/databind/)() | Bind the sheet to the DataSource. |
| [DataSourceControlUpdate](../../aspose.cells.gridweb.data/gridworksheet/datasourcecontrolupdate/)(AccessDataSource) | Bind the sheet to the DataSource. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/gridworksheet/deletebindrow/)(int) | Deletes a bind row. |
| [FilterString](../../aspose.cells.gridweb.data/gridworksheet/filterstring/)(int, string) | Sets the filter for the column.notice we shall call AddAutoFilter before calling of filterString The filter criteria string. notice we use comma-&gt;"," as split char,so the cell value you want to filter shall not contains with comma filterString(10,"123,456") means column 10 shall contain 123 or 456, filterString(10,"123") means column10 shall contain 123 the column indexvalue split with comma,eg. 123,456,789 or abc |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes/#freezepanes_1)(string, int, int) | Freezes panes at the specified cell in the worksheet. |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes/#freezepanes)(int, int, int, int) | Freezes panes at the specified cell in the worksheet. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/getcolumncaption/)(int) | Gets the column caption. If the caption is not set, returns empty string. |
| [GetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getcolumnheadertooltip/)(int) | Gets the columnheader's tooltip text. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/getcolumnreadonly/)(int) | Gets if a column is readonly. this is extended method of GridWeb specifically,it will not keep and take affect in actual excel file |
| [GetFreezedPanes](../../aspose.cells.gridweb.data/gridworksheet/getfreezedpanes/)(out int, out int, out int, out int) | Gets the freeze panes. |
| [GetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/getisreadonly/)(int, int) | Gets whether the cell is readonly.this is an extended attribute of GridWeb ,it will not keep in actual excel file |
| [GetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/getrowcaption/)(int) | Gets the row caption. If the caption is not set, returns empty string. |
| [GetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getrowheadertooltip/)(int) | Gets the rowheader's tooltip text. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/getrowreadonly/)(int) | Gets if a row is readonly. this is extended method of GridWeb specifically,it will not keep and take affect in actual excel file |
| [GroupRows](../../aspose.cells.gridweb.data/gridworksheet/grouprows/)(int, int, bool) | Groups rows. |
| [IsProtected](../../aspose.cells.gridweb.data/gridworksheet/isprotected/)() | Indicates if the worksheet is protected. |
| [MoveTo](../../aspose.cells.gridweb.data/gridworksheet/moveto/)(int) | Moves the sheet to another location in the spreadsheet. |
| [RefreshFilter](../../aspose.cells.gridweb.data/gridworksheet/refreshfilter/)() | Refresh auto filters to hide or unhide the rows. |
| [RemoveAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/removeautofilter/)() | Remove the auto filter of the worksheet. |
| [RemoveSubtotal](../../aspose.cells.gridweb.data/gridworksheet/removesubtotal/)() | Removes subtotal created by the CreateSubtotal method in the sheet. |
| [ResetFilter](../../aspose.cells.gridweb.data/gridworksheet/resetfilter/)(int) | The integer offset of the field on which you want to apply ,based on the first filter column (from the left of the list; the leftmost field is field 0). |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/gridworksheet/setallcellseditable/)() | Makes all cells editable.this is extended attribute |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setallcellsreadonly/)() | Makes all cells readonly.this is extended attribute notice this attribute can not keep in actual cell,if you want to keep protect please use setProtect |
| [SetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/setcolumncaption/)(int, string) | Sets the caption for the column.please note this is an extension attribute and can not keep in excel file |
| [SetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setcolumnheadertooltip/)(int, string) | Sets the columnheader's tooltip text. |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/setcolumnreadonly/)(int, bool) | Sets a column to readonly so user can't delete it from client side. this is extended method of GridWeb specifically,it will not keep and take affect in actual excel file |
| [SetEditableRange](../../aspose.cells.gridweb.data/gridworksheet/seteditablerange/)(int, int, int, int) | Makes a range of cells editable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Make all cells read only by calling the SetAllCellsReadonly method. then call this method to Specify the range of cells that to be editable |
| [SetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setisreadonly/)(int, int, bool) | Sets whether the cell is readonly.this is an extended attribute of GridWeb ,it will not keep in actual excel file |
| [SetProtect](../../aspose.cells.gridweb.data/gridworksheet/setprotect/)() | Protects worksheet. |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/gridworksheet/setreadonlyrange/)(int, int, int, int) | Makes a range of cells readonly. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells First make all cells editable by calling the SetAllCellsEditable method. then call this method to Specify the range of cells that to be readonly |
| [SetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/setrowcaption/)(int, string) | Sets the caption for the row. |
| [SetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setrowheadertooltip/)(int, string) | Sets the rowheader's tooltip text. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/setrowreadonly/)(int, bool) | Sets a row to readonly so user can't delete it from client side. this is extended method of GridWeb specifically,it will not keep and take affect in actual excel file |
| [UnFreezePanes](../../aspose.cells.gridweb.data/gridworksheet/unfreezepanes/)() | Unfreezes panes in the worksheet. |
| [UnGroupRows](../../aspose.cells.gridweb.data/gridworksheet/ungrouprows/)(int, int) | Ungroups rows. |
| [UnProtect](../../aspose.cells.gridweb.data/gridworksheet/unprotect/)() | unProtects worksheet. |
## Events
| Name | Description |
| --- | --- |
| event [InitializeNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/initializenewbindrow/) | Occurs when the worksheet has created a new bind row and need to initialize it. |
### See Also
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)
