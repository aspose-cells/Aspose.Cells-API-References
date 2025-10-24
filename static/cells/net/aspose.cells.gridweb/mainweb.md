##Class MainWeb
Aspose.Cells.GridWeb.MainWeb class. Parent class of GridWeb control.Internal use only
## MainWeb class
Parent class of GridWeb control.Internal use only.
```csharp
public class MainWeb : ExtWebControl, INamingContainer, IPostBackDataHandler,
IPostBackEventHandler, ISerializable
```
## Constructors
| Name | Description |
| --- | --- |
| [MainWeb](mainweb/)() | the default constructor of MainWeb control. |
## Properties
| Name | Description |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb/mainweb/activecell/) { get; set; } | Gets or sets the active cell of the current sheet. Changed to be writable since version 1.9.0.1. |
| [ActiveCellBgColor](../../aspose.cells.gridweb/mainweb/activecellbgcolor/) { get; set; } | Specifies the background color of the active cell. |
| [ActiveCellColor](../../aspose.cells.gridweb/mainweb/activecellcolor/) { get; set; } | Specifies the color of the active cell. |
| [ActiveHeaderBgColor](../../aspose.cells.gridweb/mainweb/activeheaderbgcolor/) { get; set; } | Specifies the background color of the active row/column header. |
| [ActiveHeaderColor](../../aspose.cells.gridweb/mainweb/activeheadercolor/) { get; set; } | Specifies the color of the active row/column header. |
| [ActiveSheet](../../aspose.cells.gridweb/mainweb/activesheet/) { get; } | Gets the active sheet |
| [ActiveSheetIndex](../../aspose.cells.gridweb/mainweb/activesheetindex/) { get; set; } | Gets or sets the active sheet index. Equal to the WebWorksheets.ActiveSheetIndex. |
| [ActiveTabStyle](../../aspose.cells.gridweb/mainweb/activetabstyle/) { get; set; } | Specifies the style of the active tab. |
| [ACWClientPath](../../aspose.cells.gridweb/mainweb/acwclientpath/) { get; set; } | Gets or sets the web path of the script/image files of the control. For example: "http://localhost/acw_client". You may also set this value in the web.config file. Add this section to the `<configuration>` section:`<appSettings>``<add key="aspose.cells.gridweb.acw_client_path" value="/acw_client/" />``</appSettings>` |
| [ACWLanguageFileUrl](../../aspose.cells.gridweb/mainweb/acwlanguagefileurl/) { get; set; } | Gets or sets the web url of the language file of the control. For example: "/acw_client/lang_en.js". By default, a built-in english file is used. |
| [AutoRefreshChart](../../aspose.cells.gridweb/mainweb/autorefreshchart/) { get; set; } | Gets or sets whether the Chart image is updated while updating the cell value.the default is true |
| [BottomTableStyle](../../aspose.cells.gridweb/mainweb/bottomtablestyle/) { get; set; } | Gets or sets the style of the bottom bar of the control. |
| [CurrentPageIndex](../../aspose.cells.gridweb/mainweb/currentpageindex/) { get; set; } | Gets or sets the current page index in paging mode. |
| [CustomCalculationEngine](../../aspose.cells.gridweb/mainweb/customcalculationengine/) { get; set; } | Represents user's custom calculation engine to extend the default calculation engine of Aspose.Cells. |
| [CustomCommandButtons](../../aspose.cells.gridweb/mainweb/customcommandbuttons/) { get; } | Gets the custom command button collection |
| [CustomStyleFileName](../../aspose.cells.gridweb/mainweb/customstylefilename/) { get; set; } | Gets or sets the custom style file name. |
| [DefaultFontName](../../aspose.cells.gridweb/mainweb/defaultfontname/) { get; set; } | Gets or sets the control's default font name. |
| [DefaultFontSize](../../aspose.cells.gridweb/mainweb/defaultfontsize/) { get; set; } | Gets or sets the control's default font size. |
| [DefaultGridLineColor](../../aspose.cells.gridweb/mainweb/defaultgridlinecolor/) { get; set; } | Gets or sets the default grid line's color. |
| [DisplayCellTip](../../aspose.cells.gridweb/mainweb/displaycelltip/) { get; set; } | Gets or sets whether to show tips. the default value is true. |
| [EditMode](../../aspose.cells.gridweb/mainweb/editmode/) { get; set; } | Gets or sets the control's edit mode. |
| [EnableAJAX](../../aspose.cells.gridweb/mainweb/enableajax/) { get; set; } | Gets or sets whether to use AJAX call . the default value is true. |
| [EnableAsync](../../aspose.cells.gridweb/mainweb/enableasync/) { get; set; } | Gets or sets whether load cells data in asynchronous way,suggest to apply for one sheet with more than 10000 cells. |
| [EnableClientColumnOperations](../../aspose.cells.gridweb/mainweb/enableclientcolumnoperations/) { get; set; } | Gets or sets whether to enable the client side column operations. |
| [EnableClientFreeze](../../aspose.cells.gridweb/mainweb/enableclientfreeze/) { get; set; } | Gets or sets whether to enable the client side freezing operations. |
| [EnableClientMergeOperations](../../aspose.cells.gridweb/mainweb/enableclientmergeoperations/) { get; set; } | Gets or sets whether to enable the client side merge operations. |
| [EnableClientResizeColumnRow](../../aspose.cells.gridweb/mainweb/enableclientresizecolumnrow/) { get; set; } | Gets or sets whether to enable the client side resize column and row. |
| [EnableClientRowOperations](../../aspose.cells.gridweb/mainweb/enableclientrowoperations/) { get; set; } | Gets or sets whether to enable the client side row operations. |
| [EnableDoubleClickEvent](../../aspose.cells.gridweb/mainweb/enabledoubleclickevent/) { get; set; } | Gets or sets whether to enable customer side double-click event. |
| [EnableMetalLightEffect](../../aspose.cells.gridweb/mainweb/enablemetallighteffect/) { get; set; } | Gets or sets whether to apply metal light effect. |
| [EnablePaging](../../aspose.cells.gridweb/mainweb/enablepaging/) { get; set; } | Gets or sets whether to enable the control's paging mode. |
| [EnableStyleDialogbox](../../aspose.cells.gridweb/mainweb/enablestyledialogbox/) { get; set; } | Gets or sets whether to enable the client side style dialogbox. |
| [FilteredPaging](../../aspose.cells.gridweb/mainweb/filteredpaging/) { get; set; } | Gets or sets whether to enable the paging after data filtered,will take affect when EnablePaging is true. |
| [ForceValidation](../../aspose.cells.gridweb/mainweb/forcevalidation/) { get; set; } | Gets or sets whether to force customer side validation. |
| [FrameTableStyle](../../aspose.cells.gridweb/mainweb/frametablestyle/) { get; set; } | Gets or sets the frame style of the control. |
| [GoonDefaultSaveOperation](../../aspose.cells.gridweb/mainweb/goondefaultsaveoperation/) { get; set; } | Gets or sets whether GridWeb will do the default save operation ,the default value is true. |
| [HeaderBarHeight](../../aspose.cells.gridweb/mainweb/headerbarheight/) { get; set; } | Gets or sets the height( System.Web.UI.WebControl.Unit ) of the top header bar of the control. |
| [HeaderBarStyle](../../aspose.cells.gridweb/mainweb/headerbarstyle/) { get; set; } | Gets or sets the header bar's style. |
| [HeaderBarTableStyle](../../aspose.cells.gridweb/mainweb/headerbartablestyle/) { get; set; } | Gets or sets the header bar style of the control. |
| [HeaderBarWidth](../../aspose.cells.gridweb/mainweb/headerbarwidth/) { get; set; } | Gets or sets the width( System.Web.UI.WebControl.Unit ) or the left header bar of the control. |
| override [Height](../../aspose.cells.gridweb/mainweb/height/) { get; set; } | Gets or sets the height( System.Web.UI.WebControl.Unit ) of the control. |
| [IgnoreStyleWithNoData](../../aspose.cells.gridweb/mainweb/ignorestylewithnodata/) { get; set; } | Gets or sets whether GridWeb ignores showing rows or columns that do not contain cell values but are still styled. If set to true, the performance will be better. The default value is false, which means that if the last consecutive row/column has no cell values but is styled, we will still display them. This option is only valid when EnableAsync is false. This option has no effect when EnableAsync is true, which means GridWeb will show all rows/columns with style. |
| [IsCalculateFormula](../../aspose.cells.gridweb/mainweb/iscalculateformula/) { get; set; } | Gets or sets whether to calculate formula after cell value changes or after import File. The default value is true. |
| [IsPostBack](../../aspose.cells.gridweb/mainweb/ispostback/) { get; } | Gets a value indicating whether gridweb is being loaded in response to a client postback, or if it is being loaded and accessed for the first time. |
| [LoadOptions](../../aspose.cells.gridweb/mainweb/loadoptions/) { get; set; } | Represents the loadoptions for GridWeb. |
| [MaxColumn](../../aspose.cells.gridweb/mainweb/maxcolumn/) { get; set; } | Gets or sets the maximum display column index(zero based) of the web sheet. The control uses the greater value of MaxColumn and sheet data's max column. |
| [MaxRow](../../aspose.cells.gridweb/mainweb/maxrow/) { get; set; } | Gets or sets the maximum display row index(zero based) of the web sheet. The control uses the greater value of MaxRow and sheet data's max row. |
| [Message](../../aspose.cells.gridweb/mainweb/message/) { get; set; } | Gets or sets the message for the grid. |
| [MinColumn](../../aspose.cells.gridweb/mainweb/mincolumn/) { get; set; } | Gets or sets the minimum display column index(zero based) of the web sheet. The control uses the smaller value of MinColumn and sheet data's min column. |
| [MinRow](../../aspose.cells.gridweb/mainweb/minrow/) { get; set; } | Gets or sets the minimum display row index(zero based) of the web sheet. The control uses the smaller value of MinRow and sheet data's min row. |
| [ModifiedCells](../../aspose.cells.gridweb/mainweb/modifiedcells/) { get; } | Gets the collection of the cells that modified by the client. |
| [NeedRenderGroupRows](../../aspose.cells.gridweb/mainweb/needrendergrouprows/) { get; set; } | Gets or sets whether to show grouprows . |
| [NoHScroll](../../aspose.cells.gridweb/mainweb/nohscroll/) { get; set; } | Gets or sets a value indicating whether the horizontal scroll bar is hidden. |
| [NoScroll](../../aspose.cells.gridweb/mainweb/noscroll/) { get; set; } | Gets or sets whether to show scroll bar . |
| [NoVScroll](../../aspose.cells.gridweb/mainweb/novscroll/) { get; set; } | Gets or sets a value indicating whether the vertical scroll bar is hidden. |
| [OnAjaxCallFinishedClientFunction](../../aspose.cells.gridweb/mainweb/onajaxcallfinishedclientfunction/) { get; set; } | Gets or sets the client side function name to be called when ajaxcall finished. The client function should be declared like this: function GridAjaxcallFinished() { alert(this.id+" ajaxcall finished "); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event. |
| [OnCellErrorClientFunction](../../aspose.cells.gridweb/mainweb/oncellerrorclientfunction/) { get; set; } | Gets or sets the client side function name to be called when a cell's validation is failed. The client function should be declared like this: function MyOnCellError(cell) { alert(this.getCellValueByCell(cell)); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event. |
| [OnCellSelectedAjaxCallBackClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedajaxcallbackclientfunction/) { get; set; } | Gets or sets the client side function to be called when a cell is selected. The client function should be declared like this: function MyOnSelectCellAjaxCallBack(cell,customerdata) { }Note: You may use the "this" pointer in the client function to point the grid control which fires the event. |
| [OnCellSelectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedclientfunction/) { get; set; } | Gets or sets the client side function to be called when a cell is selected. The client function should be declared like this: function MyOnSelectCell(cell) { GridWeb1.setCellValueByCell(cell, "test"); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event. |
| [OnCellUnselectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellunselectedclientfunction/) { get; set; } | Gets or sets the client side function to be called when a cell is unselected. The client function should be declared like this: function MyOnUnselectCell(cell) { this.setCellValueByCell(cell, "test"); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event. |
| [OnCellUpdatedClientFunction](../../aspose.cells.gridweb/mainweb/oncellupdatedclientfunction/) { get; set; } | Gets or sets the client side function name to be called when a cell's value is updated. The client function should be declared like this: function MyOnCellUpdated(cell) { alert(this.getCellValueByCell(cell)); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event. |
| [OnContextMenuShowClientFunction](../../aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/) { get; set; } | Gets or sets the client side function to be called when the context menu will be shown. The client function should be declared like this: function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("Delete", "block"); menu.setItemVisibility("Update", "none"); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event. |
| [OnDoubleClickCellClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickcellclientfunction/) { get; set; } | Gets or sets the client side function to be called when a cell is double clicked. The client function should be declared like this: function MyOnDoubleClickCell(cell) { this.setCellValueByCell(cell, "test"); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event. |
| [OnDoubleClickRowClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickrowclientfunction/) { get; set; } | Gets or sets the client side function to be called when a row is double clicked. The client function should be declared like this: function MyOnRowDoubleClick(row) { alert(row); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event. |
| [OnGridInitClientFunction](../../aspose.cells.gridweb/mainweb/ongridinitclientfunction/) { get; set; } | Gets or sets the client side function name to be called when the grid is initialized. The client function should be declared like this: function MyOnGridInit(grid) { alert("The grid is initialized: " + grid.id); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event. |
| [OnlyAuto](../../aspose.cells.gridweb/mainweb/onlyauto/) { get; set; } | Gets or sets whether only fit the rows which height are not customed,the default value is false |
| [OnPageChangeClientFunction](../../aspose.cells.gridweb/mainweb/onpagechangeclientfunction/) { get; set; } | Gets or sets the client side function to be called after page index changing.only take effect when EnablePaging is true. The client function should be declared like this: function MyOnPageChange(index) { console.log("current page is:"+index); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event. |
| [OnPageSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onpagesubmitclientfunction/) { get; set; } | Gets or sets the client function to be called before the page is submitted at client side. |
| [OnShapeSelectedClientFunction](../../aspose.cells.gridweb/mainweb/onshapeselectedclientfunction/) { get; set; } | Gets or sets the client side function to be called when a shape is selected. The client function should be declared like this: function MyOnSelectShape(shape) { var name=shape.getAttribute("namevalue") var text=shape.getAttribute("textvalue") var value=shape.getAttribute("controlvalue") var type=shape.getAttribute("msotype") }Note: You may use the "this" pointer in the client function to point the grid control which fires the event. |
| [OnSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onsubmitclientfunction/) { get; set; } | Gets or sets the client function to be called before the control is submitted at client side. The client function should be declared like this: function MyOnSubmit(arg, cancelEdit) { return true;} The arg is the submit argument, contains the command to be post to the server. The cancelEdit is boolean value indicates whether the control has discarded the user input before submit. The control will continue submitting if the function returns true. Note: You may use the "this" pointer in the client function to point the grid control which fires the event. |
| [PageSize](../../aspose.cells.gridweb/mainweb/pagesize/) { get; set; } | Gets or sets the page size in paging mode. |
| [PresetStyle](../../aspose.cells.gridweb/mainweb/presetstyle/) { get; set; } | Gets or sets the preset style. |
| [RefreshValidation](../../aspose.cells.gridweb/mainweb/refreshvalidation/) { get; set; } | Gets or sets whether to refresh validation value after cell value changes. |
| [RenderHiddenRow](../../aspose.cells.gridweb/mainweb/renderhiddenrow/) { get; set; } | Gets or sets whether the hidden row is rendered in GridControl,the default value is false. if you need to unhide the hidden row latter ,you shall set it as true |
| [RowHeightForCSV](../../aspose.cells.gridweb/mainweb/rowheightforcsv/) { get; set; } | Get or Set the row height value in point for csv file ,default value is 14.5. |
| [ScrollBarArrowColor](../../aspose.cells.gridweb/mainweb/scrollbararrowcolor/) { get; set; } | Specifies the color of the scrollbar's arrow button. |
| [ScrollBarBaseColor](../../aspose.cells.gridweb/mainweb/scrollbarbasecolor/) { get; set; } | Specifies the color of the scroll bar of the control. |
| [SelectCellBgColor](../../aspose.cells.gridweb/mainweb/selectcellbgcolor/) { get; set; } | Specifies the background color of the selected cells in multi-select range. |
| [SelectCellColor](../../aspose.cells.gridweb/mainweb/selectcellcolor/) { get; set; } | Specifies the color of the selected cells in multi-select range. |
| [SessionMode](../../aspose.cells.gridweb/mainweb/sessionmode/) { get; set; } | Gets or sets the session mode of the grid. |
| [SessionStorePath](../../aspose.cells.gridweb/mainweb/sessionstorepath/) { get; set; } | Gets or sets the session cache store path when session mode is File or ViewState, etc: gridweb.SessionStorePath="c:/mytempdir/session"; then it will store session data in c:/mytempdir/session |
| [Settings](../../aspose.cells.gridweb/mainweb/settings/) { get; set; } | Represents the workbook settings. |
| [ShowAddButton](../../aspose.cells.gridweb/mainweb/showaddbutton/) { get; set; } | Gets or sets whether to show the add worksheet button. |
| [ShowBottomBar](../../aspose.cells.gridweb/mainweb/showbottombar/) { get; set; } | Specifies whether to show the command bar(includes command bar and tab bar) at the bottom of the control. |
| [ShowCellEditBox](../../aspose.cells.gridweb/mainweb/showcelleditbox/) { get; set; } | whether Gridweb shows edit box toolbar as in MS-EXCEL.if enable ,a edit box for current cell will display in Gridweb. if we enable this feature, we need to import jquery js library in your aspx files to support this new feature. all the latest jquery version is ok. etc. |
| [ShowCommandBarAtTop](../../aspose.cells.gridweb/mainweb/showcommandbarattop/) { get; set; } | Specifies whether to show the command bar(includes command bar and tab bar) at the top of the control. |
| [ShowContextMenu](../../aspose.cells.gridweb/mainweb/showcontextmenu/) { get; set; } | Gets or sets whether to show the context menu. the default value is true. |
| [ShowDefaultGridLine](../../aspose.cells.gridweb/mainweb/showdefaultgridline/) { get; set; } | Gets or sets whether to show the default grid lines of the cells. |
| [ShowHeaderBar](../../aspose.cells.gridweb/mainweb/showheaderbar/) { get; set; } | Gets or sets whether to show header bar |
| [ShowLoading](../../aspose.cells.gridweb/mainweb/showloading/) { get; set; } | Specifies whether to show a loading dialogbox while postbacking to server. |
| [ShowLoadingPosition](../../aspose.cells.gridweb/mainweb/showloadingposition/) { get; set; } | Specifies the left,top postion(in px) to show the loading dialogbox while postbacking to server ,etc. 100,200 means the loading dialogbox's left,top postion is at 100px,200px . |
| [ShowSaveButton](../../aspose.cells.gridweb/mainweb/showsavebutton/) { get; set; } | Gets or sets whether to show the save button. |
| [ShowSubmitButton](../../aspose.cells.gridweb/mainweb/showsubmitbutton/) { get; set; } | Gets or sets whether to show the submit button. |
| [ShowTabBar](../../aspose.cells.gridweb/mainweb/showtabbar/) { get; set; } | Gets or sets whether to show the tab bar. |
| [ShowTabNavigation](../../aspose.cells.gridweb/mainweb/showtabnavigation/) { get; set; } | Gets or sets whether the tab navigation button is show,the default value is true. |
| [ShowUndoButton](../../aspose.cells.gridweb/mainweb/showundobutton/) { get; set; } | Gets or sets whether to show the undo button. |
| [SpanWrap](../../aspose.cells.gridweb/mainweb/spanwrap/) { get; set; } | Specifies whether to wrap content in the cell span.the default value is true. |
| [TabStyle](../../aspose.cells.gridweb/mainweb/tabstyle/) { get; set; } | Gets or sets the style of the tab bar. |
| [UseClientPageHeight](../../aspose.cells.gridweb/mainweb/useclientpageheight/) { get; set; } | Gets or sets whether gridweb use client page height as control height ,suitable for when set Height="100%",default value is false |
| [ViewPanelScrollLeft](../../aspose.cells.gridweb/mainweb/viewpanelscrollleft/) { get; set; } | Gets or sets the position of the scroll bar of the grid's view panel. |
| [ViewPanelScrollTop](../../aspose.cells.gridweb/mainweb/viewpanelscrolltop/) { get; set; } | Gets or sets the position of the scroll bar of the grid's view panel. |
| [ViewTableStyle](../../aspose.cells.gridweb/mainweb/viewtablestyle/) { get; set; } | Gets or sets the data view panel's style. |
| [WebWorksheets](../../aspose.cells.gridweb/mainweb/webworksheets/) { get; } |  |
| override [Width](../../aspose.cells.gridweb/mainweb/width/) { get; set; } | Gets or sets the width( System.Web.UI.WebControl.Unit ) of the control. |
| [WorkSheets](../../aspose.cells.gridweb/mainweb/worksheets/) { get; } | Gets or sets the collection of the worksheets. |
| [XhtmlMode](../../aspose.cells.gridweb/mainweb/xhtmlmode/) { get; set; } | Gets or sets whether to use XHTML style,the default value is true. |
| static [DPI](../../aspose.cells.gridweb/mainweb/dpi/) { get; set; } | Gets /Sets the DPI of the machine. |
| static [PictureCachePath](../../aspose.cells.gridweb/mainweb/picturecachepath/) { get; set; } | Gets or sets the image storage path for the workbook,all the shapes,images will be stored in this directory, the default path is acwcache under current application Base Directory users need to implement a schedule service to clean the files those are out of session time. |
## Methods
| Name | Description |
| --- | --- |
| [CalculateFormula](../../aspose.cells.gridweb/mainweb/calculateformula/)() | Calculates the result of formulas. |
| override [DataBind](../../aspose.cells.gridweb/mainweb/databind/)() | Bind the control and all its child contorls to the its datasource. |
| override [Dispose](../../aspose.cells.gridweb/mainweb/dispose/)() |  |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile)(Stream) | Imports from an excel file stream, including disk file stream or memory stream. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_2)(string) | Imports from an excel file. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_1)(Stream, string) | Imports from an excel file stream, including disk file stream or memory stream. |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile/#importexcelfile_3)(string, string) | Imports from an excel file. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/#loadcsvfile)(Stream) | Loads data from a CSV file stream. |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile/#loadcsvfile_1)(string) | Loads data from a CSV file. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/#loadhtmlfile)(Stream) | Loads data from a HTML file stream. |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile/#loadhtmlfile_1)(string) | Loads data from a HTML file. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/#loadspreadsheetmlfile)(Stream) | Loads data from a SpreadSheetML file stream. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile/#loadspreadsheetmlfile_1)(string) | Loads data from a SpreadSheetML file. |
| [RefreshChartShape](../../aspose.cells.gridweb/mainweb/refreshchartshape/)() | refresh all the chart image for the active worksheet . |
| override [RenderBeginTag](../../aspose.cells.gridweb/mainweb/renderbegintag/)(HtmlTextWriter) |  |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/#savecsvfile)(Stream) | Saves data to a CSV file stream. |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile/#savecsvfile_1)(string) | Saves data to a CSV file. |
| [SaveCustomStyleFile](../../aspose.cells.gridweb/mainweb/savecustomstylefile/)(string) | Saves current style data of the control to an xml file. Can be used to create your customized style file. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/#savehtmlfile)(Stream) | Saves data to a HTML file stream. |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile/#savehtmlfile_1)(string) | Saves data to a HTML file. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/#savespreadsheetmlfile)(Stream) | Saves data to a SpreadSheetML file stream. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile/#savespreadsheetmlfile_1)(string) | Saves data to a SpreadSheetML file. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile)(Stream) | Saves the worksheets to an excel file. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_3)(string) | Saves the worksheets to an excel file with Excel 2003 format. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_1)(Stream, GridSaveFormat) | Saves the worksheets to an excel file. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_2)(Stream, GridSaveOptions) | Saves the worksheets to an excel file. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_4)(string, GridSaveFormat) | Saves the worksheets to an excel file. |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile/#savetoexcelfile_5)(string, GridSaveOptions) | Saves the worksheets to an excel file. |
| [SetCustomStyle](../../aspose.cells.gridweb/mainweb/setcustomstyle/)(Stream) | sets the custom style file from stream including disk file stream or memory stream. |
## Events
| Name | Description |
| --- | --- |
| event [AfterColumnFilter](../../aspose.cells.gridweb/mainweb/aftercolumnfilter/) | Occurs after the column filtered. |
| event [AjaxCallFinished](../../aspose.cells.gridweb/mainweb/ajaxcallfinished/) | Fires when the ajax update of the control finished.(the EnableAJAX shall be set to true) |
| event [BeforeColumnFilter](../../aspose.cells.gridweb/mainweb/beforecolumnfilter/) | Occurs before the column to be filtered. |
| event [CellClickOnAjax](../../aspose.cells.gridweb/mainweb/cellclickonajax/) | Occurs when the cell is clicked,and need to do ajaxcallback for this event. |
| event [CellClientUpdate](../../aspose.cells.gridweb/mainweb/cellclientupdate/) | Occurs when a client cell update happen . When this event is fired, its parameter e.Argument contains the command's name. |
| event [CellCommand](../../aspose.cells.gridweb/mainweb/cellcommand/) | Occurs when a cell's command hyperlink is clicked. When this event is fired, its parameter e.Argument contains the command's name. |
| event [CellDoubleClick](../../aspose.cells.gridweb/mainweb/celldoubleclick/) | Occurs when the cell is double-clicked. |
| event [CellError](../../aspose.cells.gridweb/mainweb/cellerror/) | Occurs when a cell's input value error. |
| event [CellModifiedOnAjax](../../aspose.cells.gridweb/mainweb/cellmodifiedonajax/) | Occurs when the cell is modified in ajaxcall. |
| event [ColumnDeleted](../../aspose.cells.gridweb/mainweb/columndeleted/) | Occurs when user delete a column from client-side menu. |
| event [ColumnDeleting](../../aspose.cells.gridweb/mainweb/columndeleting/) | Occurs when user is trying to delete a column from the client-side menu. You may handle this event and set the cancel parameter to True to cancel a deleting operation. |
| event [ColumnDoubleClick](../../aspose.cells.gridweb/mainweb/columndoubleclick/) | Occurs when the column header is double-clicked. |
| event [ColumnInserted](../../aspose.cells.gridweb/mainweb/columninserted/) | Occurs when user insert a column from client-side menu. |
| event [CustomCommand](../../aspose.cells.gridweb/mainweb/customcommand/) | Occurs when user clicks a custom command button. |
| event [LoadCustomData](../../aspose.cells.gridweb/mainweb/loadcustomdata/) | Fires when the control's SessionMode is set to Custom and needs to load sheet data. You may handle this event in Custom Session mode to load sheet data from file or database. |
| event [PageIndexChanged](../../aspose.cells.gridweb/mainweb/pageindexchanged/) | Occurs when the control's sheet page index changed. |
| event [RowDeleted](../../aspose.cells.gridweb/mainweb/rowdeleted/) | Occurs when user has deleted a row from client-side menu. |
| event [RowDeleting](../../aspose.cells.gridweb/mainweb/rowdeleting/) | Occurs when user is trying to delete a row from the client-side menu. You may handle this event and throw a RejectDeleteException exception to cancel a deleting operation. |
| event [RowDoubleClick](../../aspose.cells.gridweb/mainweb/rowdoubleclick/) | Occurs when the row header is double-clicked. |
| event [RowInserted](../../aspose.cells.gridweb/mainweb/rowinserted/) | Occurs when user insert a row from client-side menu. |
| event [SaveCommand](../../aspose.cells.gridweb/mainweb/savecommand/) | Occurs when the "save" button is clicked. |
| event [SheetAdded](../../aspose.cells.gridweb/mainweb/sheetadded/) | Occurs when user add a worksheet from toolbar menu. |
| event [SheetDataUpdated](../../aspose.cells.gridweb/mainweb/sheetdataupdated/) | Occurs when the control has loaded the posted data and updated the sheet data. |
| event [SheetTabClick](../../aspose.cells.gridweb/mainweb/sheettabclick/) | Occurs when the sheet tab is clicked. |
| event [SubmitCommand](../../aspose.cells.gridweb/mainweb/submitcommand/) | Occurs when the "submit" button is clicked. |
| event [UndoCommand](../../aspose.cells.gridweb/mainweb/undocommand/) | Occurs when the "undo" button is clicked. |
### Examples
```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
//do your business
```
### See Also
* class [ExtWebControl](../extwebcontrol/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)
