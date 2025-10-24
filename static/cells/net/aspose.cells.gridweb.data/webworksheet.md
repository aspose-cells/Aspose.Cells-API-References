##Class WebWorksheet
Aspose.Cells.GridWeb.Data.WebWorksheet class. Represents a web worksheet
## WebWorksheet class
Represents a web worksheet.
```csharp
[Obsolete("This class is obsolete; use  GridWorksheet instead")]
public class WebWorksheet : Control, ISerializable
```
## Constructors
| Name | Description |
| --- | --- |
| [WebWorksheet](webworksheet/#constructor)() | the constructor of the WebWorksheet. |
| [WebWorksheet](webworksheet/#constructor_1)(MainWeb, GridWorksheet) | the constructor of the WebWorksheet. |
## Properties
| Name | Description |
| --- | --- |
| [BindColumns](../../aspose.cells.gridweb.data/webworksheet/bindcolumns/) { get; } | Bind columns collection. |
| [BindingSource](../../aspose.cells.gridweb.data/webworksheet/bindingsource/) { get; } | The actually binding datasource object at run-time. It is a DataView object when the DataSource property is a DataSet, DataTable or DataView object. |
| [BindStartColumn](../../aspose.cells.gridweb.data/webworksheet/bindstartcolumn/) { get; set; } | In data-binding mode, BindStartRow and BindStartColumn indicate the position of the grid to bind bo the datasource. |
| [BindStartRow](../../aspose.cells.gridweb.data/webworksheet/bindstartrow/) { get; set; } | In data-binding mode, BindStartRow and BindStartColumn indicate the position of the grid to bind bo the datasource. |
| [CellImages](../../aspose.cells.gridweb.data/webworksheet/cellimages/) { get; } |  |
| [Cells](../../aspose.cells.gridweb.data/webworksheet/cells/) { get; } | Gets the [`WebCells`](../webcells/). |
| [Comments](../../aspose.cells.gridweb.data/webworksheet/comments/) { get; } |  |
| [CurrentBindRows](../../aspose.cells.gridweb.data/webworksheet/currentbindrows/) { get; set; } | Gets the binding rows number in data-binding mode. |
| [DataMember](../../aspose.cells.gridweb.data/webworksheet/datamember/) { get; set; } | Gets or sets the DataMember from the multi-member DataSource. Generally it represents a DataTable object of a DataSet. |
| [DataSource](../../aspose.cells.gridweb.data/webworksheet/datasource/) { get; set; } | Gets or sets the DataSource. Generally it's a DataSet object. |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/webworksheet/enablecreatebindcolumnheader/) { get; set; } | In data-binding mode, indicates whether to create bind column header captions in the sheet. |
| [Hyperlinks](../../aspose.cells.gridweb.data/webworksheet/hyperlinks/) { get; } | Gets the HyperlinkCollection collection. |
| [Index](../../aspose.cells.gridweb.data/webworksheet/index/) { get; } | Gets the index of itself within the worksheets. |
| [IsProtected](../../aspose.cells.gridweb.data/webworksheet/isprotected/) { get; set; } | Gets or sets whether the worksheet is protected. When a worksheet is protected, all the cells can not be edit except the cell whose IsLocked property is false. |
| [Name](../../aspose.cells.gridweb.data/webworksheet/name/) { get; set; } | Gets or sets the name of the sheet. |
| [RowFilter](../../aspose.cells.gridweb.data/webworksheet/rowfilter/) { get; } |  |
| [Validations](../../aspose.cells.gridweb.data/webworksheet/validations/) { get; } | Gets the data validation setting collection in the worksheet. |
| override [Visible](../../aspose.cells.gridweb.data/webworksheet/visible/) { get; set; } | Indicates whether this sheet's name is shown in the sheet tabs of the control. |
## Methods
| Name | Description |
| --- | --- |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn)(int) | Autofits the column width. |
| [AutoFitColumn](../../aspose.cells.gridweb.data/webworksheet/autofitcolumn/#autofitcolumn_1)(int, int, int) | Autofits the column width. This method autofits a column based on content in a range of cells within the column from startRow to endRow. AutoFitColumn is an imprecise function. |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/webworksheet/cancelnewbindrow/)() | Cancels and deletes the new added bind row. |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/webworksheet/commitnewbindrow/)() | Commits the new added bind row and add it to the datasource. |
| [Copy](../../aspose.cells.gridweb.data/webworksheet/copy/)(WebWorksheet) | Copies from another worksheet object. |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/webworksheet/createautogenratedcolumns/)() | After setting a datasource for the worksheet, call this method to generate the bind columns automatically. |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/webworksheet/createnewbindrow/)() | Creates a new bind row and bind to the datasource. |
| [CreateSubtotal](../../aspose.cells.gridweb.data/webworksheet/createsubtotal/)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | Creates subtotal in the sheet. |
| override [DataBind](../../aspose.cells.gridweb.data/webworksheet/databind/)() | Bind the sheet to the DataSource. |
| [DeleteBindRow](../../aspose.cells.gridweb.data/webworksheet/deletebindrow/)(int) | Deletes a bind row. |
| [FreezePanes](../../aspose.cells.gridweb.data/webworksheet/freezepanes/)(int, int, int, int) | Freezes panes at the specified cell in the worksheet. |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows)(int, int) | Groups rows. |
| [GroupRows](../../aspose.cells.gridweb.data/webworksheet/grouprows/#grouprows_1)(int, int, bool) | Groups rows. |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/webworksheet/setallcellseditable/)() | Makes all cells editable.this is extended attribute |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/webworksheet/setallcellsreadonly/)() | Makes all cells readonly.this is extended attribute notice this attribute can not keep in actual cell,if you want to keep protect please use setProtect |
| [SetEditableRange](../../aspose.cells.gridweb.data/webworksheet/seteditablerange/)(int, int, int, int) | Makes a range of cells editable. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Make all cells read only by calling the SetAllCellsReadonly method. then call this method to Specify the range of cells that to be editable |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/webworksheet/setreadonlyrange/)(int, int, int, int) | Makes a range of cells readonly. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells First make all cells editable by calling the SetAllCellsEditable method. then call this method to Specify the range of cells that to be readonly |
| [UnfreezePanes](../../aspose.cells.gridweb.data/webworksheet/unfreezepanes/)() | Unfreezes panes in the worksheet. |
| [UngroupRows](../../aspose.cells.gridweb.data/webworksheet/ungrouprows/)(int, int) | Ungroups rows. |
| [UpdateBindCellValue](../../aspose.cells.gridweb.data/webworksheet/updatebindcellvalue/)(GridCell) | Updates the binding datasource record's property value according to the cell's value. |
### Remarks
NOTE: This class is now obsolete. please use GridWorksheet Instead. This class will be removed after 6 months since Aug. 2014. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
[C#]
...
using System.Web.UI.WebControls;
...
...
WebWorksheets Worksheets = GridWeb1.WebWorksheets;
WebCells cells = Worksheets[0].Cells;
//Sets default row height
cells.StandardHeight = new Unit(16, UnitType.Point);
//Sets row height
cells.SetRowHeight(2, new Unit(20, UnitType.Point));
//Sets default colum width
cells.StandardWidth = new Unit(50, UnitType.Point);
//Sets column width
cells.SetColumnWidth(3, new Unit(80, UnitType.Point));
//Merge cells
cells.Merge(5, 4, 2, 2);
//Import data
DataSet1 ds1 = new DataSet1();
for (int i =0; i<16; i++)
{
DataSet1.Table1Row row = ds1.Table1.NewTable1Row();
row["c1"] = "hello1";
row["c2"] = i;
row["c3"] = "data";
ds1.Table1.AddTable1Row(row);
}
GridWeb1.WebWorksheets.ImportDataView(ds1.Table1.DefaultView, null, null);
//Import from excel file
Worksheets.ImportExcelFile("c:\\file1.xls");
[Visual Basic]
Imports System.Web.UI.WebControls
...
...
Dim Worksheets As WebWorksheets =  GridWeb1.WebWorksheets
Dim cells As WebCells =  Worksheets(0).Cells
'Sets default row height
cells.StandardHeight = New Unit(16, UnitType.Point)
'Sets row height
cells.SetRowHeight(2,New Unit(20,UnitType.Point))
'Sets default colum width
cells.StandardWidth = New Unit(50, UnitType.Point)
'Sets column width
cells.SetColumnWidth(3,New Unit(80,UnitType.Point))
'Merge cells
cells.Merge(5, 4, 2, 2)
'Import data
Dim ds1 As DataSet1 =  New DataSet1()
Dim i As Integer
For  i = 0 To 15
Dim row As DataSet1.Table1Row =  ds1.Table1.NewTable1Row()
row("c1") = "hello1"
row("c2") = i
row("c3") = "data"
ds1.Table1.AddTable1Row(row)
Next
GridWeb1.WebWorksheets.ImportDataView(ds1.Table1.DefaultView, Nothing, Nothing)
'Import from excel file
Worksheets.ImportExcelFile("c:\\file1.xls")
```
### See Also
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)
