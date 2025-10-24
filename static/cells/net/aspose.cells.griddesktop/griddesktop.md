##Class GridDesktop
Aspose.Cells.GridDesktop.GridDesktop class. Aspose GridDesktop class Represents a root object to create an GridDesktop control. To use this control simply drag it from your toolbox to a form or usercontrol
## GridDesktop class
Aspose GridDesktop class Represents a root object to create an GridDesktop control. To use this control, simply drag it from your toolbox to a form or usercontrol.
```csharp
public class GridDesktop : UserControl
```
## Constructors
| Name | Description |
| --- | --- |
| [GridDesktop](griddesktop/)() | Aspose GridDesktop class |
## Properties
| Name | Description |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells.griddesktop/griddesktop/activesheetindex/) { get; set; } | Gets or sets the selected sheet index. |
| [ActiveSheetNameFont](../../aspose.cells.griddesktop/griddesktop/activesheetnamefont/) { get; set; } | Gets or sets the active sheet displaying font of sheet bar. |
| [AlwasysRecalculateAllFormulas](../../aspose.cells.griddesktop/griddesktop/alwasysrecalculateallformulas/) { get; set; } | Gets or sets a value indicating whether we need to run all formulas,as when we run all formulas, when update one cell value,and it affect others ,and others affect others ,more and more, cause the whole cells need recalculate ,just like the Butterfly Effect,it needs lots of stack opertation , it will get very low performance, like in CELLSNET-41921,this issue contains the very file that can show this scenario we'd better just run all formulas, ,as when run all formulas we may have some optimization. |
| [BorderStyle](../../aspose.cells.griddesktop/griddesktop/borderstyle/) { get; set; } | Indicates the border style for the control. |
| [ColumnHeaderVisible](../../aspose.cells.griddesktop/griddesktop/columnheadervisible/) { get; set; } | Gets or sets a value indicating whether column header is visible. |
| [CommentDisplayingFont](../../aspose.cells.griddesktop/griddesktop/commentdisplayingfont/) { get; set; } | Gets or sets the default displaying font of comment text. |
| [ContextMenuManager](../../aspose.cells.griddesktop/griddesktop/contextmenumanager/) { get; } | Gets the ContextMenuManager instance. |
| [DefaultCellFont](../../aspose.cells.griddesktop/griddesktop/defaultcellfont/) { get; set; } | Gets or sets the default font of the cell |
| [DefaultCellFontColor](../../aspose.cells.griddesktop/griddesktop/defaultcellfontcolor/) { get; set; } | Gets or sets the default font color of the cell. |
| [EnableClipboardCopyPaste](../../aspose.cells.griddesktop/griddesktop/enableclipboardcopypaste/) { get; set; } | Indicates whether to copy/paste based on clipboard,so that it can copy/paste with MS-EXCEL. It only copys/pastes cell value ,It does not copy any other setting of the cell like format,border style and so on The default value is false. |
| [EnableCopyWithExtension](../../aspose.cells.griddesktop/griddesktop/enablecopywithextension/) { get; set; } | Gets or sets a value indicating whether the copy operation will extend the number of rows or columns. |
| [EnableCopyWithLockedOption](../../aspose.cells.griddesktop/griddesktop/enablecopywithlockedoption/) { get; set; } | Gets or sets a value indicating whether the copy operation will copy the style's CellLocked attribute value of a cell. |
| [EnableUndo](../../aspose.cells.griddesktop/griddesktop/enableundo/) { get; set; } | Gets or sets a value indicating whether the Undo function is enabled. The default value is false. |
| [GridMemorySetting](../../aspose.cells.griddesktop/griddesktop/gridmemorysetting/) { get; set; } | Gets or sets memory option,the default value is GridMemorySetting.Normal |
| [IsHorizontalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/ishorizontalscrollbarvisible/) { get; set; } | Sets visible statue for Horizontal ScrollBar. |
| [IsVerticalScrollBarVisible](../../aspose.cells.griddesktop/griddesktop/isverticalscrollbarvisible/) { get; set; } | Sets visible statue for Vertical ScrollBar. |
| [Names](../../aspose.cells.griddesktop/griddesktop/names/) { get; } | Gets the collection of all the Name objects in the spreadsheet. |
| [PageRows](../../aspose.cells.griddesktop/griddesktop/pagerows/) { get; set; } | Sets or Gets row size for Pagination.the maximum of PageRows supported is 100000,the maximum of page number supported is 5000. |
| [PasteType](../../aspose.cells.griddesktop/griddesktop/pastetype/) { get; set; } | Indicates which paste type when do paste action，only available when EnableClipboardCopyPaste is false .the default value is GridPasteType.Default; |
| [R1C1](../../aspose.cells.griddesktop/griddesktop/r1c1/) { get; set; } | Gets or sets a value indicating whether the control using R1C1 reference style. |
| [RecalculateFormulas](../../aspose.cells.griddesktop/griddesktop/recalculateformulas/) { get; set; } | Gets or sets a value indicating whether to recalculate all the cells' formula when a cell's value changed. The default value is true. |
| [RowHeaderVisible](../../aspose.cells.griddesktop/griddesktop/rowheadervisible/) { get; set; } | Gets or sets a value indicating whether row header is visible. |
| [SheetNameFont](../../aspose.cells.griddesktop/griddesktop/sheetnamefont/) { get; set; } | Gets or sets the default displaying font of sheet bar. |
| [SheetsBarVisible](../../aspose.cells.griddesktop/griddesktop/sheetsbarvisible/) { get; set; } | Gets or sets a value indicating whether sheet bar is visible. |
| [SheetTabWidth](../../aspose.cells.griddesktop/griddesktop/sheettabwidth/) { get; set; } | Sets /Gets width of Sheet Tab. |
| [ShowContextMenu](../../aspose.cells.griddesktop/griddesktop/showcontextmenu/) { get; set; } | Gets or sets a value indicating whether the control can show context menu. |
| [ShowFormulaWarning](../../aspose.cells.griddesktop/griddesktop/showformulawarning/) { get; set; } | Sets/Gets whether to show the error or waring message for set cell formula value,the default value is true. |
| [ShowNumberStoredAsTextSymbol](../../aspose.cells.griddesktop/griddesktop/shownumberstoredastextsymbol/) { get; set; } | Sets /Gets whether show the triangle symbol for the cell which contains number string but stored as text format |
| [ShowStatus](../../aspose.cells.griddesktop/griddesktop/showstatus/) { get; set; } | Gets or sets a value indicating whether to show the calculate status The default value is true. |
| [UndoManager](../../aspose.cells.griddesktop/griddesktop/undomanager/) { get; } | Gets the UndoManager instance. |
| [Worksheets](../../aspose.cells.griddesktop/griddesktop/worksheets/) { get; } | Gets the Worksheets. |
## Methods
| Name | Description |
| --- | --- |
| [Clear](../../aspose.cells.griddesktop/griddesktop/clear/)() | Clears GridDesktop control. |
| [Copy](../../aspose.cells.griddesktop/griddesktop/copy/)() | Copies focused cell content to clipboard. |
| [Cut](../../aspose.cells.griddesktop/griddesktop/cut/)() | Cuts focused cell content to clipboard. |
| [DoSplit](../../aspose.cells.griddesktop/griddesktop/dosplit/)() | Sets Split view. |
| [EndFormatPainter](../../aspose.cells.griddesktop/griddesktop/endformatpainter/)() | Notifies GridDesktop to end FormatPainter. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile)(Stream) | Exports to a excel file stream, including disk IO stream or memory stream. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_2)(string) | Exports to an excel file. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_1)(Stream, FileFormatType) | Exports to a excel file stream, including disk IO stream or memory stream. |
| [ExportExcelFile](../../aspose.cells.griddesktop/griddesktop/exportexcelfile/#exportexcelfile_3)(string, FileFormatType) | Exports to a excel file. |
| [ExportPdfFile](../../aspose.cells.griddesktop/griddesktop/exportpdffile/#exportpdffile)(Stream, GridPdfSaveOptions) | Exports to a pdf file stream, including disk IO stream or memory stream. |
| [ExportPdfFile](../../aspose.cells.griddesktop/griddesktop/exportpdffile/#exportpdffile_1)(string, GridPdfSaveOptions) | Exports to a pdf file stream, including disk IO stream or memory stream. |
| [GetActiveWorksheet](../../aspose.cells.griddesktop/griddesktop/getactiveworksheet/)() | Gets current active worksheet. |
| [getHScrollBar](../../aspose.cells.griddesktop/griddesktop/gethscrollbar/)() | return horizontal scroll bar |
| [getVScrollBar](../../aspose.cells.griddesktop/griddesktop/getvscrollbar/)() | return vertical scroll bar |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile)(Stream) | Imports from an excel file stream, including disk file stream or memory stream. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_3)(string) | Imports from an excel file. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_1)(Stream, bool) | Imports from an excel file stream, including disk file stream or memory stream. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_4)(string, bool) | Imports from an excel file. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_5)(string, int) | Imports a worksheet from an excel file. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_2)(Stream, string, string, bool, bool) | Imports from an excel file. |
| [ImportExcelFile](../../aspose.cells.griddesktop/griddesktop/importexcelfile/#importexcelfile_6)(string, string, string, bool, bool) | Imports from an excel file. |
| [Invalidate](../../aspose.cells.griddesktop/griddesktop/invalidate/#invalidate)() | Override invalidate. |
| [OpenFindReplaceDialog](../../aspose.cells.griddesktop/griddesktop/openfindreplacedialog/)(bool) | Opens the FindReplace dialog to find or replace cells. |
| [Paste](../../aspose.cells.griddesktop/griddesktop/paste/)() | Pastes clipboard content to focused cell. |
| [RefreshControl](../../aspose.cells.griddesktop/griddesktop/refreshcontrol/)() | Refresh the GridDesktop control. |
| [RunAllFormulas](../../aspose.cells.griddesktop/griddesktop/runallformulas/)() | Runs all the cells's formula. |
| [SetAllScrollBarsVisible](../../aspose.cells.griddesktop/griddesktop/setallscrollbarsvisible/)() | Sets all scrollbars visible. |
| [SetCustomResourceManager](../../aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/)(ResourceManager) | Set custom resource manager to implement user defined localization |
| [ShowStyleDialog](../../aspose.cells.griddesktop/griddesktop/showstyledialog/)() | Opens a style dialog,to set cells style,font,colors etc. |
| [StartFormatPainter](../../aspose.cells.griddesktop/griddesktop/startformatpainter/)(bool) | Notifies GridDesktop to start FormatPainter. |
| [UnDoSplit](../../aspose.cells.griddesktop/griddesktop/undosplit/)() | Unset Split view. |
| static [GetVersion](../../aspose.cells.griddesktop/griddesktop/getversion/)() | Get the release version. |
## Fields
| Name | Description |
| --- | --- |
| [LoadDataFilter](../../aspose.cells.griddesktop/griddesktop/loaddatafilter/) | the options to filter data when loading workbook from template. |
| [ShowImportMessage](../../aspose.cells.griddesktop/griddesktop/showimportmessage/) | wether to show message box when fail to import the file ,the default value is true |
## Events
| Name | Description |
| --- | --- |
| event [AfterDeleteColumns](../../aspose.cells.griddesktop/griddesktop/afterdeletecolumns/) | Occurs after column is deleted. |
| event [AfterDeleteRows](../../aspose.cells.griddesktop/griddesktop/afterdeleterows/) | Occurs after row is deleted. |
| event [AfterInsertColumns](../../aspose.cells.griddesktop/griddesktop/afterinsertcolumns/) | Occurs after new column is inserted. |
| event [AfterInsertRows](../../aspose.cells.griddesktop/griddesktop/afterinsertrows/) | Occurs after new row is inserted. |
| event [BeforeCalculate](../../aspose.cells.griddesktop/griddesktop/beforecalculate/) | Occurs before calculate formula in workbook. |
| event [BeforeLoadFile](../../aspose.cells.griddesktop/griddesktop/beforeloadfile/) | Occurs before workbook loaded from file. |
| event [CellButtonClick](../../aspose.cells.griddesktop/griddesktop/cellbuttonclick/) | Occurs when the cell button clicked. |
| event [CellCheckedChanged](../../aspose.cells.griddesktop/griddesktop/cellcheckedchanged/) | Occurs when the cell checkbox Checked property is changed. |
| event [CellClick](../../aspose.cells.griddesktop/griddesktop/cellclick/) | Occurs when the gridcell is clicked. |
| event [CellComboBoxCopy](../../aspose.cells.griddesktop/griddesktop/cellcomboboxcopy/) | Occurs when a grid cell ComboBox is being copied. |
| event [CellDataChanged](../../aspose.cells.griddesktop/griddesktop/celldatachanged/) | Occurs when the grid cell data property is changed. |
| event [CellDoubleClick](../../aspose.cells.griddesktop/griddesktop/celldoubleclick/) | Occurs when the gridcell is double clicked. |
| event [CellFormatChanged](../../aspose.cells.griddesktop/griddesktop/cellformatchanged/) | Occurs when the cell format is changed via Format Cells dialog box. |
| event [CellKeyPressed](../../aspose.cells.griddesktop/griddesktop/cellkeypressed/) | Occurs when a key is pressed while a cell has focus. |
| event [CellSelectedIndexChanged](../../aspose.cells.griddesktop/griddesktop/cellselectedindexchanged/) | Occurs when the cell combobox SelectedIndex property has changed. |
| event [CellTextBoxChanging](../../aspose.cells.griddesktop/griddesktop/celltextboxchanging/) | Occurs when typing characters in a grid cell. |
| event [CellValidationFailed](../../aspose.cells.griddesktop/griddesktop/cellvalidationfailed/) | Occurs when a grid cell validates failed. |
| event [ColumnHeaderClick](../../aspose.cells.griddesktop/griddesktop/columnheaderclick/) | Occurs when the column header clicked. |
| event [ColumnHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/columnheaderdoubleclick/) | Occurs when the column header double clicked. |
| event [CommentDataChanged](../../aspose.cells.griddesktop/griddesktop/commentdatachanged/) | Occurs when the comment data has changed. |
| event [FailLoadFile](../../aspose.cells.griddesktop/griddesktop/failloadfile/) |  |
| event [FinishCalculate](../../aspose.cells.griddesktop/griddesktop/finishcalculate/) | Occurs after calculate formula in workbook. |
| event [FinishLoadFile](../../aspose.cells.griddesktop/griddesktop/finishloadfile/) | Occurs when the workbook is loaded. |
| event [FocusedCellChanged](../../aspose.cells.griddesktop/griddesktop/focusedcellchanged/) | Occurs when the focused cell is changed. |
| event [PictureClick](../../aspose.cells.griddesktop/griddesktop/pictureclick/) | Occurs when the shape is clicked. |
| event [RowColumnHiddenChanged](../../aspose.cells.griddesktop/griddesktop/rowcolumnhiddenchanged/) | Occurs when the row/column hide status changed. |
| event [RowFilteredEvent](../../aspose.cells.griddesktop/griddesktop/rowfilteredevent/) | Occurs after row filter item selected. |
| event [RowHeaderClick](../../aspose.cells.griddesktop/griddesktop/rowheaderclick/) | Occurs when the row header clicked. |
| event [RowHeaderDoubleClick](../../aspose.cells.griddesktop/griddesktop/rowheaderdoubleclick/) | Occurs when the row header double clicked. |
| event [SelectedCellRangeChanged](../../aspose.cells.griddesktop/griddesktop/selectedcellrangechanged/) | Occurs when the selected cellrange is changed. |
| event [SelectedSheetIndexChanged](../../aspose.cells.griddesktop/griddesktop/selectedsheetindexchanged/) | Occurs when the SelectedSheetIndex property is changed. |
| event [ShapeClick](../../aspose.cells.griddesktop/griddesktop/shapeclick/) | Occurs when the shape is clicked. |
### Remarks
Please refer to .NET SDK document about further information about System.Windows.Forms.UserControl.
### Examples
```csharp
[C#]
gridDesktop1.Worksheets[0].Cells[0, 0].Value = "2";
gridDesktop1.Worksheets[0].Cells[1, 0].Value = "3";
gridDesktop1.Worksheets[0].Cells[2, 1].Value = "=a1*a2";
gridDesktop1.RunAllFormulas();
gridDesktop1.Invalidate();
[Visual Basic]
gridDesktop1.Worksheets(0).Cells(0, 0).Value = "2"
gridDesktop1.Worksheets(0).Cells(1, 0).Value = "3"
gridDesktop1.Worksheets(0).Cells(2, 1).Value = "=a1*a2"
gridDesktop1.RunAllFormulas()
gridDesktop1.Invalidate()
```
### See Also
* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)
