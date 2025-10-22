##GridWebBean
Represents GridWeb java bean
**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebControl](../../com.aspose.gridweb/webcontrol), [com.aspose.gridweb.ExtWebControl](../../com.aspose.gridweb/extwebcontrol), [com.aspose.gridweb.MainWeb](../../com.aspose.gridweb/mainweb)
```
public class GridWebBean extends MainWeb
```
Represents GridWeb java bean
## Constructors
| Constructor | Description |
| --- | --- |
| [GridWebBean()](#GridWebBean--) | the default constructor of GridWebBean |
## Fields
| Field | Description |
| --- | --- |
| [AfterColumnFilter](#AfterColumnFilter) | Occurs after the column filtered. |
| [AjaxCallFinished](#AjaxCallFinished) | Fires when the ajax update of the control finished. |
| [BeforeColumnFilter](#BeforeColumnFilter) | Occurs before the column to be filtered. |
| [CellClickOnAjax](#CellClickOnAjax) | Occurs when the cell is clicked,and need to do ajaxcallback for this event. |
| [CellClientUpdate](#CellClientUpdate) | Occurs when a client cell update happen . |
| [CellCommand](#CellCommand) | Occurs when a cell's command hyperlink is clicked. |
| [CellDoubleClick](#CellDoubleClick) | Occurs when the cell is double-clicked. |
| [CellModifiedOnAjax](#CellModifiedOnAjax) | Occurs when the cell is modified in ajaxcall. |
| [ColumnDeleted](#ColumnDeleted) | Occurs when user delete a column from client-side menu. |
| [ColumnDeleting](#ColumnDeleting) | Occurs when user is trying to delete a column from the client-side menu. |
| [ColumnDoubleClick](#ColumnDoubleClick) | Occurs when the column header is double-clicked. |
| [ColumnInserted](#ColumnInserted) | Occurs when user insert a column from client-side menu. |
| [CustomCommand](#CustomCommand) | Occurs when user clicks a custom command button. |
| [LoadCustomData](#LoadCustomData) | Fires when the control's SessionMode is set to Custom and needs to load sheet data. |
| [PageIndexChanged](#PageIndexChanged) | Occurs when the control's sheet page index changed. |
| [RowDeleted](#RowDeleted) | Occurs when user has deleted a row from client-side menu. |
| [RowDeleting](#RowDeleting) | Occurs when user is trying to delete a row from the client-side menu. |
| [RowDoubleClick](#RowDoubleClick) | Occurs when the row header is double-clicked. |
| [RowInserted](#RowInserted) | Occurs when user insert a row from client-side menu. |
| [SaveCommand](#SaveCommand) | Occurs when the "save" button is clicked. |
| [SheetAdded](#SheetAdded) | Occurs when user add a worksheet from toolbar menu. |
| [SheetTabClick](#SheetTabClick) | Occurs when the sheet tab is clicked. |
| [SubmitCommand](#SubmitCommand) | Occurs when the "submit" button is clicked. |
| [UndoCommand](#UndoCommand) | Occurs when the "undo" button is clicked. |
## Methods
| Method | Description |
| --- | --- |
| [calculateFormula()](#calculateFormula--) | Calculates the result of formulas. |
| [createChildControls()](#createChildControls--) | implment CreateChildControls from WebControl,Internal used only. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getACWClientPath()](#getACWClientPath--) | Gets the web path of the script/image files of the control. |
| [getACWLanguageFileUrl()](#getACWLanguageFileUrl--) | Gets the web url of the language file of the control. |
| [getActiveCell()](#getActiveCell--) | Gets the active cell of the current sheet. |
| [getActiveCellBgColor()](#getActiveCellBgColor--) | Specifies the background color of the active cell. |
| [getActiveCellColor()](#getActiveCellColor--) | Specifies the color of the active cell. |
| [getActiveHeaderBgColor()](#getActiveHeaderBgColor--) | Specifies the background color of the active row/column header. |
| [getActiveHeaderColor()](#getActiveHeaderColor--) | Specifies the color of the active row/column header. |
| [getActiveSheet()](#getActiveSheet--) | Gets the active sheet |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Gets the active sheet index. |
| [getActiveTabStyle()](#getActiveTabStyle--) | Specifies the style of the active tab. |
| [getAutoRefreshChart()](#getAutoRefreshChart--) | Gets whether the Chart image is updated while updating the cell value.the default is true |
| [getBackColor()](#getBackColor--) | Gets the BackColor in the WebControl |
| [getBeanID()](#getBeanID--) | get the html id of the bean |
| [getBorderColor()](#getBorderColor--) | Gets the BorderColor in the WebControl |
| [getBorderStyle()](#getBorderStyle--) | Gets the BorderStyle in the WebControl |
| [getBorderWidth()](#getBorderWidth--) | Gets the BorderWidth in the WebControl |
| [getBottomTableStyle()](#getBottomTableStyle--) | Gets the style of the bottom bar of the control. |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | Gets the CssClass in the WebControl |
| [getCurrentPageIndex()](#getCurrentPageIndex--) | Gets the current page index in paging mode. |
| [getCustomCalculationEngine()](#getCustomCalculationEngine--) | Represents user's custom calculation engine to extend the default calculation engine of Aspose.Cells. |
| [getCustomCommandButtons()](#getCustomCommandButtons--) | Gets the custom command button collection |
| [getCustomStyleFileName()](#getCustomStyleFileName--) | Gets the custom style file name. |
| [getDPI()](#getDPI--) | Gets /Sets the DPI of the machine. |
| [getDefaultFontName()](#getDefaultFontName--) | Gets the control's default font name. |
| [getDefaultFontSize()](#getDefaultFontSize--) | Gets the control's default font size. |
| [getDefaultGridLineColor()](#getDefaultGridLineColor--) | Gets the default grid line's color. |
| [getDisplayCellTip()](#getDisplayCellTip--) | Gets whether to show tips. the default value is true. |
| [getEditMode()](#getEditMode--) | Gets the control's edit mode. |
| [getEnableAJAX()](#getEnableAJAX--) | Gets whether to use AJAX call . the default value is true. |
| [getEnableAsync()](#getEnableAsync--) | Gets whether load cells data in asynchronous way,suggest to apply for one sheet with more than 10000 cells. |
| [getEnableClientColumnOperations()](#getEnableClientColumnOperations--) | Gets whether to enable the client side column operations. |
| [getEnableClientFreeze()](#getEnableClientFreeze--) | Gets whether to enable the client side freezing operations. |
| [getEnableClientMergeOperations()](#getEnableClientMergeOperations--) | Gets whether to enable the client side merge operations. |
| [getEnableClientResizeColumnRow()](#getEnableClientResizeColumnRow--) | Gets whether to enable the client side resize column and row. |
| [getEnableClientRowOperations()](#getEnableClientRowOperations--) | Gets whether to enable the client side row operations. |
| [getEnableDoubleClickEvent()](#getEnableDoubleClickEvent--) | Gets whether to enable customer side double-click event. |
| [getEnableMetalLightEffect()](#getEnableMetalLightEffect--) | Gets whether to apply metal light effect. |
| [getEnablePaging()](#getEnablePaging--) | Gets whether to enable the control's paging mode. |
| [getEnableStyleDialogbox()](#getEnableStyleDialogbox--) | Gets whether to enable the client side style dialogbox. |
| [getEnabled()](#getEnabled--) | Gets the Enabled in the WebControl |
| [getFilteredPaging()](#getFilteredPaging--) | Gets whether to enable the paging after data filtered,will take affect when EnablePaging is true. |
| [getFont()](#getFont--) | Gets the Font in the WebControl |
| [getForceValidation()](#getForceValidation--) | Gets whether to force customer side validation. |
| [getForeColor()](#getForeColor--) | Gets the ForeColor in the WebControl |
| [getFrameTableStyle()](#getFrameTableStyle--) | Gets the frame style of the control. |
| [getGoonDefaultSaveOperation()](#getGoonDefaultSaveOperation--) | Gets whether GridWeb will do the default save operation ,the default value is true. |
| [getHTMLBody()](#getHTMLBody--) | the html code of the bean for html body, it shall be get after call of method init and prepareRender |
| [getHTMLHead()](#getHTMLHead--) | the html code of the bean for html head, it shall be get after call of method init and prepareRender |
| [getHeaderBarHeight()](#getHeaderBarHeight--) | Gets the height( System.Web.UI.WebControl.Unit ) of the top header bar of the control. |
| [getHeaderBarStyle()](#getHeaderBarStyle--) | Gets the header bar's style. |
| [getHeaderBarTableStyle()](#getHeaderBarTableStyle--) | Gets the header bar style of the control. |
| [getHeaderBarWidth()](#getHeaderBarWidth--) | Gets the width( System.Web.UI.WebControl.Unit ) or the left header bar of the control. |
| [getHeight()](#getHeight--) | Gets the height( System.Web.UI.WebControl.Unit ) of the control. |
| [getIgnoreStyleWithNoData()](#getIgnoreStyleWithNoData--) | Gets whether GridWeb ignores showing rows or columns that do not contain cell values but are still styled. |
| [getLoadOptions()](#getLoadOptions--) | Represents the loadoptions for GridWeb. |
| [getMaxColumn()](#getMaxColumn--) | Gets the maximum display column index(zero based) of the web sheet. |
| [getMaxRow()](#getMaxRow--) | Gets the maximum display row index(zero based) of the web sheet. |
| [getMessage()](#getMessage--) | Gets the message for the grid. |
| [getMinColumn()](#getMinColumn--) | Gets the minimum display column index(zero based) of the web sheet. |
| [getMinRow()](#getMinRow--) | Gets the minimum display row index(zero based) of the web sheet. |
| [getModifiedCells()](#getModifiedCells--) | Gets the collection of the cells that modified by the client. |
| [getNeedRenderGroupRows()](#getNeedRenderGroupRows--) | Gets whether to show grouprows . |
| [getNoHScroll()](#getNoHScroll--) | Gets a value indicating whether the horizontal scroll bar is hidden. |
| [getNoScroll()](#getNoScroll--) | Gets whether to show scroll bar . |
| [getNoVScroll()](#getNoVScroll--) | Gets a value indicating whether the vertical scroll bar is hidden. |
| [getOnAjaxCallFinishedClientFunction()](#getOnAjaxCallFinishedClientFunction--) | Gets the client side function name to be called when ajaxcall finished. |
| [getOnCellErrorClientFunction()](#getOnCellErrorClientFunction--) | Gets the client side function name to be called when a cell's validation is failed. |
| [getOnCellSelectedAjaxCallBackClientFunction()](#getOnCellSelectedAjaxCallBackClientFunction--) | Gets the client side function to be called when a cell is selected. |
| [getOnCellSelectedClientFunction()](#getOnCellSelectedClientFunction--) | Gets the client side function to be called when a cell is selected. |
| [getOnCellUnselectedClientFunction()](#getOnCellUnselectedClientFunction--) | Gets the client side function to be called when a cell is unselected. |
| [getOnCellUpdatedClientFunction()](#getOnCellUpdatedClientFunction--) | Gets the client side function name to be called when a cell's value is updated. |
| [getOnContextMenuShowClientFunction()](#getOnContextMenuShowClientFunction--) | Gets the client side function to be called when the context menu will be shown. |
| [getOnDoubleClickCellClientFunction()](#getOnDoubleClickCellClientFunction--) | Gets the client side function to be called when a cell is double clicked. |
| [getOnDoubleClickRowClientFunction()](#getOnDoubleClickRowClientFunction--) | Gets the client side function to be called when a row is double clicked. |
| [getOnGridInitClientFunction()](#getOnGridInitClientFunction--) | Gets the client side function name to be called when the grid is initialized. |
| [getOnPageChangeClientFunction()](#getOnPageChangeClientFunction--) | Gets the client side function to be called after page index changing.only take effect when EnablePaging is true. |
| [getOnPageSubmitClientFunction()](#getOnPageSubmitClientFunction--) | Gets the client function to be called before the page is submitted at client side. |
| [getOnShapeSelectedClientFunction()](#getOnShapeSelectedClientFunction--) | Gets the client side function to be called when a shape is selected. |
| [getOnSubmitClientFunction()](#getOnSubmitClientFunction--) | Gets the client function to be called before the control is submitted at client side. |
| [getOnlyAuto()](#getOnlyAuto--) | Gets whether only fit the rows which height are not customed,the default value is false |
| [getPageSize()](#getPageSize--) | Gets the page size in paging mode. |
| [getPictureCachePath()](#getPictureCachePath--) | Gets the image storage path for the workbook,all the shapes,images will be stored in this directory, the default path is acwcache under current application Base Directory users need to implement a schedule service to clean the files those are out of session time. |
| [getPresetStyle()](#getPresetStyle--) | Gets the preset style. |
| [getRefreshValidation()](#getRefreshValidation--) | Gets whether to refresh validation value after cell value changes. |
| [getRenderHiddenRow()](#getRenderHiddenRow--) | Gets whether the hidden row is rendered in GridControl,the default value is false. |
| [getRowHeightForCSV()](#getRowHeightForCSV--) | Gets the row height value in point for csv file ,default value is 14.5. |
| [getScrollBarArrowColor()](#getScrollBarArrowColor--) | Specifies the color of the scrollbar's arrow button. |
| [getScrollBarBaseColor()](#getScrollBarBaseColor--) | Specifies the color of the scroll bar of the control. |
| [getSelectCellBgColor()](#getSelectCellBgColor--) | Specifies the background color of the selected cells in multi-select range. |
| [getSelectCellColor()](#getSelectCellColor--) | Specifies the color of the selected cells in multi-select range. |
| [getSessionStorePath()](#getSessionStorePath--) | Gets the session cache store path when session mode is File or ViewState, etc: gridweb.SessionStorePath="c:/mytempdir/session"; then it will store session data in c:/mytempdir/session |
| [getSettings()](#getSettings--) | Represents the workbook settings. |
| [getShowAddButton()](#getShowAddButton--) | Gets whether to show the add worksheet button. |
| [getShowBottomBar()](#getShowBottomBar--) | Specifies whether to show the command bar(includes command bar and tab bar) at the bottom of the control. |
| [getShowCellEditBox()](#getShowCellEditBox--) | whether Gridweb shows edit box toolbar as in MS-EXCEL.if enable ,a edit box for current cell will display in Gridweb. |
| [getShowCommandBarAtTop()](#getShowCommandBarAtTop--) | Specifies whether to show the command bar(includes command bar and tab bar) at the top of the control. |
| [getShowContextMenu()](#getShowContextMenu--) | Gets whether to show the context menu. the default value is true. |
| [getShowDefaultGridLine()](#getShowDefaultGridLine--) | Gets whether to show the default grid lines of the cells. |
| [getShowHeaderBar()](#getShowHeaderBar--) | Gets whether to show header bar |
| [getShowLoading()](#getShowLoading--) | Specifies whether to show a loading dialogbox while postbacking to server. |
| [getShowLoadingPosition()](#getShowLoadingPosition--) | Specifies the left,top postion(in px) to show the loading dialogbox while postbacking to server ,etc. 100,200 means the loading dialogbox's left,top postion is at 100px,200px . |
| [getShowSaveButton()](#getShowSaveButton--) | Gets whether to show the save button. |
| [getShowSubmitButton()](#getShowSubmitButton--) | Gets whether to show the submit button. |
| [getShowTabBar()](#getShowTabBar--) | Gets whether to show the tab bar. |
| [getShowTabNavigation()](#getShowTabNavigation--) | Gets whether the tab navigation button is show,the default value is true. |
| [getShowUndoButton()](#getShowUndoButton--) | Gets whether to show the undo button. |
| [getSpanWrap()](#getSpanWrap--) | Specifies whether to wrap content in the cell span.the default value is true. |
| [getTabIndex()](#getTabIndex--) | Gets the TabIndex in the WebControl |
| [getTabStyle()](#getTabStyle--) | Gets the style of the tab bar. |
| [getToolTip()](#getToolTip--) | Gets the ToolTip in the WebControl |
| [getUseClientPageHeight()](#getUseClientPageHeight--) | Gets whether gridweb use client page height as control height ,suitable for when set Height="100%",default value is false |
| [getViewPanelScrollLeft()](#getViewPanelScrollLeft--) | Gets the position of the scroll bar of the grid's view panel. |
| [getViewPanelScrollTop()](#getViewPanelScrollTop--) | Gets the position of the scroll bar of the grid's view panel. |
| [getViewTableStyle()](#getViewTableStyle--) | Gets the data view panel's style. |
| [getWidth()](#getWidth--) | Gets the width( System.Web.UI.WebControl.Unit ) of the control. |
| [getWorkSheets()](#getWorkSheets--) | Gets the collection of the worksheets. |
| [getXhtmlMode()](#getXhtmlMode--) | Gets whether to use XHTML style,the default value is true. |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream stream)](#importExcelFile-java.io.InputStream-) | Imports from an excel file stream, including disk file stream or memory stream. |
| [importExcelFile(InputStream stream, String passwordtoOpen)](#importExcelFile-java.io.InputStream-java.lang.String-) | Imports from an excel file stream, including disk file stream or memory stream. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | Imports from an excel file. |
| [importExcelFile(String fileName, String passwordtoOpen)](#importExcelFile-java.lang.String-java.lang.String-) | Imports from an excel file. |
| [init()](#init--) | the bean shall be initialized by the servlet request and response of the current page |
| [isCalculateFormula()](#isCalculateFormula--) | Gets whether to calculate formula after cell value changes or after import File. |
| [loadCSVFile(InputStream stream)](#loadCSVFile-java.io.InputStream-) | Loads data from a CSV file stream. |
| [loadCSVFile(String fileName)](#loadCSVFile-java.lang.String-) | Loads data from a CSV file. |
| [loadHTMLFile(InputStream stream)](#loadHTMLFile-java.io.InputStream-) | Loads data from a HTML file stream. |
| [loadHTMLFile(String fileName)](#loadHTMLFile-java.lang.String-) | Loads data from a HTML file. |
| [loadSpreadSheetMLFile(InputStream stream)](#loadSpreadSheetMLFile-java.io.InputStream-) | Loads data from a SpreadSheetML file stream. |
| [loadSpreadSheetMLFile(String fileName)](#loadSpreadSheetMLFile-java.lang.String-) | Loads data from a SpreadSheetML file. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [prepareRender()](#prepareRender--) | the method shall be called before render GridWeb bean |
| [refreshChartShape()](#refreshChartShape--) | refresh all the chart image for the active worksheet . |
| [saveCSVFile(OutputStream stream)](#saveCSVFile-java.io.OutputStream-) | Saves data to a CSV file stream. |
| [saveCSVFile(String targetFile)](#saveCSVFile-java.lang.String-) | Saves data to a CSV file. |
| [saveCustomStyleFile(String fileName)](#saveCustomStyleFile-java.lang.String-) | Saves current style data of the control to an xml file. |
| [saveHTMLFile(OutputStream stream)](#saveHTMLFile-java.io.OutputStream-) | Saves data to a HTML file stream. |
| [saveHTMLFile(String targetFile)](#saveHTMLFile-java.lang.String-) | Saves data to a HTML file. |
| [saveSpreadSheetMLFile(OutputStream stream)](#saveSpreadSheetMLFile-java.io.OutputStream-) | Saves data to a SpreadSheetML file stream. |
| [saveSpreadSheetMLFile(String targetFile)](#saveSpreadSheetMLFile-java.lang.String-) | Saves data to a SpreadSheetML file. |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | Saves the worksheets to an excel file. |
| [saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)](#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-) | Saves the worksheets to an excel file. |
| [saveToExcelFile(OutputStream stream, int format)](#saveToExcelFile-java.io.OutputStream-int-) | Saves the worksheets to an excel file. |
| [saveToExcelFile(String targetFile)](#saveToExcelFile-java.lang.String-) | Saves the worksheets to an excel file with Excel 2003 format. |
| [saveToExcelFile(String targetFile, GridSaveOptions saveOptions)](#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-) | Saves the worksheets to an excel file. |
| [saveToExcelFile(String targetFile, int format)](#saveToExcelFile-java.lang.String-int-) | Saves the worksheets to an excel file. |
| [setACWClientPath(String value)](#setACWClientPath-java.lang.String-) | Sets the web path of the script/image files of the control. |
| [setACWLanguageFileUrl(String value)](#setACWLanguageFileUrl-java.lang.String-) | Sets the web url of the language file of the control. |
| [setActiveCell(GridCell value)](#setActiveCell-com.aspose.gridweb.GridCell-) | Sets the active cell of the current sheet. |
| [setActiveCellBgColor(Color value)](#setActiveCellBgColor-com.aspose.gridweb.Color-) | Specifies the background color of the active cell. |
| [setActiveCellColor(Color value)](#setActiveCellColor-com.aspose.gridweb.Color-) | Specifies the color of the active cell. |
| [setActiveHeaderBgColor(Color value)](#setActiveHeaderBgColor-com.aspose.gridweb.Color-) | Specifies the background color of the active row/column header. |
| [setActiveHeaderColor(Color value)](#setActiveHeaderColor-com.aspose.gridweb.Color-) | Specifies the color of the active row/column header. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Sets the active sheet index. |
| [setActiveTabStyle(GridTableItemStyle value)](#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-) | Specifies the style of the active tab. |
| [setAutoRefreshChart(boolean value)](#setAutoRefreshChart-boolean-) | Sets whether the Chart image is updated while updating the cell value.the default is true |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | Sets the BackColor in the WebControl |
| [setBeanID(String beanID)](#setBeanID-java.lang.String-) | set the html id of the bean |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | Sets the BorderColor in the WebControl |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Sets the BorderStyle in the WebControl |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | Sets the BorderWidth in the WebControl |
| [setBottomTableStyle(GridTableStyle value)](#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-) | Sets the style of the bottom bar of the control. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Sets whether to calculate formula after cell value changes or after import File. |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | Sets the CssClass in the WebControl |
| [setCurrentPageIndex(int value)](#setCurrentPageIndex-int-) | Sets the current page index in paging mode. |
| [setCustomCalculationEngine(GridAbstractCalculationEngine value)](#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-) | Represents user's custom calculation engine to extend the default calculation engine of Aspose.Cells. |
| [setCustomStyle(InputStream stream)](#setCustomStyle-java.io.InputStream-) | sets the custom style file from stream including disk file stream or memory stream. |
| [setCustomStyleFileName(String value)](#setCustomStyleFileName-java.lang.String-) | Sets the custom style file name. |
| [setDPI(double value)](#setDPI-double-) | Gets /Sets the DPI of the machine. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Sets the control's default font name. |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | Sets the control's default font size. |
| [setDefaultGridLineColor(Color value)](#setDefaultGridLineColor-com.aspose.gridweb.Color-) | Sets the default grid line's color. |
| [setDisplayCellTip(boolean value)](#setDisplayCellTip-boolean-) | Sets whether to show tips. the default value is true. |
| [setEditMode(boolean value)](#setEditMode-boolean-) | Sets the control's edit mode. |
| [setEnableAJAX(boolean value)](#setEnableAJAX-boolean-) | Sets whether to use AJAX call . the default value is true. |
| [setEnableAsync(boolean value)](#setEnableAsync-boolean-) | Sets whether load cells data in asynchronous way,suggest to apply for one sheet with more than 10000 cells. |
| [setEnableClientColumnOperations(boolean value)](#setEnableClientColumnOperations-boolean-) | Sets whether to enable the client side column operations. |
| [setEnableClientFreeze(boolean value)](#setEnableClientFreeze-boolean-) | Sets whether to enable the client side freezing operations. |
| [setEnableClientMergeOperations(boolean value)](#setEnableClientMergeOperations-boolean-) | Sets whether to enable the client side merge operations. |
| [setEnableClientResizeColumnRow(boolean value)](#setEnableClientResizeColumnRow-boolean-) | Sets whether to enable the client side resize column and row. |
| [setEnableClientRowOperations(boolean value)](#setEnableClientRowOperations-boolean-) | Sets whether to enable the client side row operations. |
| [setEnableDoubleClickEvent(boolean value)](#setEnableDoubleClickEvent-boolean-) | Sets whether to enable customer side double-click event. |
| [setEnableMetalLightEffect(boolean value)](#setEnableMetalLightEffect-boolean-) | Sets whether to apply metal light effect. |
| [setEnablePaging(boolean value)](#setEnablePaging-boolean-) | Sets whether to enable the control's paging mode. |
| [setEnableStyleDialogbox(boolean value)](#setEnableStyleDialogbox-boolean-) | Sets whether to enable the client side style dialogbox. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Sets the Enabled in the WebControl |
| [setFilteredPaging(boolean value)](#setFilteredPaging-boolean-) | Sets whether to enable the paging after data filtered,will take affect when EnablePaging is true. |
| [setForceValidation(boolean value)](#setForceValidation-boolean-) | Sets whether to force customer side validation. |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | Sets the ForeColor in the WebControl |
| [setFrameTableStyle(GridTableStyle value)](#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-) | Sets the frame style of the control. |
| [setGoonDefaultSaveOperation(boolean value)](#setGoonDefaultSaveOperation-boolean-) | Sets whether GridWeb will do the default save operation ,the default value is true. |
| [setHeaderBarHeight(Unit value)](#setHeaderBarHeight-com.aspose.gridweb.Unit-) | Sets the height( System.Web.UI.WebControl.Unit ) of the top header bar of the control. |
| [setHeaderBarStyle(GridTableItemStyle value)](#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-) | Sets the header bar's style. |
| [setHeaderBarTableStyle(GridTableStyle value)](#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-) | Sets the header bar style of the control. |
| [setHeaderBarWidth(Unit value)](#setHeaderBarWidth-com.aspose.gridweb.Unit-) | Sets the width( System.Web.UI.WebControl.Unit ) or the left header bar of the control. |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | Sets the height( System.Web.UI.WebControl.Unit ) of the control. |
| [setIgnoreStyleWithNoData(boolean value)](#setIgnoreStyleWithNoData-boolean-) | Sets whether GridWeb ignores showing rows or columns that do not contain cell values but are still styled. |
| [setLoadOptions(GridLoadOptions value)](#setLoadOptions-com.aspose.gridweb.GridLoadOptions-) | Represents the loadoptions for GridWeb. |
| [setMaxColumn(int value)](#setMaxColumn-int-) | Sets the maximum display column index(zero based) of the web sheet. |
| [setMaxRow(int value)](#setMaxRow-int-) | Sets the maximum display row index(zero based) of the web sheet. |
| [setMessage(String value)](#setMessage-java.lang.String-) | Sets the message for the grid. |
| [setMinColumn(int value)](#setMinColumn-int-) | Sets the minimum display column index(zero based) of the web sheet. |
| [setMinRow(int value)](#setMinRow-int-) | Sets the minimum display row index(zero based) of the web sheet. |
| [setNeedRenderGroupRows(boolean value)](#setNeedRenderGroupRows-boolean-) | Sets whether to show grouprows . |
| [setNoHScroll(boolean value)](#setNoHScroll-boolean-) | Sets a value indicating whether the horizontal scroll bar is hidden. |
| [setNoScroll(boolean value)](#setNoScroll-boolean-) | Sets whether to show scroll bar . |
| [setNoVScroll(boolean value)](#setNoVScroll-boolean-) | Sets a value indicating whether the vertical scroll bar is hidden. |
| [setOnAjaxCallFinishedClientFunction(String value)](#setOnAjaxCallFinishedClientFunction-java.lang.String-) | Sets the client side function name to be called when ajaxcall finished. |
| [setOnCellErrorClientFunction(String value)](#setOnCellErrorClientFunction-java.lang.String-) | Sets the client side function name to be called when a cell's validation is failed. |
| [setOnCellSelectedAjaxCallBackClientFunction(String value)](#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-) | Sets the client side function to be called when a cell is selected. |
| [setOnCellSelectedClientFunction(String value)](#setOnCellSelectedClientFunction-java.lang.String-) | Sets the client side function to be called when a cell is selected. |
| [setOnCellUnselectedClientFunction(String value)](#setOnCellUnselectedClientFunction-java.lang.String-) | Sets the client side function to be called when a cell is unselected. |
| [setOnCellUpdatedClientFunction(String value)](#setOnCellUpdatedClientFunction-java.lang.String-) | Sets the client side function name to be called when a cell's value is updated. |
| [setOnContextMenuShowClientFunction(String value)](#setOnContextMenuShowClientFunction-java.lang.String-) | Sets the client side function to be called when the context menu will be shown. |
| [setOnDoubleClickCellClientFunction(String value)](#setOnDoubleClickCellClientFunction-java.lang.String-) | Sets the client side function to be called when a cell is double clicked. |
| [setOnDoubleClickRowClientFunction(String value)](#setOnDoubleClickRowClientFunction-java.lang.String-) | Sets the client side function to be called when a row is double clicked. |
| [setOnGridInitClientFunction(String value)](#setOnGridInitClientFunction-java.lang.String-) | Sets the client side function name to be called when the grid is initialized. |
| [setOnPageChangeClientFunction(String value)](#setOnPageChangeClientFunction-java.lang.String-) | Sets the client side function to be called after page index changing.only take effect when EnablePaging is true. |
| [setOnPageSubmitClientFunction(String value)](#setOnPageSubmitClientFunction-java.lang.String-) | Sets the client function to be called before the page is submitted at client side. |
| [setOnShapeSelectedClientFunction(String value)](#setOnShapeSelectedClientFunction-java.lang.String-) | Sets the client side function to be called when a shape is selected. |
| [setOnSubmitClientFunction(String value)](#setOnSubmitClientFunction-java.lang.String-) | Sets the client function to be called before the control is submitted at client side. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Sets whether only fit the rows which height are not customed,the default value is false |
| [setPageSize(int value)](#setPageSize-int-) | Sets the page size in paging mode. |
| [setPictureCachePath(String value)](#setPictureCachePath-java.lang.String-) | Sets the image storage path for the workbook,all the shapes,images will be stored in this directory, the default path is acwcache under current application Base Directory users need to implement a schedule service to clean the files those are out of session time. |
| [setPresetStyle(int value)](#setPresetStyle-int-) | Sets the preset style. |
| [setRefreshValidation(boolean value)](#setRefreshValidation-boolean-) | Sets whether to refresh validation value after cell value changes. |
| [setRenderHiddenRow(boolean value)](#setRenderHiddenRow-boolean-) | Sets whether the hidden row is rendered in GridControl,the default value is false. |
| [setRowHeightForCSV(double value)](#setRowHeightForCSV-double-) | Sets the row height value in point for csv file ,default value is 14.5. |
| [setScrollBarArrowColor(Color value)](#setScrollBarArrowColor-com.aspose.gridweb.Color-) | Specifies the color of the scrollbar's arrow button. |
| [setScrollBarBaseColor(Color value)](#setScrollBarBaseColor-com.aspose.gridweb.Color-) | Specifies the color of the scroll bar of the control. |
| [setSelectCellBgColor(Color value)](#setSelectCellBgColor-com.aspose.gridweb.Color-) | Specifies the background color of the selected cells in multi-select range. |
| [setSelectCellColor(Color value)](#setSelectCellColor-com.aspose.gridweb.Color-) | Specifies the color of the selected cells in multi-select range. |
| [setSessionStorePath(String value)](#setSessionStorePath-java.lang.String-) | Sets the session cache store path when session mode is File or ViewState, etc: gridweb.SessionStorePath="c:/mytempdir/session"; then it will store session data in c:/mytempdir/session |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridweb.GridWorkbookSettings-) | Represents the workbook settings. |
| [setShowAddButton(boolean value)](#setShowAddButton-boolean-) | Sets whether to show the add worksheet button. |
| [setShowBottomBar(boolean value)](#setShowBottomBar-boolean-) | Specifies whether to show the command bar(includes command bar and tab bar) at the bottom of the control. |
| [setShowCellEditBox(boolean value)](#setShowCellEditBox-boolean-) | whether Gridweb shows edit box toolbar as in MS-EXCEL.if enable ,a edit box for current cell will display in Gridweb. |
| [setShowCommandBarAtTop(boolean value)](#setShowCommandBarAtTop-boolean-) | Specifies whether to show the command bar(includes command bar and tab bar) at the top of the control. |
| [setShowContextMenu(boolean value)](#setShowContextMenu-boolean-) | Sets whether to show the context menu. the default value is true. |
| [setShowDefaultGridLine(boolean value)](#setShowDefaultGridLine-boolean-) | Sets whether to show the default grid lines of the cells. |
| [setShowHeaderBar(boolean value)](#setShowHeaderBar-boolean-) | Sets whether to show header bar |
| [setShowLoading(boolean value)](#setShowLoading-boolean-) | Specifies whether to show a loading dialogbox while postbacking to server. |
| [setShowLoadingPosition(String value)](#setShowLoadingPosition-java.lang.String-) | Specifies the left,top postion(in px) to show the loading dialogbox while postbacking to server ,etc. 100,200 means the loading dialogbox's left,top postion is at 100px,200px . |
| [setShowSaveButton(boolean value)](#setShowSaveButton-boolean-) | Sets whether to show the save button. |
| [setShowSubmitButton(boolean value)](#setShowSubmitButton-boolean-) | Sets whether to show the submit button. |
| [setShowTabBar(boolean value)](#setShowTabBar-boolean-) | Sets whether to show the tab bar. |
| [setShowTabNavigation(boolean value)](#setShowTabNavigation-boolean-) | Sets whether the tab navigation button is show,the default value is true. |
| [setShowUndoButton(boolean value)](#setShowUndoButton-boolean-) | Sets whether to show the undo button. |
| [setSpanWrap(boolean value)](#setSpanWrap-boolean-) | Specifies whether to wrap content in the cell span.the default value is true. |
| [setTabIndex(short value)](#setTabIndex-short-) | Sets the TabIndex in the WebControl |
| [setTabStyle(GridTableItemStyle value)](#setTabStyle-com.aspose.gridweb.GridTableItemStyle-) | Sets the style of the tab bar. |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | Sets the ToolTip in the WebControl |
| [setUseClientPageHeight(boolean value)](#setUseClientPageHeight-boolean-) | Sets whether gridweb use client page height as control height ,suitable for when set Height="100%",default value is false |
| [setViewPanelScrollLeft(String value)](#setViewPanelScrollLeft-java.lang.String-) | Sets the position of the scroll bar of the grid's view panel. |
| [setViewPanelScrollTop(String value)](#setViewPanelScrollTop-java.lang.String-) | Sets the position of the scroll bar of the grid's view panel. |
| [setViewTableStyle(GridTableStyle value)](#setViewTableStyle-com.aspose.gridweb.GridTableStyle-) | Sets the data view panel's style. |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Sets the width( System.Web.UI.WebControl.Unit ) of the control. |
| [setXhtmlMode(boolean value)](#setXhtmlMode-boolean-) | Sets whether to use XHTML style,the default value is true. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWebBean() {#GridWebBean--}
```
public GridWebBean()
```
the default constructor of GridWebBean
### AfterColumnFilter {#AfterColumnFilter}
```
public RowColumnEventHandler AfterColumnFilter
```
Occurs after the column filtered.
### AjaxCallFinished {#AjaxCallFinished}
```
public WorkbookEventHandler AjaxCallFinished
```
Fires when the ajax update of the control finished.(the EnableAJAX shall be set to true)
### BeforeColumnFilter {#BeforeColumnFilter}
```
public RowColumnEventHandler BeforeColumnFilter
```
Occurs before the column to be filtered.
### CellClickOnAjax {#CellClickOnAjax}
```
public CellEventStringHandler CellClickOnAjax
```
Occurs when the cell is clicked,and need to do ajaxcallback for this event.
### CellClientUpdate {#CellClientUpdate}
```
public CellEventHandler CellClientUpdate
```
Occurs when a client cell update happen . When this event is fired, its parameter e.Argument contains the command's name.
### CellCommand {#CellCommand}
```
public CellEventHandler CellCommand
```
Occurs when a cell's command hyperlink is clicked. When this event is fired, its parameter e.Argument contains the command's name.
### CellDoubleClick {#CellDoubleClick}
```
public CellEventHandler CellDoubleClick
```
Occurs when the cell is double-clicked.
### CellModifiedOnAjax {#CellModifiedOnAjax}
```
public CellEventHandler CellModifiedOnAjax
```
Occurs when the cell is modified in ajaxcall.
### ColumnDeleted {#ColumnDeleted}
```
public RowColumnEventHandler ColumnDeleted
```
Occurs when user delete a column from client-side menu.
### ColumnDeleting {#ColumnDeleting}
```
public RowColumnEventHandler ColumnDeleting
```
Occurs when user is trying to delete a column from the client-side menu. You may handle this event and set the cancel parameter to True to cancel a deleting operation.
### ColumnDoubleClick {#ColumnDoubleClick}
```
public RowColumnEventHandler ColumnDoubleClick
```
Occurs when the column header is double-clicked.
### ColumnInserted {#ColumnInserted}
```
public RowColumnEventHandler ColumnInserted
```
Occurs when user insert a column from client-side menu.
### CustomCommand {#CustomCommand}
```
public CustomCommandEventHandler CustomCommand
```
Occurs when user clicks a custom command button.
### LoadCustomData {#LoadCustomData}
```
public WorkbookEventHandler LoadCustomData
```
Fires when the control's SessionMode is set to Custom and needs to load sheet data. You may handle this event in Custom Session mode to load sheet data from file or database.
### PageIndexChanged {#PageIndexChanged}
```
public WorkbookEventHandler PageIndexChanged
```
Occurs when the control's sheet page index changed.
### RowDeleted {#RowDeleted}
```
public RowColumnEventHandler RowDeleted
```
Occurs when user has deleted a row from client-side menu.
### RowDeleting {#RowDeleting}
```
public RowColumnEventHandler RowDeleting
```
Occurs when user is trying to delete a row from the client-side menu. You may handle this event and throw a RejectDeleteException exception to cancel a deleting operation.
### RowDoubleClick {#RowDoubleClick}
```
public RowColumnEventHandler RowDoubleClick
```
Occurs when the row header is double-clicked.
### RowInserted {#RowInserted}
```
public RowColumnEventHandler RowInserted
```
Occurs when user insert a row from client-side menu.
### SaveCommand {#SaveCommand}
```
public WorkbookEventHandler SaveCommand
```
Occurs when the "save" button is clicked.
### SheetAdded {#SheetAdded}
```
public SheetEventHandler SheetAdded
```
Occurs when user add a worksheet from toolbar menu.
### SheetTabClick {#SheetTabClick}
```
public WorkbookEventHandler SheetTabClick
```
Occurs when the sheet tab is clicked.
### SubmitCommand {#SubmitCommand}
```
public WorkbookEventHandler SubmitCommand
```
Occurs when the "submit" button is clicked.
### UndoCommand {#UndoCommand}
```
public WorkbookEventHandler UndoCommand
```
Occurs when the "undo" button is clicked.
### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```
Calculates the result of formulas.
### createChildControls() {#createChildControls--}
```
public void createChildControls()
```
implment CreateChildControls from WebControl,Internal used only.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |
**Returns:**
boolean
### getACWClientPath() {#getACWClientPath--}
```
public String getACWClientPath()
```
Gets the web path of the script/image files of the control. For example: "http://localhost/acw\_client". You may also set this value in the web.config file. Add this section to the `<configuration>` section:
`<appSettings>`
`<add key="aspose.cells.gridweb.acw_client_path" value="/acw_client/" />`
`</appSettings>`
**Returns:**
java.lang.String
### getACWLanguageFileUrl() {#getACWLanguageFileUrl--}
```
public String getACWLanguageFileUrl()
```
Gets the web url of the language file of the control. For example: "/acw\_client/lang\_en.js".
By default, a built-in english file is used.
**Returns:**
java.lang.String
### getActiveCell() {#getActiveCell--}
```
public GridCell getActiveCell()
```
Gets the active cell of the current sheet. Changed to be writable since version 1.9.0.1.
**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getActiveCellBgColor() {#getActiveCellBgColor--}
```
public Color getActiveCellBgColor()
```
Specifies the background color of the active cell.
**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveCellColor() {#getActiveCellColor--}
```
public Color getActiveCellColor()
```
Specifies the color of the active cell.
**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderBgColor() {#getActiveHeaderBgColor--}
```
public Color getActiveHeaderBgColor()
```
Specifies the background color of the active row/column header.
**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderColor() {#getActiveHeaderColor--}
```
public Color getActiveHeaderColor()
```
Specifies the color of the active row/column header.
**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveSheet() {#getActiveSheet--}
```
public GridWorksheet getActiveSheet()
```
Gets the active sheet
**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```
Gets the active sheet index. Equal to the WebWorksheets.ActiveSheetIndex.
**Returns:**
int
### getActiveTabStyle() {#getActiveTabStyle--}
```
public GridTableItemStyle getActiveTabStyle()
```
Specifies the style of the active tab.
**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getAutoRefreshChart() {#getAutoRefreshChart--}
```
public boolean getAutoRefreshChart()
```
Gets whether the Chart image is updated while updating the cell value.the default is true
**Returns:**
boolean
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```
Gets the BackColor in the WebControl
**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBeanID() {#getBeanID--}
```
public String getBeanID()
```
get the html id of the bean
**Returns:**
java.lang.String
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```
Gets the BorderColor in the WebControl
**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```
Gets the BorderStyle in the WebControl
See [BorderStyle](../../com.aspose.gridweb/borderstyle).
**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```
Gets the BorderWidth in the WebControl
**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomTableStyle() {#getBottomTableStyle--}
```
public GridTableStyle getBottomTableStyle()
```
Gets the style of the bottom bar of the control.
**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getCssClass() {#getCssClass--}
```
public String getCssClass()
```
Gets the CssClass in the WebControl
**Returns:**
java.lang.String
### getCurrentPageIndex() {#getCurrentPageIndex--}
```
public int getCurrentPageIndex()
```
Gets the current page index in paging mode.
**Remarks**
When in paging mode, the control will display PageSize rows of data once, and display the page select control in the tab bar.
**Returns:**
int
### getCustomCalculationEngine() {#getCustomCalculationEngine--}
```
public GridAbstractCalculationEngine getCustomCalculationEngine()
```
Represents user's custom calculation engine to extend the default calculation engine of Aspose.Cells.
**Returns:**
[GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine)
### getCustomCommandButtons() {#getCustomCommandButtons--}
```
public CustomCommandButtonCollection getCustomCommandButtons()
```
Gets the custom command button collection
**Returns:**
[CustomCommandButtonCollection](../../com.aspose.gridweb/customcommandbuttoncollection)
### getCustomStyleFileName() {#getCustomStyleFileName--}
```
public String getCustomStyleFileName()
```
Gets the custom style file name.
**Remarks**
The custom style file is an XML file. When sets the file name, the file will be loaded immediately. Hear is the content of the "standard preset style" ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>
**Example**
```
GridWeb1.setCustomStyleFileName("c:\\style\\mystyle.xml");
```
**Returns:**
java.lang.String
### getDPI() {#getDPI--}
```
public static double getDPI()
```
Gets /Sets the DPI of the machine.
**Remarks**
**Returns:**
double
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```
Gets the control's default font name.
**Example**
```
GridWeb1.setDefaultFontName("Arial");
```
**Returns:**
java.lang.String
### getDefaultFontSize() {#getDefaultFontSize--}
```
public FontUnit getDefaultFontSize()
```
Gets the control's default font size.
**Example**
```
GridWeb1.setDefaultFontSize(new FontUnit("10pt"));
```
**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### getDefaultGridLineColor() {#getDefaultGridLineColor--}
```
public Color getDefaultGridLineColor()
```
Gets the default grid line's color.
**Example**
```
GridWeb1.setDefaultGridLineColor(Color.getRed());
```
**Returns:**
[Color](../../com.aspose.gridweb/color)
### getDisplayCellTip() {#getDisplayCellTip--}
```
public boolean getDisplayCellTip()
```
Gets whether to show tips. the default value is true.
**Returns:**
boolean
### getEditMode() {#getEditMode--}
```
public boolean getEditMode()
```
Gets the control's edit mode.
**Remarks**
When sets to true, the control's cells are editable, and the "save" and the "undo" icon are displayed. When sets to false, the control's cells are readonly, and the "save" and the "undo" icon are not displayed.
**Returns:**
boolean
### getEnableAJAX() {#getEnableAJAX--}
```
public boolean getEnableAJAX()
```
Gets whether to use AJAX call . the default value is true.
**Returns:**
boolean
### getEnableAsync() {#getEnableAsync--}
```
public boolean getEnableAsync()
```
Gets whether load cells data in asynchronous way,suggest to apply for one sheet with more than 10000 cells.
**Returns:**
boolean
### getEnableClientColumnOperations() {#getEnableClientColumnOperations--}
```
public boolean getEnableClientColumnOperations()
```
Gets whether to enable the client side column operations.
**Remarks**
When sets to true, the user can use the right-click menu to add/remove columns.
**Returns:**
boolean
### getEnableClientFreeze() {#getEnableClientFreeze--}
```
public boolean getEnableClientFreeze()
```
Gets whether to enable the client side freezing operations.
**Remarks**
When sets to true, the user can use the right-click menu to freeze/unfreeze panes.
**Returns:**
boolean
### getEnableClientMergeOperations() {#getEnableClientMergeOperations--}
```
public boolean getEnableClientMergeOperations()
```
Gets whether to enable the client side merge operations.
**Remarks**
When sets to true, the user can use the right-click menu to merge/unmerge cells.
**Returns:**
boolean
### getEnableClientResizeColumnRow() {#getEnableClientResizeColumnRow--}
```
public boolean getEnableClientResizeColumnRow()
```
Gets whether to enable the client side resize column and row.
**Remarks**
When sets to true, the user can resize the column and row at client side.
**Returns:**
boolean
### getEnableClientRowOperations() {#getEnableClientRowOperations--}
```
public boolean getEnableClientRowOperations()
```
Gets whether to enable the client side row operations.
**Remarks**
When sets to true, the user can use the right-click menu to add/remove rows.
**Returns:**
boolean
### getEnableDoubleClickEvent() {#getEnableDoubleClickEvent--}
```
public boolean getEnableDoubleClickEvent()
```
Gets whether to enable customer side double-click event.
**Remarks**
When sets to true, the control will receive customer side double-click events and you may handle these events on the server side. Otherwise the control will ignore any double-click events.
**Returns:**
boolean
### getEnableMetalLightEffect() {#getEnableMetalLightEffect--}
```
public boolean getEnableMetalLightEffect()
```
Gets whether to apply metal light effect.
**Returns:**
boolean
### getEnablePaging() {#getEnablePaging--}
```
public boolean getEnablePaging()
```
Gets whether to enable the control's paging mode.
**Remarks**
When sets to true, the control will display PageSize rows of data once, and display the page select control in the tab bar.
**Returns:**
boolean
### getEnableStyleDialogbox() {#getEnableStyleDialogbox--}
```
public boolean getEnableStyleDialogbox()
```
Gets whether to enable the client side style dialogbox.
**Remarks**
When sets to true, the user can use the style dialogbox to set a cell's style by selecting the "Format Cell..." from the popup menu.
**Returns:**
boolean
### getEnabled() {#getEnabled--}
```
public boolean getEnabled()
```
Gets the Enabled in the WebControl
**Returns:**
boolean
### getFilteredPaging() {#getFilteredPaging--}
```
public boolean getFilteredPaging()
```
Gets whether to enable the paging after data filtered,will take affect when EnablePaging is true.
**Remarks**
When sets to true, the control will paging based on filtered data,the default value is false.
**Returns:**
boolean
### getFont() {#getFont--}
```
public FontInfo getFont()
```
Gets the Font in the WebControl
**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForceValidation() {#getForceValidation--}
```
public boolean getForceValidation()
```
Gets whether to force customer side validation.
**Remarks**
When sets to true, data will not post to server until all input fields are valid.
**Returns:**
boolean
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```
Gets the ForeColor in the WebControl
**Returns:**
[Color](../../com.aspose.gridweb/color)
### getFrameTableStyle() {#getFrameTableStyle--}
```
public GridTableStyle getFrameTableStyle()
```
Gets the frame style of the control.
**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getGoonDefaultSaveOperation() {#getGoonDefaultSaveOperation--}
```
public boolean getGoonDefaultSaveOperation()
```
Gets whether GridWeb will do the default save operation ,the default value is true.
**Returns:**
boolean
### getHTMLBody() {#getHTMLBody--}
```
public String getHTMLBody()
```
the html code of the bean for html body, it shall be get after call of method init and prepareRender
**Returns:**
java.lang.String
### getHTMLHead() {#getHTMLHead--}
```
public String getHTMLHead()
```
the html code of the bean for html head, it shall be get after call of method init and prepareRender
**Returns:**
java.lang.String
### getHeaderBarHeight() {#getHeaderBarHeight--}
```
public Unit getHeaderBarHeight()
```
Gets the height( System.Web.UI.WebControl.Unit ) of the top header bar of the control.
**Example**
```
GridWeb1.setHeaderBarWidth(new Unit(32, com.aspose.gridweb.UnitType.Point));
GridWeb1.setHeaderBarHeight(new Unit(24, com.aspose.gridweb.UnitType.Point));
```
**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHeaderBarStyle() {#getHeaderBarStyle--}
```
public GridTableItemStyle getHeaderBarStyle()
```
Gets the header bar's style.
**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getHeaderBarTableStyle() {#getHeaderBarTableStyle--}
```
public GridTableStyle getHeaderBarTableStyle()
```
Gets the header bar style of the control.
**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getHeaderBarWidth() {#getHeaderBarWidth--}
```
public Unit getHeaderBarWidth()
```
Gets the width( System.Web.UI.WebControl.Unit ) or the left header bar of the control.
**Example**
```
GridWeb1.setHeaderBarWidth(new Unit(32, com.aspose.gridweb.UnitType.Point));
GridWeb1.setHeaderBarHeight(new Unit(24, com.aspose.gridweb.UnitType.Point));
```
**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHeight() {#getHeight--}
```
public Unit getHeight()
```
Gets the height( System.Web.UI.WebControl.Unit ) of the control.
**Example**
```
GridWeb1.setWidth(new Unit(320, com.aspose.gridweb.UnitType.Point));
GridWeb1.setHeight(new Unit(240, com.aspose.gridweb.UnitType.Point));
```
**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getIgnoreStyleWithNoData() {#getIgnoreStyleWithNoData--}
```
public boolean getIgnoreStyleWithNoData()
```
Gets whether GridWeb ignores showing rows or columns that do not contain cell values but are still styled. If set to true, the performance will be better. The default value is false, which means that if the last consecutive row/column has no cell values but is styled, we will still display them. This option is only valid when EnableAsync is false. This option has no effect when EnableAsync is true, which means GridWeb will show all rows/columns with style.
**Returns:**
boolean
### getLoadOptions() {#getLoadOptions--}
```
public GridLoadOptions getLoadOptions()
```
Represents the loadoptions for GridWeb.
**Returns:**
[GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```
Gets the maximum display column index(zero based) of the web sheet. The control uses the greater value of MaxColumn and sheet data's max column.
**Example**
```
// Creates a 4x4 "display window".
GridWeb1.setMinRow(2);
GridWeb1.setMaxRow(5);
GridWeb1.setMinColumn(3);
GridWeb1.setMaxColumn(6);
```
**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```
Gets the maximum display row index(zero based) of the web sheet. The control uses the greater value of MaxRow and sheet data's max row.
**Example**
```
// Creates a 4x4 "display window".
GridWeb1.setMinRow(2);
GridWeb1.setMaxRow(5);
GridWeb1.setMinColumn(3);
GridWeb1.setMaxColumn(6);
```
**Returns:**
int
### getMessage() {#getMessage--}
```
public String getMessage()
```
Gets the message for the grid.
**Returns:**
java.lang.String
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```
Gets the minimum display column index(zero based) of the web sheet. The control uses the smaller value of MinColumn and sheet data's min column.
**Example**
```
// Creates a 4x4 "display window".
GridWeb1.setMinRow(2);
GridWeb1.setMaxRow(5);
GridWeb1.setMinColumn(3);
GridWeb1.setMaxColumn(6);
```
**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```
Gets the minimum display row index(zero based) of the web sheet. The control uses the smaller value of MinRow and sheet data's min row.
**Example**
```
// Creates a 4x4 "display window".
GridWeb1.setMinRow(2);
GridWeb1.setMaxRow(5);
GridWeb1.setMinColumn(3);
GridWeb1.setMaxColumn(6);
```
**Returns:**
int
### getModifiedCells() {#getModifiedCells--}
```
public ArrayList getModifiedCells()
```
Gets the collection of the cells that modified by the client.
**Returns:**
java.util.ArrayList
### getNeedRenderGroupRows() {#getNeedRenderGroupRows--}
```
public boolean getNeedRenderGroupRows()
```
Gets whether to show grouprows .
**Returns:**
boolean
### getNoHScroll() {#getNoHScroll--}
```
public boolean getNoHScroll()
```
Gets a value indicating whether the horizontal scroll bar is hidden.
**Returns:**
boolean
### getNoScroll() {#getNoScroll--}
```
public boolean getNoScroll()
```
Gets whether to show scroll bar .
**Returns:**
boolean
### getNoVScroll() {#getNoVScroll--}
```
public boolean getNoVScroll()
```
Gets a value indicating whether the vertical scroll bar is hidden.
**Returns:**
boolean
### getOnAjaxCallFinishedClientFunction() {#getOnAjaxCallFinishedClientFunction--}
```
public String getOnAjaxCallFinishedClientFunction()
```
Gets the client side function name to be called when ajaxcall finished. The client function should be declared like this:
function GridAjaxcallFinished()
\{
alert(this.id+" ajaxcall finished ");
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Returns:**
java.lang.String
### getOnCellErrorClientFunction() {#getOnCellErrorClientFunction--}
```
public String getOnCellErrorClientFunction()
```
Gets the client side function name to be called when a cell's validation is failed. The client function should be declared like this:
function MyOnCellError(cell)
\{
alert(this.getCellValueByCell(cell));
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Returns:**
java.lang.String
### getOnCellSelectedAjaxCallBackClientFunction() {#getOnCellSelectedAjaxCallBackClientFunction--}
```
public String getOnCellSelectedAjaxCallBackClientFunction()
```
Gets the client side function to be called when a cell is selected. The client function should be declared like this:
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\{
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Returns:**
java.lang.String
### getOnCellSelectedClientFunction() {#getOnCellSelectedClientFunction--}
```
public String getOnCellSelectedClientFunction()
```
Gets the client side function to be called when a cell is selected. The client function should be declared like this:
function MyOnSelectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, "test");
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Returns:**
java.lang.String
### getOnCellUnselectedClientFunction() {#getOnCellUnselectedClientFunction--}
```
public String getOnCellUnselectedClientFunction()
```
Gets the client side function to be called when a cell is unselected. The client function should be declared like this:
function MyOnUnselectCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Returns:**
java.lang.String
### getOnCellUpdatedClientFunction() {#getOnCellUpdatedClientFunction--}
```
public String getOnCellUpdatedClientFunction()
```
Gets the client side function name to be called when a cell's value is updated. The client function should be declared like this:
function MyOnCellUpdated(cell)
\{
alert(this.getCellValueByCell(cell));
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Returns:**
java.lang.String
### getOnContextMenuShowClientFunction() {#getOnContextMenuShowClientFunction--}
```
public String getOnContextMenuShowClientFunction()
```
Gets the client side function to be called when the context menu will be shown. The client function should be declared like this:
function onContextMenuShow()
\{
var menu = event.srcElement;
menu.setItemVisibility("Delete", "block");
menu.setItemVisibility("Update", "none");
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Returns:**
java.lang.String
### getOnDoubleClickCellClientFunction() {#getOnDoubleClickCellClientFunction--}
```
public String getOnDoubleClickCellClientFunction()
```
Gets the client side function to be called when a cell is double clicked. The client function should be declared like this:
function MyOnDoubleClickCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Returns:**
java.lang.String
### getOnDoubleClickRowClientFunction() {#getOnDoubleClickRowClientFunction--}
```
public String getOnDoubleClickRowClientFunction()
```
Gets the client side function to be called when a row is double clicked. The client function should be declared like this:
function MyOnRowDoubleClick(row)
\{
alert(row);
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Returns:**
java.lang.String
### getOnGridInitClientFunction() {#getOnGridInitClientFunction--}
```
public String getOnGridInitClientFunction()
```
Gets the client side function name to be called when the grid is initialized. The client function should be declared like this:
function MyOnGridInit(grid)
\{
alert("The grid is initialized: " + grid.id);
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Returns:**
java.lang.String
### getOnPageChangeClientFunction() {#getOnPageChangeClientFunction--}
```
public String getOnPageChangeClientFunction()
```
Gets the client side function to be called after page index changing.only take effect when EnablePaging is true. The client function should be declared like this:
function MyOnPageChange(index)
\{
console.log("current page is:"+index);
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Returns:**
java.lang.String
### getOnPageSubmitClientFunction() {#getOnPageSubmitClientFunction--}
```
public String getOnPageSubmitClientFunction()
```
Gets the client function to be called before the page is submitted at client side.
**Returns:**
java.lang.String
### getOnShapeSelectedClientFunction() {#getOnShapeSelectedClientFunction--}
```
public String getOnShapeSelectedClientFunction()
```
Gets the client side function to be called when a shape is selected. The client function should be declared like this:
function MyOnSelectShape(shape)
\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Returns:**
java.lang.String
### getOnSubmitClientFunction() {#getOnSubmitClientFunction--}
```
public String getOnSubmitClientFunction()
```
Gets the client function to be called before the control is submitted at client side. The client function should be declared like this:
function MyOnSubmit(arg, cancelEdit)
\{
return true;
\}
The arg is the submit argument, contains the command to be post to the server. The cancelEdit is boolean value indicates whether the control has discarded the user input before submit. The control will continue submitting if the function returns true.
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Returns:**
java.lang.String
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```
Gets whether only fit the rows which height are not customed,the default value is false
**Returns:**
boolean
### getPageSize() {#getPageSize--}
```
public int getPageSize()
```
Gets the page size in paging mode.
**Remarks**
When in paging mode, the control will display PageSize rows of data once, and display the page select control in the tab bar.
**Returns:**
int
### getPictureCachePath() {#getPictureCachePath--}
```
public static String getPictureCachePath()
```
Gets the image storage path for the workbook,all the shapes,images will be stored in this directory, the default path is acwcache under current application Base Directory users need to implement a schedule service to clean the files those are out of session time.
**Returns:**
java.lang.String
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```
Gets the preset style.
See [PresetStyle](../../com.aspose.gridweb/presetstyle).
**Example**
```
GridWeb1.setPresetStyle(PresetStyle.TRADITIONAL_1);
```
**Returns:**
int
### getRefreshValidation() {#getRefreshValidation--}
```
public boolean getRefreshValidation()
```
Gets whether to refresh validation value after cell value changes.
**Returns:**
boolean
### getRenderHiddenRow() {#getRenderHiddenRow--}
```
public boolean getRenderHiddenRow()
```
Gets whether the hidden row is rendered in GridControl,the default value is false. if you need to unhide the hidden row latter ,you shall set it as true
**Returns:**
boolean
### getRowHeightForCSV() {#getRowHeightForCSV--}
```
public double getRowHeightForCSV()
```
Gets the row height value in point for csv file ,default value is 14.5.
**Returns:**
double
### getScrollBarArrowColor() {#getScrollBarArrowColor--}
```
public Color getScrollBarArrowColor()
```
Specifies the color of the scrollbar's arrow button.
**Returns:**
[Color](../../com.aspose.gridweb/color)
### getScrollBarBaseColor() {#getScrollBarBaseColor--}
```
public Color getScrollBarBaseColor()
```
Specifies the color of the scroll bar of the control.
**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellBgColor() {#getSelectCellBgColor--}
```
public Color getSelectCellBgColor()
```
Specifies the background color of the selected cells in multi-select range.
**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellColor() {#getSelectCellColor--}
```
public Color getSelectCellColor()
```
Specifies the color of the selected cells in multi-select range.
**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSessionStorePath() {#getSessionStorePath--}
```
public String getSessionStorePath()
```
Gets the session cache store path when session mode is File or ViewState, etc: gridweb.SessionStorePath="c:/mytempdir/session"; then it will store session data in c:/mytempdir/session
**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```
Represents the workbook settings.
**Returns:**
[GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings)
### getShowAddButton() {#getShowAddButton--}
```
public boolean getShowAddButton()
```
Gets whether to show the add worksheet button.
**Returns:**
boolean
### getShowBottomBar() {#getShowBottomBar--}
```
public boolean getShowBottomBar()
```
Specifies whether to show the command bar(includes command bar and tab bar) at the bottom of the control.
**Returns:**
boolean
### getShowCellEditBox() {#getShowCellEditBox--}
```
public boolean getShowCellEditBox()
```
whether Gridweb shows edit box toolbar as in MS-EXCEL.if enable ,a edit box for current cell will display in Gridweb. if we enable this feature, we need to import jquery js library in your aspx files to support this new feature. all the latest jquery version is ok. etc.
**Returns:**
boolean
### getShowCommandBarAtTop() {#getShowCommandBarAtTop--}
```
public boolean getShowCommandBarAtTop()
```
Specifies whether to show the command bar(includes command bar and tab bar) at the top of the control.
**Returns:**
boolean
### getShowContextMenu() {#getShowContextMenu--}
```
public boolean getShowContextMenu()
```
Gets whether to show the context menu. the default value is true.
**Returns:**
boolean
### getShowDefaultGridLine() {#getShowDefaultGridLine--}
```
public boolean getShowDefaultGridLine()
```
Gets whether to show the default grid lines of the cells.
**Returns:**
boolean
### getShowHeaderBar() {#getShowHeaderBar--}
```
public boolean getShowHeaderBar()
```
Gets whether to show header bar
**Returns:**
boolean
### getShowLoading() {#getShowLoading--}
```
public boolean getShowLoading()
```
Specifies whether to show a loading dialogbox while postbacking to server.
**Returns:**
boolean
### getShowLoadingPosition() {#getShowLoadingPosition--}
```
public String getShowLoadingPosition()
```
Specifies the left,top postion(in px) to show the loading dialogbox while postbacking to server ,etc. 100,200 means the loading dialogbox's left,top postion is at 100px,200px .
**Returns:**
java.lang.String
### getShowSaveButton() {#getShowSaveButton--}
```
public boolean getShowSaveButton()
```
Gets whether to show the save button.
**Returns:**
boolean
### getShowSubmitButton() {#getShowSubmitButton--}
```
public boolean getShowSubmitButton()
```
Gets whether to show the submit button.
**Returns:**
boolean
### getShowTabBar() {#getShowTabBar--}
```
public boolean getShowTabBar()
```
Gets whether to show the tab bar.
**Returns:**
boolean
### getShowTabNavigation() {#getShowTabNavigation--}
```
public boolean getShowTabNavigation()
```
Gets whether the tab navigation button is show,the default value is true.
**Returns:**
boolean
### getShowUndoButton() {#getShowUndoButton--}
```
public boolean getShowUndoButton()
```
Gets whether to show the undo button.
**Returns:**
boolean
### getSpanWrap() {#getSpanWrap--}
```
public boolean getSpanWrap()
```
Specifies whether to wrap content in the cell span.the default value is true.
**Returns:**
boolean
### getTabIndex() {#getTabIndex--}
```
public short getTabIndex()
```
Gets the TabIndex in the WebControl
**Returns:**
short
### getTabStyle() {#getTabStyle--}
```
public GridTableItemStyle getTabStyle()
```
Gets the style of the tab bar.
**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```
Gets the ToolTip in the WebControl
**Returns:**
java.lang.String
### getUseClientPageHeight() {#getUseClientPageHeight--}
```
public boolean getUseClientPageHeight()
```
Gets whether gridweb use client page height as control height ,suitable for when set Height="100%",default value is false
**Returns:**
boolean
### getViewPanelScrollLeft() {#getViewPanelScrollLeft--}
```
public String getViewPanelScrollLeft()
```
Gets the position of the scroll bar of the grid's view panel.
**Returns:**
java.lang.String
### getViewPanelScrollTop() {#getViewPanelScrollTop--}
```
public String getViewPanelScrollTop()
```
Gets the position of the scroll bar of the grid's view panel.
**Returns:**
java.lang.String
### getViewTableStyle() {#getViewTableStyle--}
```
public GridTableStyle getViewTableStyle()
```
Gets the data view panel's style.
**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getWidth() {#getWidth--}
```
public Unit getWidth()
```
Gets the width( System.Web.UI.WebControl.Unit ) of the control.
**Example**
```
GridWeb1.setWidth(new Unit(320, com.aspose.gridweb.UnitType.Point));
GridWeb1.setHeight(new Unit(240, com.aspose.gridweb.UnitType.Point));
```
**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getWorkSheets() {#getWorkSheets--}
```
public GridWorksheetCollection getWorkSheets()
```
Gets the collection of the worksheets.
**Returns:**
[GridWorksheetCollection](../../com.aspose.gridweb/gridworksheetcollection)
### getXhtmlMode() {#getXhtmlMode--}
```
public boolean getXhtmlMode()
```
Gets whether to use XHTML style,the default value is true.
**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### importExcelFile(InputStream stream) {#importExcelFile-java.io.InputStream-}
```
public void importExcelFile(InputStream stream)
```
Imports from an excel file stream, including disk file stream or memory stream.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The excel file's stream, including disk file stream or memory stream. |
### importExcelFile(InputStream stream, String passwordtoOpen) {#importExcelFile-java.io.InputStream-java.lang.String-}
```
public void importExcelFile(InputStream stream, String passwordtoOpen)
```
Imports from an excel file stream, including disk file stream or memory stream.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The excel file's stream, including disk file stream or memory stream. |
| passwordtoOpen | java.lang.String | the open password for the file which is encrypted . |
### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```
Imports from an excel file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The excel file's name. |
### importExcelFile(String fileName, String passwordtoOpen) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String fileName, String passwordtoOpen)
```
Imports from an excel file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The excel file's name. |
| passwordtoOpen | java.lang.String | the open password for the file which is encrypted . |
### init() {#init--}
```
public void init()
```
the bean shall be initialized by the servlet request and response of the current page
### isCalculateFormula() {#isCalculateFormula--}
```
public boolean isCalculateFormula()
```
Gets whether to calculate formula after cell value changes or after import File. The default value is true.
**Returns:**
boolean
### loadCSVFile(InputStream stream) {#loadCSVFile-java.io.InputStream-}
```
public void loadCSVFile(InputStream stream)
```
Loads data from a CSV file stream.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The file stream. |
### loadCSVFile(String fileName) {#loadCSVFile-java.lang.String-}
```
public void loadCSVFile(String fileName)
```
Loads data from a CSV file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file's name. |
### loadHTMLFile(InputStream stream) {#loadHTMLFile-java.io.InputStream-}
```
public void loadHTMLFile(InputStream stream)
```
Loads data from a HTML file stream.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The file stream. |
### loadHTMLFile(String fileName) {#loadHTMLFile-java.lang.String-}
```
public void loadHTMLFile(String fileName)
```
Loads data from a HTML file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file's name. |
### loadSpreadSheetMLFile(InputStream stream) {#loadSpreadSheetMLFile-java.io.InputStream-}
```
public void loadSpreadSheetMLFile(InputStream stream)
```
Loads data from a SpreadSheetML file stream.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The file's stream. |
### loadSpreadSheetMLFile(String fileName) {#loadSpreadSheetMLFile-java.lang.String-}
```
public void loadSpreadSheetMLFile(String fileName)
```
Loads data from a SpreadSheetML file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file's name. |
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### prepareRender() {#prepareRender--}
```
public void prepareRender()
```
the method shall be called before render GridWeb bean
### refreshChartShape() {#refreshChartShape--}
```
public void refreshChartShape()
```
refresh all the chart image for the active worksheet .
### saveCSVFile(OutputStream stream) {#saveCSVFile-java.io.OutputStream-}
```
public void saveCSVFile(OutputStream stream)
```
Saves data to a CSV file stream.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The file stream. |
### saveCSVFile(String targetFile) {#saveCSVFile-java.lang.String-}
```
public void saveCSVFile(String targetFile)
```
Saves data to a CSV file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| targetFile | java.lang.String | The file's name. |
### saveCustomStyleFile(String fileName) {#saveCustomStyleFile-java.lang.String-}
```
public void saveCustomStyleFile(String fileName)
```
Saves current style data of the control to an xml file. Can be used to create your customized style file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The style file's name. |
### saveHTMLFile(OutputStream stream) {#saveHTMLFile-java.io.OutputStream-}
```
public void saveHTMLFile(OutputStream stream)
```
Saves data to a HTML file stream.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The file stream. |
### saveHTMLFile(String targetFile) {#saveHTMLFile-java.lang.String-}
```
public void saveHTMLFile(String targetFile)
```
Saves data to a HTML file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| targetFile | java.lang.String | The file's name. |
### saveSpreadSheetMLFile(OutputStream stream) {#saveSpreadSheetMLFile-java.io.OutputStream-}
```
public void saveSpreadSheetMLFile(OutputStream stream)
```
Saves data to a SpreadSheetML file stream.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The file stream. |
### saveSpreadSheetMLFile(String targetFile) {#saveSpreadSheetMLFile-java.lang.String-}
```
public void saveSpreadSheetMLFile(String targetFile)
```
Saves data to a SpreadSheetML file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| targetFile | java.lang.String | The file's name. |
### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```
Saves the worksheets to an excel file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream to write to. |
### saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions) {#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)
```
Saves the worksheets to an excel file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream to write to. |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | The save options. |
### saveToExcelFile(OutputStream stream, int format) {#saveToExcelFile-java.io.OutputStream-int-}
```
public void saveToExcelFile(OutputStream stream, int format)
```
Saves the worksheets to an excel file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream to write to. |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). The file format(Excel2003, Excel2007, CSV, SpreadsheetML) |
### saveToExcelFile(String targetFile) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String targetFile)
```
Saves the worksheets to an excel file with Excel 2003 format.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| targetFile | java.lang.String | The name of the target file to write to. |
### saveToExcelFile(String targetFile, GridSaveOptions saveOptions) {#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(String targetFile, GridSaveOptions saveOptions)
```
Saves the worksheets to an excel file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| targetFile | java.lang.String | The name of the target file to write to. |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | The save options. |
### saveToExcelFile(String targetFile, int format) {#saveToExcelFile-java.lang.String-int-}
```
public void saveToExcelFile(String targetFile, int format)
```
Saves the worksheets to an excel file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| targetFile | java.lang.String | The name of the target file to write to. |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). The file format(Excel2003, Excel2007, CSV, SpreadsheetML) |
### setACWClientPath(String value) {#setACWClientPath-java.lang.String-}
```
public void setACWClientPath(String value)
```
Sets the web path of the script/image files of the control. For example: "http://localhost/acw\_client". You may also set this value in the web.config file. Add this section to the `<configuration>` section:
`<appSettings>`
`<add key="aspose.cells.gridweb.acw_client_path" value="/acw_client/" />`
`</appSettings>`
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setACWLanguageFileUrl(String value) {#setACWLanguageFileUrl-java.lang.String-}
```
public void setACWLanguageFileUrl(String value)
```
Sets the web url of the language file of the control. For example: "/acw\_client/lang\_en.js".
By default, a built-in english file is used.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setActiveCell(GridCell value) {#setActiveCell-com.aspose.gridweb.GridCell-}
```
public void setActiveCell(GridCell value)
```
Sets the active cell of the current sheet. Changed to be writable since version 1.9.0.1.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |
### setActiveCellBgColor(Color value) {#setActiveCellBgColor-com.aspose.gridweb.Color-}
```
public void setActiveCellBgColor(Color value)
```
Specifies the background color of the active cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |
### setActiveCellColor(Color value) {#setActiveCellColor-com.aspose.gridweb.Color-}
```
public void setActiveCellColor(Color value)
```
Specifies the color of the active cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |
### setActiveHeaderBgColor(Color value) {#setActiveHeaderBgColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderBgColor(Color value)
```
Specifies the background color of the active row/column header.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |
### setActiveHeaderColor(Color value) {#setActiveHeaderColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderColor(Color value)
```
Specifies the color of the active row/column header.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |
### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```
Sets the active sheet index. Equal to the WebWorksheets.ActiveSheetIndex.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setActiveTabStyle(GridTableItemStyle value) {#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setActiveTabStyle(GridTableItemStyle value)
```
Specifies the style of the active tab.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |
### setAutoRefreshChart(boolean value) {#setAutoRefreshChart-boolean-}
```
public void setAutoRefreshChart(boolean value)
```
Sets whether the Chart image is updated while updating the cell value.the default is true
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setBackColor(Color value) {#setBackColor-com.aspose.gridweb.Color-}
```
public void setBackColor(Color value)
```
Sets the BackColor in the WebControl
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |
### setBeanID(String beanID) {#setBeanID-java.lang.String-}
```
public void setBeanID(String beanID)
```
set the html id of the bean
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| beanID | java.lang.String |  |
### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```
Sets the BorderColor in the WebControl
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |
### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```
Sets the BorderStyle in the WebControl
See [BorderStyle](../../com.aspose.gridweb/borderstyle).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```
Sets the BorderWidth in the WebControl
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |
### setBottomTableStyle(GridTableStyle value) {#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setBottomTableStyle(GridTableStyle value)
```
Sets the style of the bottom bar of the control.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |
### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```
Sets whether to calculate formula after cell value changes or after import File. The default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```
Sets the CssClass in the WebControl
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setCurrentPageIndex(int value) {#setCurrentPageIndex-int-}
```
public void setCurrentPageIndex(int value)
```
Sets the current page index in paging mode.
**Remarks**
When in paging mode, the control will display PageSize rows of data once, and display the page select control in the tab bar.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setCustomCalculationEngine(GridAbstractCalculationEngine value) {#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-}
```
public void setCustomCalculationEngine(GridAbstractCalculationEngine value)
```
Represents user's custom calculation engine to extend the default calculation engine of Aspose.Cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine) |  |
### setCustomStyle(InputStream stream) {#setCustomStyle-java.io.InputStream-}
```
public void setCustomStyle(InputStream stream)
```
sets the custom style file from stream including disk file stream or memory stream.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The file's stream, including disk file stream or memory stream. |
### setCustomStyleFileName(String value) {#setCustomStyleFileName-java.lang.String-}
```
public void setCustomStyleFileName(String value)
```
Sets the custom style file name.
**Remarks**
The custom style file is an XML file. When sets the file name, the file will be loaded immediately. Hear is the content of the "standard preset style" ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```
Gets /Sets the DPI of the machine.
**Remarks**
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```
Sets the control's default font name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```
Sets the control's default font size.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |
### setDefaultGridLineColor(Color value) {#setDefaultGridLineColor-com.aspose.gridweb.Color-}
```
public void setDefaultGridLineColor(Color value)
```
Sets the default grid line's color.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |
### setDisplayCellTip(boolean value) {#setDisplayCellTip-boolean-}
```
public void setDisplayCellTip(boolean value)
```
Sets whether to show tips. the default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEditMode(boolean value) {#setEditMode-boolean-}
```
public void setEditMode(boolean value)
```
Sets the control's edit mode.
**Remarks**
When sets to true, the control's cells are editable, and the "save" and the "undo" icon are displayed. When sets to false, the control's cells are readonly, and the "save" and the "undo" icon are not displayed.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEnableAJAX(boolean value) {#setEnableAJAX-boolean-}
```
public void setEnableAJAX(boolean value)
```
Sets whether to use AJAX call . the default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEnableAsync(boolean value) {#setEnableAsync-boolean-}
```
public void setEnableAsync(boolean value)
```
Sets whether load cells data in asynchronous way,suggest to apply for one sheet with more than 10000 cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEnableClientColumnOperations(boolean value) {#setEnableClientColumnOperations-boolean-}
```
public void setEnableClientColumnOperations(boolean value)
```
Sets whether to enable the client side column operations.
**Remarks**
When sets to true, the user can use the right-click menu to add/remove columns.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEnableClientFreeze(boolean value) {#setEnableClientFreeze-boolean-}
```
public void setEnableClientFreeze(boolean value)
```
Sets whether to enable the client side freezing operations.
**Remarks**
When sets to true, the user can use the right-click menu to freeze/unfreeze panes.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEnableClientMergeOperations(boolean value) {#setEnableClientMergeOperations-boolean-}
```
public void setEnableClientMergeOperations(boolean value)
```
Sets whether to enable the client side merge operations.
**Remarks**
When sets to true, the user can use the right-click menu to merge/unmerge cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEnableClientResizeColumnRow(boolean value) {#setEnableClientResizeColumnRow-boolean-}
```
public void setEnableClientResizeColumnRow(boolean value)
```
Sets whether to enable the client side resize column and row.
**Remarks**
When sets to true, the user can resize the column and row at client side.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEnableClientRowOperations(boolean value) {#setEnableClientRowOperations-boolean-}
```
public void setEnableClientRowOperations(boolean value)
```
Sets whether to enable the client side row operations.
**Remarks**
When sets to true, the user can use the right-click menu to add/remove rows.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEnableDoubleClickEvent(boolean value) {#setEnableDoubleClickEvent-boolean-}
```
public void setEnableDoubleClickEvent(boolean value)
```
Sets whether to enable customer side double-click event.
**Remarks**
When sets to true, the control will receive customer side double-click events and you may handle these events on the server side. Otherwise the control will ignore any double-click events.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEnableMetalLightEffect(boolean value) {#setEnableMetalLightEffect-boolean-}
```
public void setEnableMetalLightEffect(boolean value)
```
Sets whether to apply metal light effect.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEnablePaging(boolean value) {#setEnablePaging-boolean-}
```
public void setEnablePaging(boolean value)
```
Sets whether to enable the control's paging mode.
**Remarks**
When sets to true, the control will display PageSize rows of data once, and display the page select control in the tab bar.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEnableStyleDialogbox(boolean value) {#setEnableStyleDialogbox-boolean-}
```
public void setEnableStyleDialogbox(boolean value)
```
Sets whether to enable the client side style dialogbox.
**Remarks**
When sets to true, the user can use the style dialogbox to set a cell's style by selecting the "Format Cell..." from the popup menu.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```
Sets the Enabled in the WebControl
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setFilteredPaging(boolean value) {#setFilteredPaging-boolean-}
```
public void setFilteredPaging(boolean value)
```
Sets whether to enable the paging after data filtered,will take affect when EnablePaging is true.
**Remarks**
When sets to true, the control will paging based on filtered data,the default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setForceValidation(boolean value) {#setForceValidation-boolean-}
```
public void setForceValidation(boolean value)
```
Sets whether to force customer side validation.
**Remarks**
When sets to true, data will not post to server until all input fields are valid.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```
Sets the ForeColor in the WebControl
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |
### setFrameTableStyle(GridTableStyle value) {#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setFrameTableStyle(GridTableStyle value)
```
Sets the frame style of the control.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |
### setGoonDefaultSaveOperation(boolean value) {#setGoonDefaultSaveOperation-boolean-}
```
public void setGoonDefaultSaveOperation(boolean value)
```
Sets whether GridWeb will do the default save operation ,the default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setHeaderBarHeight(Unit value) {#setHeaderBarHeight-com.aspose.gridweb.Unit-}
```
public void setHeaderBarHeight(Unit value)
```
Sets the height( System.Web.UI.WebControl.Unit ) of the top header bar of the control.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |
### setHeaderBarStyle(GridTableItemStyle value) {#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setHeaderBarStyle(GridTableItemStyle value)
```
Sets the header bar's style.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |
### setHeaderBarTableStyle(GridTableStyle value) {#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setHeaderBarTableStyle(GridTableStyle value)
```
Sets the header bar style of the control.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |
### setHeaderBarWidth(Unit value) {#setHeaderBarWidth-com.aspose.gridweb.Unit-}
```
public void setHeaderBarWidth(Unit value)
```
Sets the width( System.Web.UI.WebControl.Unit ) or the left header bar of the control.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |
### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```
Sets the height( System.Web.UI.WebControl.Unit ) of the control.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |
### setIgnoreStyleWithNoData(boolean value) {#setIgnoreStyleWithNoData-boolean-}
```
public void setIgnoreStyleWithNoData(boolean value)
```
Sets whether GridWeb ignores showing rows or columns that do not contain cell values but are still styled. If set to true, the performance will be better. The default value is false, which means that if the last consecutive row/column has no cell values but is styled, we will still display them. This option is only valid when EnableAsync is false. This option has no effect when EnableAsync is true, which means GridWeb will show all rows/columns with style.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setLoadOptions(GridLoadOptions value) {#setLoadOptions-com.aspose.gridweb.GridLoadOptions-}
```
public void setLoadOptions(GridLoadOptions value)
```
Represents the loadoptions for GridWeb.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridLoadOptions](../../com.aspose.gridweb/gridloadoptions) |  |
### setMaxColumn(int value) {#setMaxColumn-int-}
```
public void setMaxColumn(int value)
```
Sets the maximum display column index(zero based) of the web sheet. The control uses the greater value of MaxColumn and sheet data's max column.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setMaxRow(int value) {#setMaxRow-int-}
```
public void setMaxRow(int value)
```
Sets the maximum display row index(zero based) of the web sheet. The control uses the greater value of MaxRow and sheet data's max row.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setMessage(String value) {#setMessage-java.lang.String-}
```
public void setMessage(String value)
```
Sets the message for the grid.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setMinColumn(int value) {#setMinColumn-int-}
```
public void setMinColumn(int value)
```
Sets the minimum display column index(zero based) of the web sheet. The control uses the smaller value of MinColumn and sheet data's min column.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setMinRow(int value) {#setMinRow-int-}
```
public void setMinRow(int value)
```
Sets the minimum display row index(zero based) of the web sheet. The control uses the smaller value of MinRow and sheet data's min row.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setNeedRenderGroupRows(boolean value) {#setNeedRenderGroupRows-boolean-}
```
public void setNeedRenderGroupRows(boolean value)
```
Sets whether to show grouprows .
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setNoHScroll(boolean value) {#setNoHScroll-boolean-}
```
public void setNoHScroll(boolean value)
```
Sets a value indicating whether the horizontal scroll bar is hidden.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setNoScroll(boolean value) {#setNoScroll-boolean-}
```
public void setNoScroll(boolean value)
```
Sets whether to show scroll bar .
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setNoVScroll(boolean value) {#setNoVScroll-boolean-}
```
public void setNoVScroll(boolean value)
```
Sets a value indicating whether the vertical scroll bar is hidden.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setOnAjaxCallFinishedClientFunction(String value) {#setOnAjaxCallFinishedClientFunction-java.lang.String-}
```
public void setOnAjaxCallFinishedClientFunction(String value)
```
Sets the client side function name to be called when ajaxcall finished. The client function should be declared like this:
function GridAjaxcallFinished()
\{
alert(this.id+" ajaxcall finished ");
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOnCellErrorClientFunction(String value) {#setOnCellErrorClientFunction-java.lang.String-}
```
public void setOnCellErrorClientFunction(String value)
```
Sets the client side function name to be called when a cell's validation is failed. The client function should be declared like this:
function MyOnCellError(cell)
\{
alert(this.getCellValueByCell(cell));
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOnCellSelectedAjaxCallBackClientFunction(String value) {#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-}
```
public void setOnCellSelectedAjaxCallBackClientFunction(String value)
```
Sets the client side function to be called when a cell is selected. The client function should be declared like this:
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\{
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOnCellSelectedClientFunction(String value) {#setOnCellSelectedClientFunction-java.lang.String-}
```
public void setOnCellSelectedClientFunction(String value)
```
Sets the client side function to be called when a cell is selected. The client function should be declared like this:
function MyOnSelectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, "test");
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOnCellUnselectedClientFunction(String value) {#setOnCellUnselectedClientFunction-java.lang.String-}
```
public void setOnCellUnselectedClientFunction(String value)
```
Sets the client side function to be called when a cell is unselected. The client function should be declared like this:
function MyOnUnselectCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOnCellUpdatedClientFunction(String value) {#setOnCellUpdatedClientFunction-java.lang.String-}
```
public void setOnCellUpdatedClientFunction(String value)
```
Sets the client side function name to be called when a cell's value is updated. The client function should be declared like this:
function MyOnCellUpdated(cell)
\{
alert(this.getCellValueByCell(cell));
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOnContextMenuShowClientFunction(String value) {#setOnContextMenuShowClientFunction-java.lang.String-}
```
public void setOnContextMenuShowClientFunction(String value)
```
Sets the client side function to be called when the context menu will be shown. The client function should be declared like this:
function onContextMenuShow()
\{
var menu = event.srcElement;
menu.setItemVisibility("Delete", "block");
menu.setItemVisibility("Update", "none");
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOnDoubleClickCellClientFunction(String value) {#setOnDoubleClickCellClientFunction-java.lang.String-}
```
public void setOnDoubleClickCellClientFunction(String value)
```
Sets the client side function to be called when a cell is double clicked. The client function should be declared like this:
function MyOnDoubleClickCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOnDoubleClickRowClientFunction(String value) {#setOnDoubleClickRowClientFunction-java.lang.String-}
```
public void setOnDoubleClickRowClientFunction(String value)
```
Sets the client side function to be called when a row is double clicked. The client function should be declared like this:
function MyOnRowDoubleClick(row)
\{
alert(row);
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOnGridInitClientFunction(String value) {#setOnGridInitClientFunction-java.lang.String-}
```
public void setOnGridInitClientFunction(String value)
```
Sets the client side function name to be called when the grid is initialized. The client function should be declared like this:
function MyOnGridInit(grid)
\{
alert("The grid is initialized: " + grid.id);
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOnPageChangeClientFunction(String value) {#setOnPageChangeClientFunction-java.lang.String-}
```
public void setOnPageChangeClientFunction(String value)
```
Sets the client side function to be called after page index changing.only take effect when EnablePaging is true. The client function should be declared like this:
function MyOnPageChange(index)
\{
console.log("current page is:"+index);
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOnPageSubmitClientFunction(String value) {#setOnPageSubmitClientFunction-java.lang.String-}
```
public void setOnPageSubmitClientFunction(String value)
```
Sets the client function to be called before the page is submitted at client side.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOnShapeSelectedClientFunction(String value) {#setOnShapeSelectedClientFunction-java.lang.String-}
```
public void setOnShapeSelectedClientFunction(String value)
```
Sets the client side function to be called when a shape is selected. The client function should be declared like this:
function MyOnSelectShape(shape)
\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\}
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOnSubmitClientFunction(String value) {#setOnSubmitClientFunction-java.lang.String-}
```
public void setOnSubmitClientFunction(String value)
```
Sets the client function to be called before the control is submitted at client side. The client function should be declared like this:
function MyOnSubmit(arg, cancelEdit)
\{
return true;
\}
The arg is the submit argument, contains the command to be post to the server. The cancelEdit is boolean value indicates whether the control has discarded the user input before submit. The control will continue submitting if the function returns true.
Note: You may use the "this" pointer in the client function to point the grid control which fires the event.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```
Sets whether only fit the rows which height are not customed,the default value is false
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setPageSize(int value) {#setPageSize-int-}
```
public void setPageSize(int value)
```
Sets the page size in paging mode.
**Remarks**
When in paging mode, the control will display PageSize rows of data once, and display the page select control in the tab bar.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setPictureCachePath(String value) {#setPictureCachePath-java.lang.String-}
```
public static void setPictureCachePath(String value)
```
Sets the image storage path for the workbook,all the shapes,images will be stored in this directory, the default path is acwcache under current application Base Directory users need to implement a schedule service to clean the files those are out of session time.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```
Sets the preset style.
See [PresetStyle](../../com.aspose.gridweb/presetstyle).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setRefreshValidation(boolean value) {#setRefreshValidation-boolean-}
```
public void setRefreshValidation(boolean value)
```
Sets whether to refresh validation value after cell value changes.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setRenderHiddenRow(boolean value) {#setRenderHiddenRow-boolean-}
```
public void setRenderHiddenRow(boolean value)
```
Sets whether the hidden row is rendered in GridControl,the default value is false. if you need to unhide the hidden row latter ,you shall set it as true
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setRowHeightForCSV(double value) {#setRowHeightForCSV-double-}
```
public void setRowHeightForCSV(double value)
```
Sets the row height value in point for csv file ,default value is 14.5.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setScrollBarArrowColor(Color value) {#setScrollBarArrowColor-com.aspose.gridweb.Color-}
```
public void setScrollBarArrowColor(Color value)
```
Specifies the color of the scrollbar's arrow button.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |
### setScrollBarBaseColor(Color value) {#setScrollBarBaseColor-com.aspose.gridweb.Color-}
```
public void setScrollBarBaseColor(Color value)
```
Specifies the color of the scroll bar of the control.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |
### setSelectCellBgColor(Color value) {#setSelectCellBgColor-com.aspose.gridweb.Color-}
```
public void setSelectCellBgColor(Color value)
```
Specifies the background color of the selected cells in multi-select range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |
### setSelectCellColor(Color value) {#setSelectCellColor-com.aspose.gridweb.Color-}
```
public void setSelectCellColor(Color value)
```
Specifies the color of the selected cells in multi-select range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |
### setSessionStorePath(String value) {#setSessionStorePath-java.lang.String-}
```
public void setSessionStorePath(String value)
```
Sets the session cache store path when session mode is File or ViewState, etc: gridweb.SessionStorePath="c:/mytempdir/session"; then it will store session data in c:/mytempdir/session
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridweb.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```
Represents the workbook settings.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings) |  |
### setShowAddButton(boolean value) {#setShowAddButton-boolean-}
```
public void setShowAddButton(boolean value)
```
Sets whether to show the add worksheet button.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShowBottomBar(boolean value) {#setShowBottomBar-boolean-}
```
public void setShowBottomBar(boolean value)
```
Specifies whether to show the command bar(includes command bar and tab bar) at the bottom of the control.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShowCellEditBox(boolean value) {#setShowCellEditBox-boolean-}
```
public void setShowCellEditBox(boolean value)
```
whether Gridweb shows edit box toolbar as in MS-EXCEL.if enable ,a edit box for current cell will display in Gridweb. if we enable this feature, we need to import jquery js library in your aspx files to support this new feature. all the latest jquery version is ok. etc.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShowCommandBarAtTop(boolean value) {#setShowCommandBarAtTop-boolean-}
```
public void setShowCommandBarAtTop(boolean value)
```
Specifies whether to show the command bar(includes command bar and tab bar) at the top of the control.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShowContextMenu(boolean value) {#setShowContextMenu-boolean-}
```
public void setShowContextMenu(boolean value)
```
Sets whether to show the context menu. the default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShowDefaultGridLine(boolean value) {#setShowDefaultGridLine-boolean-}
```
public void setShowDefaultGridLine(boolean value)
```
Sets whether to show the default grid lines of the cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShowHeaderBar(boolean value) {#setShowHeaderBar-boolean-}
```
public void setShowHeaderBar(boolean value)
```
Sets whether to show header bar
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShowLoading(boolean value) {#setShowLoading-boolean-}
```
public void setShowLoading(boolean value)
```
Specifies whether to show a loading dialogbox while postbacking to server.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShowLoadingPosition(String value) {#setShowLoadingPosition-java.lang.String-}
```
public void setShowLoadingPosition(String value)
```
Specifies the left,top postion(in px) to show the loading dialogbox while postbacking to server ,etc. 100,200 means the loading dialogbox's left,top postion is at 100px,200px .
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setShowSaveButton(boolean value) {#setShowSaveButton-boolean-}
```
public void setShowSaveButton(boolean value)
```
Sets whether to show the save button.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShowSubmitButton(boolean value) {#setShowSubmitButton-boolean-}
```
public void setShowSubmitButton(boolean value)
```
Sets whether to show the submit button.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShowTabBar(boolean value) {#setShowTabBar-boolean-}
```
public void setShowTabBar(boolean value)
```
Sets whether to show the tab bar.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShowTabNavigation(boolean value) {#setShowTabNavigation-boolean-}
```
public void setShowTabNavigation(boolean value)
```
Sets whether the tab navigation button is show,the default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShowUndoButton(boolean value) {#setShowUndoButton-boolean-}
```
public void setShowUndoButton(boolean value)
```
Sets whether to show the undo button.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSpanWrap(boolean value) {#setSpanWrap-boolean-}
```
public void setSpanWrap(boolean value)
```
Specifies whether to wrap content in the cell span.the default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setTabIndex(short value) {#setTabIndex-short-}
```
public void setTabIndex(short value)
```
Sets the TabIndex in the WebControl
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | short |  |
### setTabStyle(GridTableItemStyle value) {#setTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setTabStyle(GridTableItemStyle value)
```
Sets the style of the tab bar.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |
### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```
Sets the ToolTip in the WebControl
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setUseClientPageHeight(boolean value) {#setUseClientPageHeight-boolean-}
```
public void setUseClientPageHeight(boolean value)
```
Sets whether gridweb use client page height as control height ,suitable for when set Height="100%",default value is false
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setViewPanelScrollLeft(String value) {#setViewPanelScrollLeft-java.lang.String-}
```
public void setViewPanelScrollLeft(String value)
```
Sets the position of the scroll bar of the grid's view panel.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setViewPanelScrollTop(String value) {#setViewPanelScrollTop-java.lang.String-}
```
public void setViewPanelScrollTop(String value)
```
Sets the position of the scroll bar of the grid's view panel.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setViewTableStyle(GridTableStyle value) {#setViewTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setViewTableStyle(GridTableStyle value)
```
Sets the data view panel's style.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |
### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```
Sets the width( System.Web.UI.WebControl.Unit ) of the control.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |
### setXhtmlMode(boolean value) {#setXhtmlMode-boolean-}
```
public void setXhtmlMode(boolean value)
```
Sets whether to use XHTML style,the default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```
### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
