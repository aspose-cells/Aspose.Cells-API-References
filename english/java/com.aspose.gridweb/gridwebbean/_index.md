---
title: GridWebBean
second_title: Aspose.Cells for Java API Reference
description: Represents GridWeb java bean
type: docs
url: /java/com.aspose.gridweb/gridwebbean/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.ExtWebControl](../../com.aspose.gridweb/extwebcontrol), [com.aspose.gridweb.MainWeb](../../com.aspose.gridweb/mainweb)
```
public class GridWebBean extends MainWeb
```

Represents GridWeb java bean
## Constructors

| Constructor | Description |
| --- | --- |
| [GridWebBean()](#GridWebBean--) |  |
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
| [CellError](#CellError) | Occurs when a cell's input value error. |
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
| [SheetDataUpdated](#SheetDataUpdated) | Occurs when the control has loaded the posted data and updated the sheet data. |
| [SheetTabClick](#SheetTabClick) | Occurs when the sheet tab is clicked. |
| [SubmitCommand](#SubmitCommand) | Occurs when the "submit" button is clicked. |
| [UndoCommand](#UndoCommand) | Occurs when the "undo" button is clicked. |
## Methods

| Method | Description |
| --- | --- |
| [calculateFormula()](#calculateFormula--) | Calculates the result of formulas. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getACWClientPath()](#getACWClientPath--) | the web path of the script/image files of the control. |
| [getACWLanguageFileUrl()](#getACWLanguageFileUrl--) | the web url of the language file of the control. |
| [getActiveCell()](#getActiveCell--) | the active cell of the current sheet. |
| [getActiveCellBgColor()](#getActiveCellBgColor--) | Specifies the background color of the active cell. |
| [getActiveCellColor()](#getActiveCellColor--) | Specifies the color of the active cell. |
| [getActiveHeaderBgColor()](#getActiveHeaderBgColor--) | Specifies the background color of the active row/column header. |
| [getActiveHeaderColor()](#getActiveHeaderColor--) | Specifies the color of the active row/column header. |
| [getActiveSheet()](#getActiveSheet--) | Gets the active sheet |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | the active sheet index. |
| [getActiveTabStyle()](#getActiveTabStyle--) | Specifies the style of the active tab. |
| [getAutoRefreshChart()](#getAutoRefreshChart--) | whether the Chart image is updated while updating the cell value.the default is true |
| [getBeanID()](#getBeanID--) | get the html id of the bean |
| [getBottomTableStyle()](#getBottomTableStyle--) | the style of the bottom bar of the control. |
| [getClass()](#getClass--) |  |
| [getCurrentPageIndex()](#getCurrentPageIndex--) |  |
| [getCustomCalculationEngine()](#getCustomCalculationEngine--) | Represents user's custom calculation engine to extend the default calculation engine of Aspose.Cells. |
| [getCustomCommandButtons()](#getCustomCommandButtons--) |  |
| [getCustomStyleFileName()](#getCustomStyleFileName--) | the custom style file name. |
| [getDefaultFontName()](#getDefaultFontName--) | the control's default font name. |
| [getDefaultGridLineColor()](#getDefaultGridLineColor--) | the default grid line's color. |
| [getDisplayCellTip()](#getDisplayCellTip--) |  |
| [getEditMode()](#getEditMode--) | the control's edit mode. |
| [getEnableAJAX()](#getEnableAJAX--) |  |
| [getEnableAsync()](#getEnableAsync--) | whether load cells data in asynchronous way,suggest to apply for one sheet with more than 10000 cells. |
| [getEnableClientColumnOperations()](#getEnableClientColumnOperations--) | whether to enable the client side column operations. |
| [getEnableClientFreeze()](#getEnableClientFreeze--) | whether to enable the client side freezing operations. |
| [getEnableClientMergeOperations()](#getEnableClientMergeOperations--) | whether to enable the client side merge operations. |
| [getEnableClientResizeColumnRow()](#getEnableClientResizeColumnRow--) | whether to enable the client side resize column and row. |
| [getEnableClientRowOperations()](#getEnableClientRowOperations--) | whether to enable the client side row operations. |
| [getEnableDoubleClickEvent()](#getEnableDoubleClickEvent--) | whether to enable customer side double-click event. |
| [getEnableMetalLightEffect()](#getEnableMetalLightEffect--) | whether to apply metal light effect. |
| [getEnablePaging()](#getEnablePaging--) | whether to enable the control's paging mode. |
| [getEnableStyleDialogbox()](#getEnableStyleDialogbox--) | whether to enable the client side style dialogbox. |
| [getFilteredPaging()](#getFilteredPaging--) | whether to enable the paging after data filtered,will take affect when EnablePaging is true. |
| [getForceValidation()](#getForceValidation--) | whether to force customer side validation. |
| [getFrameTableStyle()](#getFrameTableStyle--) | the frame style of the control. |
| [getGoonDefaultSaveOperation()](#getGoonDefaultSaveOperation--) | whether GridWeb will do the default save operation ,the default value is true. |
| [getHTMLBody()](#getHTMLBody--) | the html code of the bean for html body, it shall be get after call of method init and prepareRender |
| [getHTMLHead()](#getHTMLHead--) | the html code of the bean for html head, it shall be get after call of method init and prepareRender |
| [getHeaderBarStyle()](#getHeaderBarStyle--) | the header bar's style. |
| [getHeaderBarTableStyle()](#getHeaderBarTableStyle--) | the header bar style of the control. |
| [getIgnoreStyleWithNoData()](#getIgnoreStyleWithNoData--) | whether GridWeb ignores showing rows or columns that do not contain cell values but are still styled. |
| [getLinksTable()](#getLinksTable--) |  |
| [getMaxColumn()](#getMaxColumn--) | the maximum display column index(zero based) of the web sheet. |
| [getMaxRow()](#getMaxRow--) | the maximum display row index(zero based) of the web sheet. |
| [getMessage()](#getMessage--) |  |
| [getMinColumn()](#getMinColumn--) |  |
| [getMinRow()](#getMinRow--) | the minimum display row index(zero based) of the web sheet. |
| [getModifiedCells()](#getModifiedCells--) | Gets the collection of the cells that modified by the client. |
| [getNeedRenderGroupRows()](#getNeedRenderGroupRows--) | whether to show grouprows . |
| [getNoHScroll()](#getNoHScroll--) | a value indicating whether the horizontal scroll bar is hidden. |
| [getNoScroll()](#getNoScroll--) |  |
| [getNoVScroll()](#getNoVScroll--) | a value indicating whether the vertical scroll bar is hidden. |
| [getOnAjaxCallFinishedClientFunction()](#getOnAjaxCallFinishedClientFunction--) | the client side function name to be called when ajaxcall finished. |
| [getOnCellErrorClientFunction()](#getOnCellErrorClientFunction--) | the client side function name to be called when a cell's validation is failed. |
| [getOnCellSelectedAjaxCallBackClientFunction()](#getOnCellSelectedAjaxCallBackClientFunction--) | the client side function to be called when a cell is selected. |
| [getOnCellSelectedClientFunction()](#getOnCellSelectedClientFunction--) | the client side function to be called when a cell is selected. |
| [getOnCellUnselectedClientFunction()](#getOnCellUnselectedClientFunction--) | the client side function to be called when a cell is unselected. |
| [getOnCellUpdatedClientFunction()](#getOnCellUpdatedClientFunction--) | the client side function name to be called when a cell's value is updated. |
| [getOnContextMenuShowClientFunction()](#getOnContextMenuShowClientFunction--) | the client side function to be called when the context menu will be shown. |
| [getOnDoubleClickCellClientFunction()](#getOnDoubleClickCellClientFunction--) | the client side function to be called when a cell is double clicked. |
| [getOnDoubleClickRowClientFunction()](#getOnDoubleClickRowClientFunction--) | the client side function to be called when a row is double clicked. |
| [getOnGridInitClientFunction()](#getOnGridInitClientFunction--) | the client side function name to be called when the grid is initialized. |
| [getOnPageChangeClientFunction()](#getOnPageChangeClientFunction--) | the client side function to be called after page index changing.only take effect when EnablePaging is true. |
| [getOnPageSubmitClientFunction()](#getOnPageSubmitClientFunction--) | the client function to be called before the page is submitted at client side. |
| [getOnShapeSelectedClientFunction()](#getOnShapeSelectedClientFunction--) | the client side function to be called when a shape is selected. |
| [getOnSubmitClientFunction()](#getOnSubmitClientFunction--) | the client function to be called before the control is submitted at client side. |
| [getOnlyAuto()](#getOnlyAuto--) | whether only fit the rows which height are not customed,the default value is false |
| [getPageSize()](#getPageSize--) | the page size in paging mode. |
| [getPictureCachePath()](#getPictureCachePath--) | the image storage path for the workbook,all the shapes,images will be stored in this directory, the default path is acwcache under current application Base Directory users need to implement a schedule service to clean the files those are out of session time. |
| [getPicturesTable()](#getPicturesTable--) |  |
| [getPresetStyle()](#getPresetStyle--) | the preset style. |
| [getRefreshValidation()](#getRefreshValidation--) | whether to refresh validation value after cell value changes. |
| [getRenderHiddenRow()](#getRenderHiddenRow--) | whether the hidden row is rendered in GridControl,the default value is false. |
| [getScrollBarArrowColor()](#getScrollBarArrowColor--) | Specifies the color of the scrollbar's arrow button. |
| [getScrollBarBaseColor()](#getScrollBarBaseColor--) | Specifies the color of the scroll bar of the control. |
| [getSelectCellBgColor()](#getSelectCellBgColor--) | Specifies the background color of the selected cells in multi-select range. |
| [getSelectCellColor()](#getSelectCellColor--) | Specifies the color of the selected cells in multi-select range. |
| [getSessionLoaded()](#getSessionLoaded--) |  |
| [getSessionMode()](#getSessionMode--) | the session mode of the grid. |
| [getSessionSaved()](#getSessionSaved--) |  |
| [getSessionStorePath()](#getSessionStorePath--) | the session cache store path when session mode is File or ViewState, etc: gridweb.SessionStorePath="c:/mytempdir/session"; then it will store session data in c:/mytempdir/session |
| [getSettings()](#getSettings--) | Represents the workbook settings. |
| [getShapesTable()](#getShapesTable--) |  |
| [getShowAddButton()](#getShowAddButton--) | whether to show the add worksheet button. |
| [getShowBottomBar()](#getShowBottomBar--) |  |
| [getShowCellEditBox()](#getShowCellEditBox--) | whether Gridweb shows edit box toolbar as in MS-EXCEL.if enable ,a edit box for current cell will display in Gridweb. |
| [getShowCommandBarAtTop()](#getShowCommandBarAtTop--) | Specifies whether to show the command bar(includes command bar and tab bar) at the top of the control. |
| [getShowContextMenu()](#getShowContextMenu--) |  |
| [getShowDefaultGridLine()](#getShowDefaultGridLine--) | whether to show the default grid lines of the cells. |
| [getShowHeaderBar()](#getShowHeaderBar--) |  |
| [getShowLoading()](#getShowLoading--) | Specifies whether to show a loading dialogbox while postbacking to server. |
| [getShowLoadingPosition()](#getShowLoadingPosition--) | Specifies the left,top postion(in px) to show the loading dialogbox while postbacking to server ,etc. 100,200 means the loading dialogbox's left,top postion is at 100px,200px . |
| [getShowSaveButton()](#getShowSaveButton--) | whether to show the save button. |
| [getShowSubmitButton()](#getShowSubmitButton--) | whether to show the submit button. |
| [getShowTabBar()](#getShowTabBar--) |  |
| [getShowTabNavigation()](#getShowTabNavigation--) | whether the tab navigation button is show,the default value is true. |
| [getShowUndoButton()](#getShowUndoButton--) | whether to show the undo button. |
| [getSpanWrap()](#getSpanWrap--) | Specifies whether to wrap content in the cell span.the default value is true. |
| [getTabStyle()](#getTabStyle--) | the style of the tab bar. |
| [getUseClientPageHeight()](#getUseClientPageHeight--) | whether gridweb use client page height as control height ,suitable for when set Height="100%",default value is false |
| [getValidationsTable()](#getValidationsTable--) |  |
| [getViewPanelScrollLeft()](#getViewPanelScrollLeft--) | the position of the scroll bar of the grid's view panel. |
| [getViewPanelScrollTop()](#getViewPanelScrollTop--) | the position of the scroll bar of the grid's view panel. |
| [getViewTableStyle()](#getViewTableStyle--) | the data view panel's style. |
| [getWorkSheets()](#getWorkSheets--) |  |
| [getXhtmlMode()](#getXhtmlMode--) |  |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream stream)](#importExcelFile-java.io.InputStream-) | Imports from an excel file stream, including disk file stream or memory stream. |
| [importExcelFile(InputStream stream, String passwordtoOpen)](#importExcelFile-java.io.InputStream-java.lang.String-) | Imports from an excel file stream, including disk file stream or memory stream. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | Imports from an excel file. |
| [importExcelFile(String fileName, String passwordtoOpen)](#importExcelFile-java.lang.String-java.lang.String-) | Imports from an excel file. |
| [init()](#init--) | the bean shall be initialized by the servlet request and response of the current page |
| [isCalculateFormula()](#isCalculateFormula--) | whether to calculate formula after cell value changes or after import File. |
| [isPostBack()](#isPostBack--) | Gets a value indicating whether gridweb is being loaded in response to a client postback, or if it is being loaded and accessed for the first time. |
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
| [setACWClientPath(String value)](#setACWClientPath-java.lang.String-) | For the description of this property, please see [getACWClientPath()](../../com.aspose.gridweb/mainweb\#getACWClientPath--) |
| [setACWLanguageFileUrl(String value)](#setACWLanguageFileUrl-java.lang.String-) | For the description of this property, please see [getACWLanguageFileUrl()](../../com.aspose.gridweb/mainweb\#getACWLanguageFileUrl--) |
| [setActiveCell(GridCell value)](#setActiveCell-com.aspose.gridweb.GridCell-) | For the description of this property, please see [getActiveCell()](../../com.aspose.gridweb/mainweb\#getActiveCell--) |
| [setActiveCellBgColor(Color value)](#setActiveCellBgColor-com.aspose.gridweb.Color-) | For the description of this property, please see [getActiveCellBgColor()](../../com.aspose.gridweb/mainweb\#getActiveCellBgColor--) |
| [setActiveCellColor(Color value)](#setActiveCellColor-com.aspose.gridweb.Color-) | For the description of this property, please see [getActiveCellColor()](../../com.aspose.gridweb/mainweb\#getActiveCellColor--) |
| [setActiveHeaderBgColor(Color value)](#setActiveHeaderBgColor-com.aspose.gridweb.Color-) | For the description of this property, please see [getActiveHeaderBgColor()](../../com.aspose.gridweb/mainweb\#getActiveHeaderBgColor--) |
| [setActiveHeaderColor(Color value)](#setActiveHeaderColor-com.aspose.gridweb.Color-) | For the description of this property, please see [getActiveHeaderColor()](../../com.aspose.gridweb/mainweb\#getActiveHeaderColor--) |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | For the description of this property, please see [getActiveSheetIndex()](../../com.aspose.gridweb/mainweb\#getActiveSheetIndex--) |
| [setActiveTabStyle(GridTableItemStyle value)](#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-) | For the description of this property, please see [getActiveTabStyle()](../../com.aspose.gridweb/mainweb\#getActiveTabStyle--) |
| [setAutoRefreshChart(boolean value)](#setAutoRefreshChart-boolean-) | For the description of this property, please see [getAutoRefreshChart()](../../com.aspose.gridweb/mainweb\#getAutoRefreshChart--) |
| [setBeanID(String beanID)](#setBeanID-java.lang.String-) | set the html id of the bean |
| [setBottomTableStyle(GridTableStyle value)](#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-) | For the description of this property, please see [getBottomTableStyle()](../../com.aspose.gridweb/mainweb\#getBottomTableStyle--) |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | For the description of this property, please see [isCalculateFormula()](../../com.aspose.gridweb/mainweb\#isCalculateFormula--) |
| [setCurrentPageIndex(int value)](#setCurrentPageIndex-int-) | For the description of this property, please see [getCurrentPageIndex()](../../com.aspose.gridweb/mainweb\#getCurrentPageIndex--) |
| [setCustomCalculationEngine(GridAbstractCalculationEngine value)](#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-) | For the description of this property, please see [getCustomCalculationEngine()](../../com.aspose.gridweb/mainweb\#getCustomCalculationEngine--) |
| [setCustomStyle(InputStream stream)](#setCustomStyle-java.io.InputStream-) | sets the custom style file from stream including disk file stream or memory stream. |
| [setCustomStyleFileName(String value)](#setCustomStyleFileName-java.lang.String-) | For the description of this property, please see [getCustomStyleFileName()](../../com.aspose.gridweb/mainweb\#getCustomStyleFileName--) |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | For the description of this property, please see [getDefaultFontName()](../../com.aspose.gridweb/mainweb\#getDefaultFontName--) |
| [setDefaultGridLineColor(Color value)](#setDefaultGridLineColor-com.aspose.gridweb.Color-) | For the description of this property, please see [getDefaultGridLineColor()](../../com.aspose.gridweb/mainweb\#getDefaultGridLineColor--) |
| [setDisplayCellTip(boolean value)](#setDisplayCellTip-boolean-) | For the description of this property, please see [getDisplayCellTip()](../../com.aspose.gridweb/mainweb\#getDisplayCellTip--) |
| [setEditMode(boolean value)](#setEditMode-boolean-) | For the description of this property, please see [getEditMode()](../../com.aspose.gridweb/mainweb\#getEditMode--) |
| [setEnableAJAX(boolean value)](#setEnableAJAX-boolean-) | For the description of this property, please see [getEnableAJAX()](../../com.aspose.gridweb/mainweb\#getEnableAJAX--) |
| [setEnableAsync(boolean value)](#setEnableAsync-boolean-) | For the description of this property, please see [getEnableAsync()](../../com.aspose.gridweb/mainweb\#getEnableAsync--) |
| [setEnableClientColumnOperations(boolean value)](#setEnableClientColumnOperations-boolean-) | For the description of this property, please see [getEnableClientColumnOperations()](../../com.aspose.gridweb/mainweb\#getEnableClientColumnOperations--) |
| [setEnableClientFreeze(boolean value)](#setEnableClientFreeze-boolean-) | For the description of this property, please see [getEnableClientFreeze()](../../com.aspose.gridweb/mainweb\#getEnableClientFreeze--) |
| [setEnableClientMergeOperations(boolean value)](#setEnableClientMergeOperations-boolean-) | For the description of this property, please see [getEnableClientMergeOperations()](../../com.aspose.gridweb/mainweb\#getEnableClientMergeOperations--) |
| [setEnableClientResizeColumnRow(boolean value)](#setEnableClientResizeColumnRow-boolean-) | For the description of this property, please see [getEnableClientResizeColumnRow()](../../com.aspose.gridweb/mainweb\#getEnableClientResizeColumnRow--) |
| [setEnableClientRowOperations(boolean value)](#setEnableClientRowOperations-boolean-) | For the description of this property, please see [getEnableClientRowOperations()](../../com.aspose.gridweb/mainweb\#getEnableClientRowOperations--) |
| [setEnableDoubleClickEvent(boolean value)](#setEnableDoubleClickEvent-boolean-) | For the description of this property, please see [getEnableDoubleClickEvent()](../../com.aspose.gridweb/mainweb\#getEnableDoubleClickEvent--) |
| [setEnableMetalLightEffect(boolean value)](#setEnableMetalLightEffect-boolean-) | For the description of this property, please see [getEnableMetalLightEffect()](../../com.aspose.gridweb/mainweb\#getEnableMetalLightEffect--) |
| [setEnablePaging(boolean value)](#setEnablePaging-boolean-) | For the description of this property, please see [getEnablePaging()](../../com.aspose.gridweb/mainweb\#getEnablePaging--) |
| [setEnableStyleDialogbox(boolean value)](#setEnableStyleDialogbox-boolean-) | For the description of this property, please see [getEnableStyleDialogbox()](../../com.aspose.gridweb/mainweb\#getEnableStyleDialogbox--) |
| [setFilteredPaging(boolean value)](#setFilteredPaging-boolean-) | For the description of this property, please see [getFilteredPaging()](../../com.aspose.gridweb/mainweb\#getFilteredPaging--) |
| [setForceValidation(boolean value)](#setForceValidation-boolean-) | For the description of this property, please see [getForceValidation()](../../com.aspose.gridweb/mainweb\#getForceValidation--) |
| [setFrameTableStyle(GridTableStyle value)](#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-) | For the description of this property, please see [getFrameTableStyle()](../../com.aspose.gridweb/mainweb\#getFrameTableStyle--) |
| [setGoonDefaultSaveOperation(boolean value)](#setGoonDefaultSaveOperation-boolean-) | For the description of this property, please see [getGoonDefaultSaveOperation()](../../com.aspose.gridweb/mainweb\#getGoonDefaultSaveOperation--) |
| [setHeaderBarStyle(GridTableItemStyle value)](#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-) | For the description of this property, please see [getHeaderBarStyle()](../../com.aspose.gridweb/mainweb\#getHeaderBarStyle--) |
| [setHeaderBarTableStyle(GridTableStyle value)](#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-) | For the description of this property, please see [getHeaderBarTableStyle()](../../com.aspose.gridweb/mainweb\#getHeaderBarTableStyle--) |
| [setIgnoreStyleWithNoData(boolean value)](#setIgnoreStyleWithNoData-boolean-) | For the description of this property, please see [getIgnoreStyleWithNoData()](../../com.aspose.gridweb/mainweb\#getIgnoreStyleWithNoData--) |
| [setMaxColumn(int value)](#setMaxColumn-int-) | For the description of this property, please see [getMaxColumn()](../../com.aspose.gridweb/mainweb\#getMaxColumn--) |
| [setMaxRow(int value)](#setMaxRow-int-) | For the description of this property, please see [getMaxRow()](../../com.aspose.gridweb/mainweb\#getMaxRow--) |
| [setMessage(String value)](#setMessage-java.lang.String-) | For the description of this property, please see [getMessage()](../../com.aspose.gridweb/mainweb\#getMessage--) |
| [setMinColumn(int value)](#setMinColumn-int-) | For the description of this property, please see [getMinColumn()](../../com.aspose.gridweb/mainweb\#getMinColumn--) |
| [setMinRow(int value)](#setMinRow-int-) | For the description of this property, please see [getMinRow()](../../com.aspose.gridweb/mainweb\#getMinRow--) |
| [setNeedRenderGroupRows(boolean value)](#setNeedRenderGroupRows-boolean-) | For the description of this property, please see [getNeedRenderGroupRows()](../../com.aspose.gridweb/mainweb\#getNeedRenderGroupRows--) |
| [setNoHScroll(boolean value)](#setNoHScroll-boolean-) | For the description of this property, please see [getNoHScroll()](../../com.aspose.gridweb/mainweb\#getNoHScroll--) |
| [setNoScroll(boolean value)](#setNoScroll-boolean-) | For the description of this property, please see [getNoScroll()](../../com.aspose.gridweb/mainweb\#getNoScroll--) |
| [setNoVScroll(boolean value)](#setNoVScroll-boolean-) | For the description of this property, please see [getNoVScroll()](../../com.aspose.gridweb/mainweb\#getNoVScroll--) |
| [setOnAjaxCallFinishedClientFunction(String value)](#setOnAjaxCallFinishedClientFunction-java.lang.String-) | For the description of this property, please see [getOnAjaxCallFinishedClientFunction()](../../com.aspose.gridweb/mainweb\#getOnAjaxCallFinishedClientFunction--) |
| [setOnCellErrorClientFunction(String value)](#setOnCellErrorClientFunction-java.lang.String-) | For the description of this property, please see [getOnCellErrorClientFunction()](../../com.aspose.gridweb/mainweb\#getOnCellErrorClientFunction--) |
| [setOnCellSelectedAjaxCallBackClientFunction(String value)](#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-) | For the description of this property, please see [getOnCellSelectedAjaxCallBackClientFunction()](../../com.aspose.gridweb/mainweb\#getOnCellSelectedAjaxCallBackClientFunction--) |
| [setOnCellSelectedClientFunction(String value)](#setOnCellSelectedClientFunction-java.lang.String-) | For the description of this property, please see [getOnCellSelectedClientFunction()](../../com.aspose.gridweb/mainweb\#getOnCellSelectedClientFunction--) |
| [setOnCellUnselectedClientFunction(String value)](#setOnCellUnselectedClientFunction-java.lang.String-) | For the description of this property, please see [getOnCellUnselectedClientFunction()](../../com.aspose.gridweb/mainweb\#getOnCellUnselectedClientFunction--) |
| [setOnCellUpdatedClientFunction(String value)](#setOnCellUpdatedClientFunction-java.lang.String-) | For the description of this property, please see [getOnCellUpdatedClientFunction()](../../com.aspose.gridweb/mainweb\#getOnCellUpdatedClientFunction--) |
| [setOnContextMenuShowClientFunction(String value)](#setOnContextMenuShowClientFunction-java.lang.String-) | For the description of this property, please see [getOnContextMenuShowClientFunction()](../../com.aspose.gridweb/mainweb\#getOnContextMenuShowClientFunction--) |
| [setOnDoubleClickCellClientFunction(String value)](#setOnDoubleClickCellClientFunction-java.lang.String-) | For the description of this property, please see [getOnDoubleClickCellClientFunction()](../../com.aspose.gridweb/mainweb\#getOnDoubleClickCellClientFunction--) |
| [setOnDoubleClickRowClientFunction(String value)](#setOnDoubleClickRowClientFunction-java.lang.String-) | For the description of this property, please see [getOnDoubleClickRowClientFunction()](../../com.aspose.gridweb/mainweb\#getOnDoubleClickRowClientFunction--) |
| [setOnGridInitClientFunction(String value)](#setOnGridInitClientFunction-java.lang.String-) | For the description of this property, please see [getOnGridInitClientFunction()](../../com.aspose.gridweb/mainweb\#getOnGridInitClientFunction--) |
| [setOnPageChangeClientFunction(String value)](#setOnPageChangeClientFunction-java.lang.String-) | For the description of this property, please see [getOnPageChangeClientFunction()](../../com.aspose.gridweb/mainweb\#getOnPageChangeClientFunction--) |
| [setOnPageSubmitClientFunction(String value)](#setOnPageSubmitClientFunction-java.lang.String-) | For the description of this property, please see [getOnPageSubmitClientFunction()](../../com.aspose.gridweb/mainweb\#getOnPageSubmitClientFunction--) |
| [setOnShapeSelectedClientFunction(String value)](#setOnShapeSelectedClientFunction-java.lang.String-) | For the description of this property, please see [getOnShapeSelectedClientFunction()](../../com.aspose.gridweb/mainweb\#getOnShapeSelectedClientFunction--) |
| [setOnSubmitClientFunction(String value)](#setOnSubmitClientFunction-java.lang.String-) | For the description of this property, please see [getOnSubmitClientFunction()](../../com.aspose.gridweb/mainweb\#getOnSubmitClientFunction--) |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | For the description of this property, please see [getOnlyAuto()](../../com.aspose.gridweb/mainweb\#getOnlyAuto--) |
| [setPageSize(int value)](#setPageSize-int-) | For the description of this property, please see [getPageSize()](../../com.aspose.gridweb/mainweb\#getPageSize--) |
| [setPictureCachePath(String value)](#setPictureCachePath-java.lang.String-) | For the description of this property, please see [getPictureCachePath()](../../com.aspose.gridweb/mainweb\#getPictureCachePath--) |
| [setPresetStyle(int value)](#setPresetStyle-int-) | For the description of this property, please see [getPresetStyle()](../../com.aspose.gridweb/mainweb\#getPresetStyle--) |
| [setRefreshValidation(boolean value)](#setRefreshValidation-boolean-) | For the description of this property, please see [getRefreshValidation()](../../com.aspose.gridweb/mainweb\#getRefreshValidation--) |
| [setRenderHiddenRow(boolean value)](#setRenderHiddenRow-boolean-) | For the description of this property, please see [getRenderHiddenRow()](../../com.aspose.gridweb/mainweb\#getRenderHiddenRow--) |
| [setScrollBarArrowColor(Color value)](#setScrollBarArrowColor-com.aspose.gridweb.Color-) | For the description of this property, please see [getScrollBarArrowColor()](../../com.aspose.gridweb/mainweb\#getScrollBarArrowColor--) |
| [setScrollBarBaseColor(Color value)](#setScrollBarBaseColor-com.aspose.gridweb.Color-) | For the description of this property, please see [getScrollBarBaseColor()](../../com.aspose.gridweb/mainweb\#getScrollBarBaseColor--) |
| [setSelectCellBgColor(Color value)](#setSelectCellBgColor-com.aspose.gridweb.Color-) | For the description of this property, please see [getSelectCellBgColor()](../../com.aspose.gridweb/mainweb\#getSelectCellBgColor--) |
| [setSelectCellColor(Color value)](#setSelectCellColor-com.aspose.gridweb.Color-) | For the description of this property, please see [getSelectCellColor()](../../com.aspose.gridweb/mainweb\#getSelectCellColor--) |
| [setSessionLoaded(boolean value)](#setSessionLoaded-boolean-) | For the description of this property, please see [getSessionLoaded()](../../com.aspose.gridweb/mainweb\#getSessionLoaded--) |
| [setSessionMode(int value)](#setSessionMode-int-) | For the description of this property, please see [getSessionMode()](../../com.aspose.gridweb/mainweb\#getSessionMode--) |
| [setSessionSaved(boolean value)](#setSessionSaved-boolean-) | For the description of this property, please see [getSessionSaved()](../../com.aspose.gridweb/mainweb\#getSessionSaved--) |
| [setSessionStorePath(String value)](#setSessionStorePath-java.lang.String-) | For the description of this property, please see [getSessionStorePath()](../../com.aspose.gridweb/mainweb\#getSessionStorePath--) |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridweb.GridWorkbookSettings-) | For the description of this property, please see [getSettings()](../../com.aspose.gridweb/mainweb\#getSettings--) |
| [setShowAddButton(boolean value)](#setShowAddButton-boolean-) | For the description of this property, please see [getShowAddButton()](../../com.aspose.gridweb/mainweb\#getShowAddButton--) |
| [setShowBottomBar(boolean value)](#setShowBottomBar-boolean-) | For the description of this property, please see [getShowBottomBar()](../../com.aspose.gridweb/mainweb\#getShowBottomBar--) |
| [setShowCellEditBox(boolean value)](#setShowCellEditBox-boolean-) | For the description of this property, please see [getShowCellEditBox()](../../com.aspose.gridweb/mainweb\#getShowCellEditBox--) |
| [setShowCommandBarAtTop(boolean value)](#setShowCommandBarAtTop-boolean-) | For the description of this property, please see [getShowCommandBarAtTop()](../../com.aspose.gridweb/mainweb\#getShowCommandBarAtTop--) |
| [setShowContextMenu(boolean value)](#setShowContextMenu-boolean-) | For the description of this property, please see [getShowContextMenu()](../../com.aspose.gridweb/mainweb\#getShowContextMenu--) |
| [setShowDefaultGridLine(boolean value)](#setShowDefaultGridLine-boolean-) | For the description of this property, please see [getShowDefaultGridLine()](../../com.aspose.gridweb/mainweb\#getShowDefaultGridLine--) |
| [setShowHeaderBar(boolean value)](#setShowHeaderBar-boolean-) | For the description of this property, please see [getShowHeaderBar()](../../com.aspose.gridweb/mainweb\#getShowHeaderBar--) |
| [setShowLoading(boolean value)](#setShowLoading-boolean-) | For the description of this property, please see [getShowLoading()](../../com.aspose.gridweb/mainweb\#getShowLoading--) |
| [setShowLoadingPosition(String value)](#setShowLoadingPosition-java.lang.String-) | For the description of this property, please see [getShowLoadingPosition()](../../com.aspose.gridweb/mainweb\#getShowLoadingPosition--) |
| [setShowSaveButton(boolean value)](#setShowSaveButton-boolean-) | For the description of this property, please see [getShowSaveButton()](../../com.aspose.gridweb/mainweb\#getShowSaveButton--) |
| [setShowSubmitButton(boolean value)](#setShowSubmitButton-boolean-) | For the description of this property, please see [getShowSubmitButton()](../../com.aspose.gridweb/mainweb\#getShowSubmitButton--) |
| [setShowTabBar(boolean value)](#setShowTabBar-boolean-) | For the description of this property, please see [getShowTabBar()](../../com.aspose.gridweb/mainweb\#getShowTabBar--) |
| [setShowTabNavigation(boolean value)](#setShowTabNavigation-boolean-) | For the description of this property, please see [getShowTabNavigation()](../../com.aspose.gridweb/mainweb\#getShowTabNavigation--) |
| [setShowUndoButton(boolean value)](#setShowUndoButton-boolean-) | For the description of this property, please see [getShowUndoButton()](../../com.aspose.gridweb/mainweb\#getShowUndoButton--) |
| [setSpanWrap(boolean value)](#setSpanWrap-boolean-) | For the description of this property, please see [getSpanWrap()](../../com.aspose.gridweb/mainweb\#getSpanWrap--) |
| [setTabStyle(GridTableItemStyle value)](#setTabStyle-com.aspose.gridweb.GridTableItemStyle-) | For the description of this property, please see [getTabStyle()](../../com.aspose.gridweb/mainweb\#getTabStyle--) |
| [setUseClientPageHeight(boolean value)](#setUseClientPageHeight-boolean-) | For the description of this property, please see [getUseClientPageHeight()](../../com.aspose.gridweb/mainweb\#getUseClientPageHeight--) |
| [setViewPanelScrollLeft(String value)](#setViewPanelScrollLeft-java.lang.String-) | For the description of this property, please see [getViewPanelScrollLeft()](../../com.aspose.gridweb/mainweb\#getViewPanelScrollLeft--) |
| [setViewPanelScrollTop(String value)](#setViewPanelScrollTop-java.lang.String-) | For the description of this property, please see [getViewPanelScrollTop()](../../com.aspose.gridweb/mainweb\#getViewPanelScrollTop--) |
| [setViewTableStyle(GridTableStyle value)](#setViewTableStyle-com.aspose.gridweb.GridTableStyle-) | For the description of this property, please see [getViewTableStyle()](../../com.aspose.gridweb/mainweb\#getViewTableStyle--) |
| [setXhtmlMode(boolean value)](#setXhtmlMode-boolean-) | For the description of this property, please see [getXhtmlMode()](../../com.aspose.gridweb/mainweb\#getXhtmlMode--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWebBean() {#GridWebBean--}
```
public GridWebBean()
```


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

### CellError {#CellError}
```
public CellErrorHandler CellError
```


Occurs when a cell's input value error.

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

### SheetDataUpdated {#SheetDataUpdated}
```
public WorkbookEventHandler SheetDataUpdated
```


Occurs when the control has loaded the posted data and updated the sheet data.

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


the web path of the script/image files of the control. For example: "http://localhost/acw\_client". You may also set this value in the web.config file. Add this section to the <configuration> section:
<appSettings>

<add key="aspose.cells.gridweb.acw\_client\_path" value="/acw\_client/" />

</appSettings>


**Returns:**
java.lang.String
### getACWLanguageFileUrl() {#getACWLanguageFileUrl--}
```
public String getACWLanguageFileUrl()
```


the web url of the language file of the control. For example: "/acw\_client/lang\_en.js".
By default, a built-in english file is used.


**Returns:**
java.lang.String
### getActiveCell() {#getActiveCell--}
```
public GridCell getActiveCell()
```


the active cell of the current sheet. Changed to be writable since version 1.9.0.1.

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


the active sheet index. Equal to the WebWorksheets.ActiveSheetIndex.

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


whether the Chart image is updated while updating the cell value.the default is true

**Returns:**
boolean
### getBeanID() {#getBeanID--}
```
public String getBeanID()
```


get the html id of the bean

**Returns:**
java.lang.String
### getBottomTableStyle() {#getBottomTableStyle--}
```
public GridTableStyle getBottomTableStyle()
```


the style of the bottom bar of the control.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentPageIndex() {#getCurrentPageIndex--}
```
public int getCurrentPageIndex()
```




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




**Returns:**
[CustomCommandButtonCollection](../../com.aspose.gridweb/customcommandbuttoncollection)
### getCustomStyleFileName() {#getCustomStyleFileName--}
```
public String getCustomStyleFileName()
```


the custom style file name. The custom style file is an XML file. When sets the file name, the file will be loaded immediately. Hear is the content of the "standard preset style" ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

```
GridWeb1.setCustomStyleFileName("c:\\style\\mystyle.xml");
```

**Returns:**
java.lang.String
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


the control's default font name.

```
GridWeb1.setDefaultFontName("Arial");
```

**Returns:**
java.lang.String
### getDefaultGridLineColor() {#getDefaultGridLineColor--}
```
public Color getDefaultGridLineColor()
```


the default grid line's color.

```
GridWeb1.setDefaultGridLineColor(Color.getRed());
```

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getDisplayCellTip() {#getDisplayCellTip--}
```
public boolean getDisplayCellTip()
```




**Returns:**
boolean
### getEditMode() {#getEditMode--}
```
public boolean getEditMode()
```


the control's edit mode. When sets to true, the control's cells are editable, and the "save" and the "undo" icon are displayed. When sets to false, the control's cells are readonly, and the "save" and the "undo" icon are not displayed.

**Returns:**
boolean
### getEnableAJAX() {#getEnableAJAX--}
```
public boolean getEnableAJAX()
```




**Returns:**
boolean
### getEnableAsync() {#getEnableAsync--}
```
public boolean getEnableAsync()
```


whether load cells data in asynchronous way,suggest to apply for one sheet with more than 10000 cells.

**Returns:**
boolean
### getEnableClientColumnOperations() {#getEnableClientColumnOperations--}
```
public boolean getEnableClientColumnOperations()
```


whether to enable the client side column operations. When sets to true, the user can use the right-click menu to add/remove columns.

**Returns:**
boolean
### getEnableClientFreeze() {#getEnableClientFreeze--}
```
public boolean getEnableClientFreeze()
```


whether to enable the client side freezing operations. When sets to true, the user can use the right-click menu to freeze/unfreeze panes.

**Returns:**
boolean
### getEnableClientMergeOperations() {#getEnableClientMergeOperations--}
```
public boolean getEnableClientMergeOperations()
```


whether to enable the client side merge operations. When sets to true, the user can use the right-click menu to merge/unmerge cells.

**Returns:**
boolean
### getEnableClientResizeColumnRow() {#getEnableClientResizeColumnRow--}
```
public boolean getEnableClientResizeColumnRow()
```


whether to enable the client side resize column and row. When sets to true, the user can resize the column and row at client side.

**Returns:**
boolean
### getEnableClientRowOperations() {#getEnableClientRowOperations--}
```
public boolean getEnableClientRowOperations()
```


whether to enable the client side row operations. When sets to true, the user can use the right-click menu to add/remove rows.

**Returns:**
boolean
### getEnableDoubleClickEvent() {#getEnableDoubleClickEvent--}
```
public boolean getEnableDoubleClickEvent()
```


whether to enable customer side double-click event. When sets to true, the control will receive customer side double-click events and you may handle these events on the server side. Otherwise the control will ignore any double-click events.

**Returns:**
boolean
### getEnableMetalLightEffect() {#getEnableMetalLightEffect--}
```
public boolean getEnableMetalLightEffect()
```


whether to apply metal light effect.

**Returns:**
boolean
### getEnablePaging() {#getEnablePaging--}
```
public boolean getEnablePaging()
```


whether to enable the control's paging mode. When sets to true, the control will display PageSize rows of data once, and display the page select control in the tab bar.

**Returns:**
boolean
### getEnableStyleDialogbox() {#getEnableStyleDialogbox--}
```
public boolean getEnableStyleDialogbox()
```


whether to enable the client side style dialogbox. When sets to true, the user can use the style dialogbox to set a cell's style by selecting the "Format Cell..." from the popup menu.

**Returns:**
boolean
### getFilteredPaging() {#getFilteredPaging--}
```
public boolean getFilteredPaging()
```


whether to enable the paging after data filtered,will take affect when EnablePaging is true. When sets to true, the control will paging based on filtered data,the default value is false.

**Returns:**
boolean
### getForceValidation() {#getForceValidation--}
```
public boolean getForceValidation()
```


whether to force customer side validation. When sets to true, data will not post to server until all input fields are valid.

**Returns:**
boolean
### getFrameTableStyle() {#getFrameTableStyle--}
```
public GridTableStyle getFrameTableStyle()
```


the frame style of the control.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getGoonDefaultSaveOperation() {#getGoonDefaultSaveOperation--}
```
public boolean getGoonDefaultSaveOperation()
```


whether GridWeb will do the default save operation ,the default value is true.

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
### getHeaderBarStyle() {#getHeaderBarStyle--}
```
public GridTableItemStyle getHeaderBarStyle()
```


the header bar's style.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getHeaderBarTableStyle() {#getHeaderBarTableStyle--}
```
public GridTableStyle getHeaderBarTableStyle()
```


the header bar style of the control.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getIgnoreStyleWithNoData() {#getIgnoreStyleWithNoData--}
```
public boolean getIgnoreStyleWithNoData()
```


whether GridWeb ignores showing rows or columns that do not contain cell values but are still styled. If set to true, the performance will be better. The default value is false, which means that if the last consecutive row/column has no cell values but is styled, we will still display them. This option is only valid when EnableAsync is false. This option has no effect when EnableAsync is true, which means GridWeb will show all rows/columns with style.

**Returns:**
boolean
### getLinksTable() {#getLinksTable--}
```
public HashMap getLinksTable()
```




**Returns:**
java.util.HashMap
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


the maximum display column index(zero based) of the web sheet. The control uses the greater value of MaxColumn and sheet data's max column.

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


the maximum display row index(zero based) of the web sheet. The control uses the greater value of MaxRow and sheet data's max row.

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




**Returns:**
java.lang.String
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```




**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


the minimum display row index(zero based) of the web sheet. The control uses the smaller value of MinRow and sheet data's min row.

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


whether to show grouprows .

**Returns:**
boolean
### getNoHScroll() {#getNoHScroll--}
```
public boolean getNoHScroll()
```


a value indicating whether the horizontal scroll bar is hidden.

**Returns:**
boolean
### getNoScroll() {#getNoScroll--}
```
public boolean getNoScroll()
```




**Returns:**
boolean
### getNoVScroll() {#getNoVScroll--}
```
public boolean getNoVScroll()
```


a value indicating whether the vertical scroll bar is hidden.

**Returns:**
boolean
### getOnAjaxCallFinishedClientFunction() {#getOnAjaxCallFinishedClientFunction--}
```
public String getOnAjaxCallFinishedClientFunction()
```


the client side function name to be called when ajaxcall finished. The client function should be declared like this:
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


the client side function name to be called when a cell's validation is failed. The client function should be declared like this:
function MyOnCellError(cell)
\{
alert(GridWeb1.getCellValueByCell(cell));
\}

Note: You may use the "this" pointer in the client function to point the grid control which fires the event.

**Returns:**
java.lang.String
### getOnCellSelectedAjaxCallBackClientFunction() {#getOnCellSelectedAjaxCallBackClientFunction--}
```
public String getOnCellSelectedAjaxCallBackClientFunction()
```


the client side function to be called when a cell is selected. The client function should be declared like this:
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


the client side function to be called when a cell is selected. The client function should be declared like this:
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


the client side function to be called when a cell is unselected. The client function should be declared like this:
function MyOnUnselectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, "test");
\}

Note: You may use the "this" pointer in the client function to point the grid control which fires the event.

**Returns:**
java.lang.String
### getOnCellUpdatedClientFunction() {#getOnCellUpdatedClientFunction--}
```
public String getOnCellUpdatedClientFunction()
```


the client side function name to be called when a cell's value is updated. The client function should be declared like this:
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


the client side function to be called when the context menu will be shown. The client function should be declared like this:
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


the client side function to be called when a cell is double clicked. The client function should be declared like this:
function MyOnDoubleClickCell(cell)
\{
GridWeb1.setCellValueByCell(cell, "test");
\}

Note: You may use the "this" pointer in the client function to point the grid control which fires the event.

**Returns:**
java.lang.String
### getOnDoubleClickRowClientFunction() {#getOnDoubleClickRowClientFunction--}
```
public String getOnDoubleClickRowClientFunction()
```


the client side function to be called when a row is double clicked. The client function should be declared like this:
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


the client side function name to be called when the grid is initialized. The client function should be declared like this:
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


the client side function to be called after page index changing.only take effect when EnablePaging is true. The client function should be declared like this:
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


the client function to be called before the page is submitted at client side.

**Returns:**
java.lang.String
### getOnShapeSelectedClientFunction() {#getOnShapeSelectedClientFunction--}
```
public String getOnShapeSelectedClientFunction()
```


the client side function to be called when a shape is selected. The client function should be declared like this:
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


the client function to be called before the control is submitted at client side. The client function should be declared like this:
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


whether only fit the rows which height are not customed,the default value is false

**Returns:**
boolean
### getPageSize() {#getPageSize--}
```
public int getPageSize()
```


the page size in paging mode. When in paging mode, the control will display PageSize rows of data once, and display the page select control in the tab bar.

**Returns:**
int
### getPictureCachePath() {#getPictureCachePath--}
```
public static String getPictureCachePath()
```


the image storage path for the workbook,all the shapes,images will be stored in this directory, the default path is acwcache under current application Base Directory users need to implement a schedule service to clean the files those are out of session time.

**Returns:**
java.lang.String
### getPicturesTable() {#getPicturesTable--}
```
public HashMap getPicturesTable()
```




**Returns:**
java.util.HashMap
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


the preset style.

```
GridWeb1.setPresetStyle(PresetStyle.TRADITIONAL_1);
```

**Returns:**
int
### getRefreshValidation() {#getRefreshValidation--}
```
public boolean getRefreshValidation()
```


whether to refresh validation value after cell value changes.

**Returns:**
boolean
### getRenderHiddenRow() {#getRenderHiddenRow--}
```
public boolean getRenderHiddenRow()
```


whether the hidden row is rendered in GridControl,the default value is false. if you need to unhide the hidden row latter ,you shall set it as true

**Returns:**
boolean
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
### getSessionLoaded() {#getSessionLoaded--}
```
public boolean getSessionLoaded()
```




**Returns:**
boolean
### getSessionMode() {#getSessionMode--}
```
public int getSessionMode()
```


the session mode of the grid. There are 4 type of session mode:
1. Session(default): Use system session to store sheet data.
Generally the asp.net uses InProc session state. The grid also supports "StateServer" out process session state and SQLServer session state.
2. ViewState: Use page's viewstate to store sheet data.
3. Custom: Use LoadCustomData and SheetDataUpdated events to store/recover sheet data.
4. File: store/recover sheet data in SessionStorePath.
When using SessionMode.ViewState, the grid will store sheets data in the page's view state. This will decrease the server's memory usage, but the page's size will be larger and it will impact the overall performance.

```
GridWeb1.setSessionMode(SessionMode.VIEW_STATE);
```

**Returns:**
int
### getSessionSaved() {#getSessionSaved--}
```
public boolean getSessionSaved()
```




**Returns:**
boolean
### getSessionStorePath() {#getSessionStorePath--}
```
public String getSessionStorePath()
```


the session cache store path when session mode is File or ViewState, etc: gridweb.SessionStorePath="c:/mytempdir/session"; then it will store session data in c:/mytempdir/session

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Represents the workbook settings.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings)
### getShapesTable() {#getShapesTable--}
```
public HashMap getShapesTable()
```




**Returns:**
java.util.HashMap
### getShowAddButton() {#getShowAddButton--}
```
public boolean getShowAddButton()
```


whether to show the add worksheet button.

**Returns:**
boolean
### getShowBottomBar() {#getShowBottomBar--}
```
public boolean getShowBottomBar()
```




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




**Returns:**
boolean
### getShowDefaultGridLine() {#getShowDefaultGridLine--}
```
public boolean getShowDefaultGridLine()
```


whether to show the default grid lines of the cells.

**Returns:**
boolean
### getShowHeaderBar() {#getShowHeaderBar--}
```
public boolean getShowHeaderBar()
```




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


whether to show the save button.

**Returns:**
boolean
### getShowSubmitButton() {#getShowSubmitButton--}
```
public boolean getShowSubmitButton()
```


whether to show the submit button.

**Returns:**
boolean
### getShowTabBar() {#getShowTabBar--}
```
public boolean getShowTabBar()
```




**Returns:**
boolean
### getShowTabNavigation() {#getShowTabNavigation--}
```
public boolean getShowTabNavigation()
```


whether the tab navigation button is show,the default value is true.

**Returns:**
boolean
### getShowUndoButton() {#getShowUndoButton--}
```
public boolean getShowUndoButton()
```


whether to show the undo button.

**Returns:**
boolean
### getSpanWrap() {#getSpanWrap--}
```
public boolean getSpanWrap()
```


Specifies whether to wrap content in the cell span.the default value is true.

**Returns:**
boolean
### getTabStyle() {#getTabStyle--}
```
public GridTableItemStyle getTabStyle()
```


the style of the tab bar.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getUseClientPageHeight() {#getUseClientPageHeight--}
```
public boolean getUseClientPageHeight()
```


whether gridweb use client page height as control height ,suitable for when set Height="100%",default value is false

**Returns:**
boolean
### getValidationsTable() {#getValidationsTable--}
```
public HashMap getValidationsTable()
```




**Returns:**
java.util.HashMap
### getViewPanelScrollLeft() {#getViewPanelScrollLeft--}
```
public String getViewPanelScrollLeft()
```


the position of the scroll bar of the grid's view panel.

**Returns:**
java.lang.String
### getViewPanelScrollTop() {#getViewPanelScrollTop--}
```
public String getViewPanelScrollTop()
```


the position of the scroll bar of the grid's view panel.

**Returns:**
java.lang.String
### getViewTableStyle() {#getViewTableStyle--}
```
public GridTableStyle getViewTableStyle()
```


the data view panel's style.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getWorkSheets() {#getWorkSheets--}
```
public GridWorksheetCollection getWorkSheets()
```




**Returns:**
[GridWorksheetCollection](../../com.aspose.gridweb/gridworksheetcollection)
### getXhtmlMode() {#getXhtmlMode--}
```
public boolean getXhtmlMode()
```




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


whether to calculate formula after cell value changes or after import File. The default value is true.

**Returns:**
boolean
### isPostBack() {#isPostBack--}
```
public boolean isPostBack()
```


Gets a value indicating whether gridweb is being loaded in response to a client postback, or if it is being loaded and accessed for the first time.

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
| format | int | The file format(Excel2003, Excel2007, CSV, SpreadsheetML) |

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
| format | int | The file format(Excel2003, Excel2007, CSV, SpreadsheetML) |

### setACWClientPath(String value) {#setACWClientPath-java.lang.String-}
```
public void setACWClientPath(String value)
```


For the description of this property, please see [getACWClientPath()](../../com.aspose.gridweb/mainweb\#getACWClientPath--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setACWLanguageFileUrl(String value) {#setACWLanguageFileUrl-java.lang.String-}
```
public void setACWLanguageFileUrl(String value)
```


For the description of this property, please see [getACWLanguageFileUrl()](../../com.aspose.gridweb/mainweb\#getACWLanguageFileUrl--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setActiveCell(GridCell value) {#setActiveCell-com.aspose.gridweb.GridCell-}
```
public void setActiveCell(GridCell value)
```


For the description of this property, please see [getActiveCell()](../../com.aspose.gridweb/mainweb\#getActiveCell--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setActiveCellBgColor(Color value) {#setActiveCellBgColor-com.aspose.gridweb.Color-}
```
public void setActiveCellBgColor(Color value)
```


For the description of this property, please see [getActiveCellBgColor()](../../com.aspose.gridweb/mainweb\#getActiveCellBgColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveCellColor(Color value) {#setActiveCellColor-com.aspose.gridweb.Color-}
```
public void setActiveCellColor(Color value)
```


For the description of this property, please see [getActiveCellColor()](../../com.aspose.gridweb/mainweb\#getActiveCellColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderBgColor(Color value) {#setActiveHeaderBgColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderBgColor(Color value)
```


For the description of this property, please see [getActiveHeaderBgColor()](../../com.aspose.gridweb/mainweb\#getActiveHeaderBgColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderColor(Color value) {#setActiveHeaderColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderColor(Color value)
```


For the description of this property, please see [getActiveHeaderColor()](../../com.aspose.gridweb/mainweb\#getActiveHeaderColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


For the description of this property, please see [getActiveSheetIndex()](../../com.aspose.gridweb/mainweb\#getActiveSheetIndex--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setActiveTabStyle(GridTableItemStyle value) {#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setActiveTabStyle(GridTableItemStyle value)
```


For the description of this property, please see [getActiveTabStyle()](../../com.aspose.gridweb/mainweb\#getActiveTabStyle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setAutoRefreshChart(boolean value) {#setAutoRefreshChart-boolean-}
```
public void setAutoRefreshChart(boolean value)
```


For the description of this property, please see [getAutoRefreshChart()](../../com.aspose.gridweb/mainweb\#getAutoRefreshChart--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBeanID(String beanID) {#setBeanID-java.lang.String-}
```
public void setBeanID(String beanID)
```


set the html id of the bean

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| beanID | java.lang.String |  |

### setBottomTableStyle(GridTableStyle value) {#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setBottomTableStyle(GridTableStyle value)
```


For the description of this property, please see [getBottomTableStyle()](../../com.aspose.gridweb/mainweb\#getBottomTableStyle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


For the description of this property, please see [isCalculateFormula()](../../com.aspose.gridweb/mainweb\#isCalculateFormula--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCurrentPageIndex(int value) {#setCurrentPageIndex-int-}
```
public void setCurrentPageIndex(int value)
```


For the description of this property, please see [getCurrentPageIndex()](../../com.aspose.gridweb/mainweb\#getCurrentPageIndex--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCustomCalculationEngine(GridAbstractCalculationEngine value) {#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-}
```
public void setCustomCalculationEngine(GridAbstractCalculationEngine value)
```


For the description of this property, please see [getCustomCalculationEngine()](../../com.aspose.gridweb/mainweb\#getCustomCalculationEngine--)

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


For the description of this property, please see [getCustomStyleFileName()](../../com.aspose.gridweb/mainweb\#getCustomStyleFileName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


For the description of this property, please see [getDefaultFontName()](../../com.aspose.gridweb/mainweb\#getDefaultFontName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setDefaultGridLineColor(Color value) {#setDefaultGridLineColor-com.aspose.gridweb.Color-}
```
public void setDefaultGridLineColor(Color value)
```


For the description of this property, please see [getDefaultGridLineColor()](../../com.aspose.gridweb/mainweb\#getDefaultGridLineColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setDisplayCellTip(boolean value) {#setDisplayCellTip-boolean-}
```
public void setDisplayCellTip(boolean value)
```


For the description of this property, please see [getDisplayCellTip()](../../com.aspose.gridweb/mainweb\#getDisplayCellTip--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEditMode(boolean value) {#setEditMode-boolean-}
```
public void setEditMode(boolean value)
```


For the description of this property, please see [getEditMode()](../../com.aspose.gridweb/mainweb\#getEditMode--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableAJAX(boolean value) {#setEnableAJAX-boolean-}
```
public void setEnableAJAX(boolean value)
```


For the description of this property, please see [getEnableAJAX()](../../com.aspose.gridweb/mainweb\#getEnableAJAX--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableAsync(boolean value) {#setEnableAsync-boolean-}
```
public void setEnableAsync(boolean value)
```


For the description of this property, please see [getEnableAsync()](../../com.aspose.gridweb/mainweb\#getEnableAsync--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableClientColumnOperations(boolean value) {#setEnableClientColumnOperations-boolean-}
```
public void setEnableClientColumnOperations(boolean value)
```


For the description of this property, please see [getEnableClientColumnOperations()](../../com.aspose.gridweb/mainweb\#getEnableClientColumnOperations--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableClientFreeze(boolean value) {#setEnableClientFreeze-boolean-}
```
public void setEnableClientFreeze(boolean value)
```


For the description of this property, please see [getEnableClientFreeze()](../../com.aspose.gridweb/mainweb\#getEnableClientFreeze--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableClientMergeOperations(boolean value) {#setEnableClientMergeOperations-boolean-}
```
public void setEnableClientMergeOperations(boolean value)
```


For the description of this property, please see [getEnableClientMergeOperations()](../../com.aspose.gridweb/mainweb\#getEnableClientMergeOperations--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableClientResizeColumnRow(boolean value) {#setEnableClientResizeColumnRow-boolean-}
```
public void setEnableClientResizeColumnRow(boolean value)
```


For the description of this property, please see [getEnableClientResizeColumnRow()](../../com.aspose.gridweb/mainweb\#getEnableClientResizeColumnRow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableClientRowOperations(boolean value) {#setEnableClientRowOperations-boolean-}
```
public void setEnableClientRowOperations(boolean value)
```


For the description of this property, please see [getEnableClientRowOperations()](../../com.aspose.gridweb/mainweb\#getEnableClientRowOperations--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableDoubleClickEvent(boolean value) {#setEnableDoubleClickEvent-boolean-}
```
public void setEnableDoubleClickEvent(boolean value)
```


For the description of this property, please see [getEnableDoubleClickEvent()](../../com.aspose.gridweb/mainweb\#getEnableDoubleClickEvent--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableMetalLightEffect(boolean value) {#setEnableMetalLightEffect-boolean-}
```
public void setEnableMetalLightEffect(boolean value)
```


For the description of this property, please see [getEnableMetalLightEffect()](../../com.aspose.gridweb/mainweb\#getEnableMetalLightEffect--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnablePaging(boolean value) {#setEnablePaging-boolean-}
```
public void setEnablePaging(boolean value)
```


For the description of this property, please see [getEnablePaging()](../../com.aspose.gridweb/mainweb\#getEnablePaging--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableStyleDialogbox(boolean value) {#setEnableStyleDialogbox-boolean-}
```
public void setEnableStyleDialogbox(boolean value)
```


For the description of this property, please see [getEnableStyleDialogbox()](../../com.aspose.gridweb/mainweb\#getEnableStyleDialogbox--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFilteredPaging(boolean value) {#setFilteredPaging-boolean-}
```
public void setFilteredPaging(boolean value)
```


For the description of this property, please see [getFilteredPaging()](../../com.aspose.gridweb/mainweb\#getFilteredPaging--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setForceValidation(boolean value) {#setForceValidation-boolean-}
```
public void setForceValidation(boolean value)
```


For the description of this property, please see [getForceValidation()](../../com.aspose.gridweb/mainweb\#getForceValidation--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFrameTableStyle(GridTableStyle value) {#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setFrameTableStyle(GridTableStyle value)
```


For the description of this property, please see [getFrameTableStyle()](../../com.aspose.gridweb/mainweb\#getFrameTableStyle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setGoonDefaultSaveOperation(boolean value) {#setGoonDefaultSaveOperation-boolean-}
```
public void setGoonDefaultSaveOperation(boolean value)
```


For the description of this property, please see [getGoonDefaultSaveOperation()](../../com.aspose.gridweb/mainweb\#getGoonDefaultSaveOperation--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHeaderBarStyle(GridTableItemStyle value) {#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setHeaderBarStyle(GridTableItemStyle value)
```


For the description of this property, please see [getHeaderBarStyle()](../../com.aspose.gridweb/mainweb\#getHeaderBarStyle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setHeaderBarTableStyle(GridTableStyle value) {#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setHeaderBarTableStyle(GridTableStyle value)
```


For the description of this property, please see [getHeaderBarTableStyle()](../../com.aspose.gridweb/mainweb\#getHeaderBarTableStyle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setIgnoreStyleWithNoData(boolean value) {#setIgnoreStyleWithNoData-boolean-}
```
public void setIgnoreStyleWithNoData(boolean value)
```


For the description of this property, please see [getIgnoreStyleWithNoData()](../../com.aspose.gridweb/mainweb\#getIgnoreStyleWithNoData--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMaxColumn(int value) {#setMaxColumn-int-}
```
public void setMaxColumn(int value)
```


For the description of this property, please see [getMaxColumn()](../../com.aspose.gridweb/mainweb\#getMaxColumn--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMaxRow(int value) {#setMaxRow-int-}
```
public void setMaxRow(int value)
```


For the description of this property, please see [getMaxRow()](../../com.aspose.gridweb/mainweb\#getMaxRow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMessage(String value) {#setMessage-java.lang.String-}
```
public void setMessage(String value)
```


For the description of this property, please see [getMessage()](../../com.aspose.gridweb/mainweb\#getMessage--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setMinColumn(int value) {#setMinColumn-int-}
```
public void setMinColumn(int value)
```


For the description of this property, please see [getMinColumn()](../../com.aspose.gridweb/mainweb\#getMinColumn--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMinRow(int value) {#setMinRow-int-}
```
public void setMinRow(int value)
```


For the description of this property, please see [getMinRow()](../../com.aspose.gridweb/mainweb\#getMinRow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setNeedRenderGroupRows(boolean value) {#setNeedRenderGroupRows-boolean-}
```
public void setNeedRenderGroupRows(boolean value)
```


For the description of this property, please see [getNeedRenderGroupRows()](../../com.aspose.gridweb/mainweb\#getNeedRenderGroupRows--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setNoHScroll(boolean value) {#setNoHScroll-boolean-}
```
public void setNoHScroll(boolean value)
```


For the description of this property, please see [getNoHScroll()](../../com.aspose.gridweb/mainweb\#getNoHScroll--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setNoScroll(boolean value) {#setNoScroll-boolean-}
```
public void setNoScroll(boolean value)
```


For the description of this property, please see [getNoScroll()](../../com.aspose.gridweb/mainweb\#getNoScroll--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setNoVScroll(boolean value) {#setNoVScroll-boolean-}
```
public void setNoVScroll(boolean value)
```


For the description of this property, please see [getNoVScroll()](../../com.aspose.gridweb/mainweb\#getNoVScroll--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setOnAjaxCallFinishedClientFunction(String value) {#setOnAjaxCallFinishedClientFunction-java.lang.String-}
```
public void setOnAjaxCallFinishedClientFunction(String value)
```


For the description of this property, please see [getOnAjaxCallFinishedClientFunction()](../../com.aspose.gridweb/mainweb\#getOnAjaxCallFinishedClientFunction--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOnCellErrorClientFunction(String value) {#setOnCellErrorClientFunction-java.lang.String-}
```
public void setOnCellErrorClientFunction(String value)
```


For the description of this property, please see [getOnCellErrorClientFunction()](../../com.aspose.gridweb/mainweb\#getOnCellErrorClientFunction--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOnCellSelectedAjaxCallBackClientFunction(String value) {#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-}
```
public void setOnCellSelectedAjaxCallBackClientFunction(String value)
```


For the description of this property, please see [getOnCellSelectedAjaxCallBackClientFunction()](../../com.aspose.gridweb/mainweb\#getOnCellSelectedAjaxCallBackClientFunction--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOnCellSelectedClientFunction(String value) {#setOnCellSelectedClientFunction-java.lang.String-}
```
public void setOnCellSelectedClientFunction(String value)
```


For the description of this property, please see [getOnCellSelectedClientFunction()](../../com.aspose.gridweb/mainweb\#getOnCellSelectedClientFunction--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOnCellUnselectedClientFunction(String value) {#setOnCellUnselectedClientFunction-java.lang.String-}
```
public void setOnCellUnselectedClientFunction(String value)
```


For the description of this property, please see [getOnCellUnselectedClientFunction()](../../com.aspose.gridweb/mainweb\#getOnCellUnselectedClientFunction--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOnCellUpdatedClientFunction(String value) {#setOnCellUpdatedClientFunction-java.lang.String-}
```
public void setOnCellUpdatedClientFunction(String value)
```


For the description of this property, please see [getOnCellUpdatedClientFunction()](../../com.aspose.gridweb/mainweb\#getOnCellUpdatedClientFunction--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOnContextMenuShowClientFunction(String value) {#setOnContextMenuShowClientFunction-java.lang.String-}
```
public void setOnContextMenuShowClientFunction(String value)
```


For the description of this property, please see [getOnContextMenuShowClientFunction()](../../com.aspose.gridweb/mainweb\#getOnContextMenuShowClientFunction--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOnDoubleClickCellClientFunction(String value) {#setOnDoubleClickCellClientFunction-java.lang.String-}
```
public void setOnDoubleClickCellClientFunction(String value)
```


For the description of this property, please see [getOnDoubleClickCellClientFunction()](../../com.aspose.gridweb/mainweb\#getOnDoubleClickCellClientFunction--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOnDoubleClickRowClientFunction(String value) {#setOnDoubleClickRowClientFunction-java.lang.String-}
```
public void setOnDoubleClickRowClientFunction(String value)
```


For the description of this property, please see [getOnDoubleClickRowClientFunction()](../../com.aspose.gridweb/mainweb\#getOnDoubleClickRowClientFunction--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOnGridInitClientFunction(String value) {#setOnGridInitClientFunction-java.lang.String-}
```
public void setOnGridInitClientFunction(String value)
```


For the description of this property, please see [getOnGridInitClientFunction()](../../com.aspose.gridweb/mainweb\#getOnGridInitClientFunction--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOnPageChangeClientFunction(String value) {#setOnPageChangeClientFunction-java.lang.String-}
```
public void setOnPageChangeClientFunction(String value)
```


For the description of this property, please see [getOnPageChangeClientFunction()](../../com.aspose.gridweb/mainweb\#getOnPageChangeClientFunction--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOnPageSubmitClientFunction(String value) {#setOnPageSubmitClientFunction-java.lang.String-}
```
public void setOnPageSubmitClientFunction(String value)
```


For the description of this property, please see [getOnPageSubmitClientFunction()](../../com.aspose.gridweb/mainweb\#getOnPageSubmitClientFunction--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOnShapeSelectedClientFunction(String value) {#setOnShapeSelectedClientFunction-java.lang.String-}
```
public void setOnShapeSelectedClientFunction(String value)
```


For the description of this property, please see [getOnShapeSelectedClientFunction()](../../com.aspose.gridweb/mainweb\#getOnShapeSelectedClientFunction--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOnSubmitClientFunction(String value) {#setOnSubmitClientFunction-java.lang.String-}
```
public void setOnSubmitClientFunction(String value)
```


For the description of this property, please see [getOnSubmitClientFunction()](../../com.aspose.gridweb/mainweb\#getOnSubmitClientFunction--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


For the description of this property, please see [getOnlyAuto()](../../com.aspose.gridweb/mainweb\#getOnlyAuto--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPageSize(int value) {#setPageSize-int-}
```
public void setPageSize(int value)
```


For the description of this property, please see [getPageSize()](../../com.aspose.gridweb/mainweb\#getPageSize--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPictureCachePath(String value) {#setPictureCachePath-java.lang.String-}
```
public static void setPictureCachePath(String value)
```


For the description of this property, please see [getPictureCachePath()](../../com.aspose.gridweb/mainweb\#getPictureCachePath--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


For the description of this property, please see [getPresetStyle()](../../com.aspose.gridweb/mainweb\#getPresetStyle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRefreshValidation(boolean value) {#setRefreshValidation-boolean-}
```
public void setRefreshValidation(boolean value)
```


For the description of this property, please see [getRefreshValidation()](../../com.aspose.gridweb/mainweb\#getRefreshValidation--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRenderHiddenRow(boolean value) {#setRenderHiddenRow-boolean-}
```
public void setRenderHiddenRow(boolean value)
```


For the description of this property, please see [getRenderHiddenRow()](../../com.aspose.gridweb/mainweb\#getRenderHiddenRow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setScrollBarArrowColor(Color value) {#setScrollBarArrowColor-com.aspose.gridweb.Color-}
```
public void setScrollBarArrowColor(Color value)
```


For the description of this property, please see [getScrollBarArrowColor()](../../com.aspose.gridweb/mainweb\#getScrollBarArrowColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setScrollBarBaseColor(Color value) {#setScrollBarBaseColor-com.aspose.gridweb.Color-}
```
public void setScrollBarBaseColor(Color value)
```


For the description of this property, please see [getScrollBarBaseColor()](../../com.aspose.gridweb/mainweb\#getScrollBarBaseColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellBgColor(Color value) {#setSelectCellBgColor-com.aspose.gridweb.Color-}
```
public void setSelectCellBgColor(Color value)
```


For the description of this property, please see [getSelectCellBgColor()](../../com.aspose.gridweb/mainweb\#getSelectCellBgColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellColor(Color value) {#setSelectCellColor-com.aspose.gridweb.Color-}
```
public void setSelectCellColor(Color value)
```


For the description of this property, please see [getSelectCellColor()](../../com.aspose.gridweb/mainweb\#getSelectCellColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSessionLoaded(boolean value) {#setSessionLoaded-boolean-}
```
public void setSessionLoaded(boolean value)
```


For the description of this property, please see [getSessionLoaded()](../../com.aspose.gridweb/mainweb\#getSessionLoaded--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSessionMode(int value) {#setSessionMode-int-}
```
public void setSessionMode(int value)
```


For the description of this property, please see [getSessionMode()](../../com.aspose.gridweb/mainweb\#getSessionMode--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSessionSaved(boolean value) {#setSessionSaved-boolean-}
```
public void setSessionSaved(boolean value)
```


For the description of this property, please see [getSessionSaved()](../../com.aspose.gridweb/mainweb\#getSessionSaved--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSessionStorePath(String value) {#setSessionStorePath-java.lang.String-}
```
public void setSessionStorePath(String value)
```


For the description of this property, please see [getSessionStorePath()](../../com.aspose.gridweb/mainweb\#getSessionStorePath--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridweb.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


For the description of this property, please see [getSettings()](../../com.aspose.gridweb/mainweb\#getSettings--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings) |  |

### setShowAddButton(boolean value) {#setShowAddButton-boolean-}
```
public void setShowAddButton(boolean value)
```


For the description of this property, please see [getShowAddButton()](../../com.aspose.gridweb/mainweb\#getShowAddButton--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowBottomBar(boolean value) {#setShowBottomBar-boolean-}
```
public void setShowBottomBar(boolean value)
```


For the description of this property, please see [getShowBottomBar()](../../com.aspose.gridweb/mainweb\#getShowBottomBar--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowCellEditBox(boolean value) {#setShowCellEditBox-boolean-}
```
public void setShowCellEditBox(boolean value)
```


For the description of this property, please see [getShowCellEditBox()](../../com.aspose.gridweb/mainweb\#getShowCellEditBox--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowCommandBarAtTop(boolean value) {#setShowCommandBarAtTop-boolean-}
```
public void setShowCommandBarAtTop(boolean value)
```


For the description of this property, please see [getShowCommandBarAtTop()](../../com.aspose.gridweb/mainweb\#getShowCommandBarAtTop--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowContextMenu(boolean value) {#setShowContextMenu-boolean-}
```
public void setShowContextMenu(boolean value)
```


For the description of this property, please see [getShowContextMenu()](../../com.aspose.gridweb/mainweb\#getShowContextMenu--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowDefaultGridLine(boolean value) {#setShowDefaultGridLine-boolean-}
```
public void setShowDefaultGridLine(boolean value)
```


For the description of this property, please see [getShowDefaultGridLine()](../../com.aspose.gridweb/mainweb\#getShowDefaultGridLine--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowHeaderBar(boolean value) {#setShowHeaderBar-boolean-}
```
public void setShowHeaderBar(boolean value)
```


For the description of this property, please see [getShowHeaderBar()](../../com.aspose.gridweb/mainweb\#getShowHeaderBar--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowLoading(boolean value) {#setShowLoading-boolean-}
```
public void setShowLoading(boolean value)
```


For the description of this property, please see [getShowLoading()](../../com.aspose.gridweb/mainweb\#getShowLoading--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowLoadingPosition(String value) {#setShowLoadingPosition-java.lang.String-}
```
public void setShowLoadingPosition(String value)
```


For the description of this property, please see [getShowLoadingPosition()](../../com.aspose.gridweb/mainweb\#getShowLoadingPosition--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setShowSaveButton(boolean value) {#setShowSaveButton-boolean-}
```
public void setShowSaveButton(boolean value)
```


For the description of this property, please see [getShowSaveButton()](../../com.aspose.gridweb/mainweb\#getShowSaveButton--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowSubmitButton(boolean value) {#setShowSubmitButton-boolean-}
```
public void setShowSubmitButton(boolean value)
```


For the description of this property, please see [getShowSubmitButton()](../../com.aspose.gridweb/mainweb\#getShowSubmitButton--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowTabBar(boolean value) {#setShowTabBar-boolean-}
```
public void setShowTabBar(boolean value)
```


For the description of this property, please see [getShowTabBar()](../../com.aspose.gridweb/mainweb\#getShowTabBar--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowTabNavigation(boolean value) {#setShowTabNavigation-boolean-}
```
public void setShowTabNavigation(boolean value)
```


For the description of this property, please see [getShowTabNavigation()](../../com.aspose.gridweb/mainweb\#getShowTabNavigation--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowUndoButton(boolean value) {#setShowUndoButton-boolean-}
```
public void setShowUndoButton(boolean value)
```


For the description of this property, please see [getShowUndoButton()](../../com.aspose.gridweb/mainweb\#getShowUndoButton--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSpanWrap(boolean value) {#setSpanWrap-boolean-}
```
public void setSpanWrap(boolean value)
```


For the description of this property, please see [getSpanWrap()](../../com.aspose.gridweb/mainweb\#getSpanWrap--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTabStyle(GridTableItemStyle value) {#setTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setTabStyle(GridTableItemStyle value)
```


For the description of this property, please see [getTabStyle()](../../com.aspose.gridweb/mainweb\#getTabStyle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setUseClientPageHeight(boolean value) {#setUseClientPageHeight-boolean-}
```
public void setUseClientPageHeight(boolean value)
```


For the description of this property, please see [getUseClientPageHeight()](../../com.aspose.gridweb/mainweb\#getUseClientPageHeight--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setViewPanelScrollLeft(String value) {#setViewPanelScrollLeft-java.lang.String-}
```
public void setViewPanelScrollLeft(String value)
```


For the description of this property, please see [getViewPanelScrollLeft()](../../com.aspose.gridweb/mainweb\#getViewPanelScrollLeft--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setViewPanelScrollTop(String value) {#setViewPanelScrollTop-java.lang.String-}
```
public void setViewPanelScrollTop(String value)
```


For the description of this property, please see [getViewPanelScrollTop()](../../com.aspose.gridweb/mainweb\#getViewPanelScrollTop--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setViewTableStyle(GridTableStyle value) {#setViewTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setViewTableStyle(GridTableStyle value)
```


For the description of this property, please see [getViewTableStyle()](../../com.aspose.gridweb/mainweb\#getViewTableStyle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setXhtmlMode(boolean value) {#setXhtmlMode-boolean-}
```
public void setXhtmlMode(boolean value)
```


For the description of this property, please see [getXhtmlMode()](../../com.aspose.gridweb/mainweb\#getXhtmlMode--)

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

