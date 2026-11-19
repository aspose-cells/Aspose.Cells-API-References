---
title: "GridWeb"
second_title: "Aspose.Cells for Java API 参考"
description: "GridWeb 控件的基本类。"
type: docs
url: /zh/java/com.aspose.gridweb/gridweb/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebControl](../../com.aspose.gridweb/webcontrol), [com.aspose.gridweb.ExtWebControl](../../com.aspose.gridweb/extwebcontrol), [com.aspose.gridweb.MainWeb](../../com.aspose.gridweb/mainweb)
```
public class GridWeb extends MainWeb
```

GridWeb 控件的基本类。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GridWeb()](#GridWeb--) |  |
## 字段

| 字段 | 描述 |
| --- | --- |
| [AfterColumnFilter](#AfterColumnFilter) | 在列过滤后发生。 |
| [AjaxCallFinished](#AjaxCallFinished) | 当控件的 ajax 更新完成时触发。 |
| [BeforeColumnFilter](#BeforeColumnFilter) | 在列过滤之前发生。 |
| [CellClickOnAjax](#CellClickOnAjax) | 当单元格被点击时发生，并且需要为此事件执行 ajax 回调。 |
| [CellClientUpdate](#CellClientUpdate) | 当客户端单元格更新发生时。 |
| [CellCommand](#CellCommand) | 当单元格的命令超链接被点击时发生。 |
| [CellDoubleClick](#CellDoubleClick) | 当单元格被双击时发生。 |
| [CellModifiedOnAjax](#CellModifiedOnAjax) | 当单元格在 ajax 调用中被修改时发生。 |
| [ColumnDeleted](#ColumnDeleted) | 当用户从客户端菜单删除列时发生。 |
| [ColumnDeleting](#ColumnDeleting) | 当用户尝试从客户端菜单删除列时发生。 |
| [ColumnDoubleClick](#ColumnDoubleClick) | 当列标题被双击时发生。 |
| [ColumnInserted](#ColumnInserted) | 当用户从客户端菜单插入列时发生。 |
| [CustomCommand](#CustomCommand) | 当用户点击自定义命令按钮时发生。 |
| [LoadCustomData](#LoadCustomData) | 当控件的 SessionMode 设置为 Custom 并且需要加载工作表数据时触发。 |
| [PageIndexChanged](#PageIndexChanged) | 当控件的工作表页面索引更改时发生。 |
| [RowDeleted](#RowDeleted) | 当用户已从客户端菜单删除行时发生。 |
| [RowDeleting](#RowDeleting) | 当用户尝试从客户端菜单删除行时发生。 |
| [RowDoubleClick](#RowDoubleClick) | 当行标题被双击时发生。 |
| [RowInserted](#RowInserted) | 当用户从客户端菜单插入行时发生。 |
| [SaveCommand](#SaveCommand) | 当点击 "save" 按钮时发生。 |
| [SheetAdded](#SheetAdded) | 当用户从工具栏菜单添加工作表时发生。 |
| [SheetTabClick](#SheetTabClick) | 当工作表标签被点击时发生。 |
| [SubmitCommand](#SubmitCommand) | 当单击 \"submit\" 按钮时发生。 |
| [UndoCommand](#UndoCommand) | 当单击 \"undo\" 按钮时发生。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [calculateFormula()](#calculateFormula--) | 计算公式的结果。 |
| [createChildControls()](#createChildControls--) | 实现来自 WebControl 的 CreateChildControls，仅供内部使用。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getACWClientPath()](#getACWClientPath--) | 获取控件的脚本/图像文件的网络路径。 |
| [getACWLanguageFileUrl()](#getACWLanguageFileUrl--) | 获取控件语言文件的网络 URL。 |
| [getActiveCell()](#getActiveCell--) | 获取当前工作表的活动单元格。 |
| [getActiveCellBgColor()](#getActiveCellBgColor--) | 指定活动单元格的背景颜色。 |
| [getActiveCellColor()](#getActiveCellColor--) | 指定活动单元格的颜色。 |
| [getActiveHeaderBgColor()](#getActiveHeaderBgColor--) | 指定活动行/列标题的背景颜色。 |
| [getActiveHeaderColor()](#getActiveHeaderColor--) | 指定活动行/列标题的颜色。 |
| [getActiveSheet()](#getActiveSheet--) | 获取活动工作表 |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | 获取活动工作表的索引。 |
| [getActiveTabStyle()](#getActiveTabStyle--) | 指定活动标签页的样式。 |
| [getAutoRefreshChart()](#getAutoRefreshChart--) | 获取在更新单元格值时是否更新图表图像。默认值为 true。 |
| [getBackColor()](#getBackColor--) | 获取 WebControl 中的 BackColor |
| [getBorderColor()](#getBorderColor--) | 获取 WebControl 中的 BorderColor |
| [getBorderStyle()](#getBorderStyle--) | 获取 WebControl 中的 BorderStyle |
| [getBorderWidth()](#getBorderWidth--) | 获取 WebControl 中的 BorderWidth |
| [getBottomTableStyle()](#getBottomTableStyle--) | 获取控件底部栏的样式。 |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | 获取 WebControl 中的 CssClass |
| [getCurrentPageIndex()](#getCurrentPageIndex--) | 获取分页模式下的当前页索引。 |
| [getCustomCalculationEngine()](#getCustomCalculationEngine--) | 表示用户的自定义计算引擎，用于扩展 Aspose.Cells 的默认计算引擎。 |
| [getCustomCommandButtons()](#getCustomCommandButtons--) | 获取自定义命令按钮集合。 |
| [getCustomStyleFileName()](#getCustomStyleFileName--) | 获取自定义样式文件名。 |
| [getDPI()](#getDPI--) | 获取/设置机器的 DPI。 |
| [getDefaultFontName()](#getDefaultFontName--) | 获取控件的默认字体名称。 |
| [getDefaultFontSize()](#getDefaultFontSize--) | 获取控件的默认字体大小。 |
| [getDefaultGridLineColor()](#getDefaultGridLineColor--) | 获取默认网格线的颜色。 |
| [getDisplayCellTip()](#getDisplayCellTip--) | 获取是否显示提示。默认值为 true。 |
| [getEditMode()](#getEditMode--) | 获取控件的编辑模式。 |
| [getEnableAJAX()](#getEnableAJAX--) | 获取是否使用 AJAX 调用。默认值为 true。 |
| [getEnableAsync()](#getEnableAsync--) | 获取是否以异步方式加载单元格数据，建议在单个工作表超过 10000 个单元格时使用。 |
| [getEnableClientColumnOperations()](#getEnableClientColumnOperations--) | 获取是否启用客户端列操作。 |
| [getEnableClientFreeze()](#getEnableClientFreeze--) | 获取是否启用客户端冻结操作。 |
| [getEnableClientMergeOperations()](#getEnableClientMergeOperations--) | 获取是否启用客户端合并操作。 |
| [getEnableClientResizeColumnRow()](#getEnableClientResizeColumnRow--) | 获取是否启用客户端列和行的大小调整。 |
| [getEnableClientRowOperations()](#getEnableClientRowOperations--) | 获取是否启用客户端行操作。 |
| [getEnableDoubleClickEvent()](#getEnableDoubleClickEvent--) | 获取是否启用客户侧双击事件。 |
| [getEnableMetalLightEffect()](#getEnableMetalLightEffect--) | 获取是否应用金属光效。 |
| [getEnablePaging()](#getEnablePaging--) | 获取是否启用控件的分页模式。 |
| [getEnableStyleDialogbox()](#getEnableStyleDialogbox--) | 获取是否启用客户端样式对话框。 |
| [getEnabled()](#getEnabled--) | 获取 WebControl 中的 Enabled |
| [getFilteredPaging()](#getFilteredPaging--) | 获取在数据过滤后是否启用分页，EnablePaging 为 true 时生效。 |
| [getFont()](#getFont--) | 获取 WebControl 中的 Font |
| [getForceValidation()](#getForceValidation--) | 获取是否强制客户侧验证。 |
| [getForeColor()](#getForeColor--) | 获取 WebControl 中的 ForeColor |
| [getFrameTableStyle()](#getFrameTableStyle--) | 获取控件的框架样式。 |
| [getGoonDefaultSaveOperation()](#getGoonDefaultSaveOperation--) | 获取 GridWeb 是否执行默认保存操作，默认值为 true。 |
| [getHeaderBarHeight()](#getHeaderBarHeight--) | 获取控件顶部标题栏的高度（System.Web.UI.WebControl.Unit）。 |
| [getHeaderBarStyle()](#getHeaderBarStyle--) | 获取标题栏的样式。 |
| [getHeaderBarTableStyle()](#getHeaderBarTableStyle--) | 获取控件标题栏的样式。 |
| [getHeaderBarWidth()](#getHeaderBarWidth--) | 获取控件左侧标题栏的宽度（System.Web.UI.WebControl.Unit）。 |
| [getHeight()](#getHeight--) | 获取控件的高度（System.Web.UI.WebControl.Unit）。 |
| [getIgnoreStyleWithNoData()](#getIgnoreStyleWithNoData--) | 获取 GridWeb 是否忽略显示没有单元格值但仍有样式的行或列。 |
| [getLoadOptions()](#getLoadOptions--) | 表示 GridWeb 的加载选项。 |
| [getMaxColumn()](#getMaxColumn--) | 获取网页工作表的最大显示列索引（从零开始）。 |
| [getMaxRow()](#getMaxRow--) | 获取网页工作表的最大显示行索引（从零开始）。 |
| [getMessage()](#getMessage--) | 获取网格的消息。 |
| [getMinColumn()](#getMinColumn--) | 获取网页工作表的最小显示列索引（从零开始）。 |
| [getMinRow()](#getMinRow--) | 获取网页工作表的最小显示行索引（从零开始）。 |
| [getModifiedCells()](#getModifiedCells--) | 获取由客户端修改的单元格集合。 |
| [getNeedRenderGroupRows()](#getNeedRenderGroupRows--) | 获取是否显示组行。 |
| [getNoHScroll()](#getNoHScroll--) | 获取指示水平滚动条是否隐藏的值。 |
| [getNoScroll()](#getNoScroll--) | 获取是否显示滚动条。 |
| [getNoVScroll()](#getNoVScroll--) | 获取指示垂直滚动条是否隐藏的值。 |
| [getOnAjaxCallFinishedClientFunction()](#getOnAjaxCallFinishedClientFunction--) | 获取 ajaxcall 完成时要调用的客户端函数名称。 |
| [getOnCellErrorClientFunction()](#getOnCellErrorClientFunction--) | 获取当单元格验证失败时要调用的客户端函数名称。 |
| [getOnCellSelectedAjaxCallBackClientFunction()](#getOnCellSelectedAjaxCallBackClientFunction--) | 获取当单元格被选中时要调用的客户端函数。 |
| [getOnCellSelectedClientFunction()](#getOnCellSelectedClientFunction--) | 获取当单元格被选中时要调用的客户端函数。 |
| [getOnCellUnselectedClientFunction()](#getOnCellUnselectedClientFunction--) | 获取当单元格被取消选中时要调用的客户端函数。 |
| [getOnCellUpdatedClientFunction()](#getOnCellUpdatedClientFunction--) | 获取当单元格的值被更新时要调用的客户端函数名称。 |
| [getOnContextMenuShowClientFunction()](#getOnContextMenuShowClientFunction--) | 获取当上下文菜单将要显示时要调用的客户端函数。 |
| [getOnDoubleClickCellClientFunction()](#getOnDoubleClickCellClientFunction--) | 获取当单元格被双击时要调用的客户端函数。 |
| [getOnDoubleClickRowClientFunction()](#getOnDoubleClickRowClientFunction--) | 获取当行被双击时要调用的客户端函数。 |
| [getOnGridInitClientFunction()](#getOnGridInitClientFunction--) | 获取当网格初始化时要调用的客户端函数名称。 |
| [getOnPageChangeClientFunction()](#getOnPageChangeClientFunction--) | 获取在页面索引更改后要调用的客户端函数，仅在 EnablePaging 为 true 时生效。 |
| [getOnPageSubmitClientFunction()](#getOnPageSubmitClientFunction--) | 获取在页面提交前要在客户端调用的函数。 |
| [getOnShapeSelectedClientFunction()](#getOnShapeSelectedClientFunction--) | 获取当形状被选中时要调用的客户端函数。 |
| [getOnSubmitClientFunction()](#getOnSubmitClientFunction--) | 获取在控件提交前要在客户端调用的函数。 |
| [getOnlyAuto()](#getOnlyAuto--) | 获取是否仅适配高度未自定义的行，默认值为 false。 |
| [getPageSize()](#getPageSize--) | 获取分页模式下的页面大小。 |
| [getPictureCachePath()](#getPictureCachePath--) | 获取工作簿的图像存储路径，所有形状和图像都将存储在此目录中，默认路径是当前应用程序基目录下的 acwcache，用户需要实现一个计划服务来清理超出会话时间的文件。 |
| [getPresetStyle()](#getPresetStyle--) | 获取预设样式。 |
| [getRefreshValidation()](#getRefreshValidation--) | 获取在单元格值更改后是否刷新验证值。 |
| [getRenderHiddenRow()](#getRenderHiddenRow--) | 获取在 GridControl 中是否渲染隐藏行，默认值为 false。 |
| [getRowHeightForCSV()](#getRowHeightForCSV--) | 获取 CSV 文件的行高（单位为点），默认值为 14.5。 |
| [getScrollBarArrowColor()](#getScrollBarArrowColor--) | 指定滚动条箭头按钮的颜色。 |
| [getScrollBarBaseColor()](#getScrollBarBaseColor--) | 指定控件滚动条的颜色。 |
| [getSelectCellBgColor()](#getSelectCellBgColor--) | 指定多选范围内已选单元格的背景颜色。 |
| [getSelectCellColor()](#getSelectCellColor--) | 指定多选范围内已选单元格的颜色。 |
| [getSelectCells()](#getSelectCells--) | 获取已选单元格集合。 |
| [getSessionStorePath()](#getSessionStorePath--) | 当会话模式为 File 或 ViewState 等时获取会话缓存存储路径，例如：gridweb.SessionStorePath="c:/mytempdir/session"；此时会将会话数据存储在 c:/mytempdir/session 中。 |
| [getSettings()](#getSettings--) | 表示工作簿设置。 |
| [getShowAddButton()](#getShowAddButton--) | 获取是否显示添加工作表按钮。 |
| [getShowBottomBar()](#getShowBottomBar--) | 指定是否在控件底部显示命令栏（包括命令栏和标签栏）。 |
| [getShowCellEditBox()](#getShowCellEditBox--) | 是否在 Gridweb 中显示类似 MS-EXCEL 的编辑框工具栏。启用后，将在 Gridweb 中显示当前单元格的编辑框。 |
| [getShowCommandBarAtTop()](#getShowCommandBarAtTop--) | 指定是否在控件顶部显示命令栏（包括命令栏和标签栏）。 |
| [getShowContextMenu()](#getShowContextMenu--) | 获取是否显示上下文菜单。默认值为 true。 |
| [getShowDefaultGridLine()](#getShowDefaultGridLine--) | 获取是否显示单元格的默认网格线。 |
| [getShowHeaderBar()](#getShowHeaderBar--) | 获取是否显示标题栏。 |
| [getShowLoading()](#getShowLoading--) | 指定在回发到服务器期间是否显示加载对话框。 |
| [getShowLoadingPosition()](#getShowLoadingPosition--) | 指定在回发到服务器期间显示加载对话框的左、上位置（单位为像素），例如 100,200 表示加载对话框的左、上位置分别为 100px 和 200px。 |
| [getShowSaveButton()](#getShowSaveButton--) | 获取是否显示保存按钮。 |
| [getShowSubmitButton()](#getShowSubmitButton--) | 获取是否显示提交按钮。 |
| [getShowTabBar()](#getShowTabBar--) | 获取是否显示标签栏。 |
| [getShowTabNavigation()](#getShowTabNavigation--) | 获取标签导航按钮是否显示，默认值为 true。 |
| [getShowUndoButton()](#getShowUndoButton--) | 获取是否显示撤销按钮。 |
| [getSpanWrap()](#getSpanWrap--) | 指定是否在单元格跨越范围内换行内容，默认值为 true。 |
| [getTabIndex()](#getTabIndex--) | 获取 WebControl 中的 TabIndex |
| [getTabStyle()](#getTabStyle--) | 获取标签栏的样式。 |
| [getToolTip()](#getToolTip--) | 获取 WebControl 中的 ToolTip |
| [getUseClientPageHeight()](#getUseClientPageHeight--) | 获取 Gridweb 是否使用客户端页面高度作为控件高度，适用于设置 Height="100%" 的情况，默认值为 false。 |
| [getVersion()](#getVersion--) | 获取发布版本。 |
| [getViewPanelScrollLeft()](#getViewPanelScrollLeft--) | 获取网格视图面板滚动条的位置。 |
| [getViewPanelScrollTop()](#getViewPanelScrollTop--) | 获取网格视图面板滚动条的位置。 |
| [getViewTableStyle()](#getViewTableStyle--) | 获取数据视图面板的样式。 |
| [getWidth()](#getWidth--) | 获取控件的宽度（System.Web.UI.WebControl.Unit）。 |
| [getWorkSheets()](#getWorkSheets--) | 获取工作表的集合。 |
| [getXhtmlMode()](#getXhtmlMode--) | 获取是否使用 XHTML 样式，默认值为 true。 |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream stream)](#importExcelFile-java.io.InputStream-) | 从 Excel 文件流导入，包括磁盘文件流或内存流。 |
| [importExcelFile(InputStream stream, String passwordtoOpen)](#importExcelFile-java.io.InputStream-java.lang.String-) | 从 Excel 文件流导入，包括磁盘文件流或内存流。 |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | 从 Excel 文件导入。 |
| [importExcelFile(String fileName, String passwordtoOpen)](#importExcelFile-java.lang.String-java.lang.String-) | 从 Excel 文件导入。 |
| [isCalculateFormula()](#isCalculateFormula--) | 获取在单元格值更改后或导入文件后是否计算公式。 |
| [loadCSVFile(InputStream stream)](#loadCSVFile-java.io.InputStream-) | 从 CSV 文件流加载数据。 |
| [loadCSVFile(String fileName)](#loadCSVFile-java.lang.String-) | 从 CSV 文件加载数据。 |
| [loadHTMLFile(InputStream stream)](#loadHTMLFile-java.io.InputStream-) | 从 HTML 文件流加载数据。 |
| [loadHTMLFile(String fileName)](#loadHTMLFile-java.lang.String-) | 从 HTML 文件加载数据。 |
| [loadSpreadSheetMLFile(InputStream stream)](#loadSpreadSheetMLFile-java.io.InputStream-) | 从 SpreadSheetML 文件流加载数据。 |
| [loadSpreadSheetMLFile(String fileName)](#loadSpreadSheetMLFile-java.lang.String-) | 从 SpreadSheetML 文件加载数据。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshChartShape()](#refreshChartShape--) | 刷新活动工作表的所有图表图像。 |
| [saveCSVFile(OutputStream stream)](#saveCSVFile-java.io.OutputStream-) | 将数据保存到 CSV 文件流。 |
| [saveCSVFile(String targetFile)](#saveCSVFile-java.lang.String-) | 将数据保存到 CSV 文件。 |
| [saveCustomStyleFile(String fileName)](#saveCustomStyleFile-java.lang.String-) | 将控件的当前样式数据保存到 XML 文件。 |
| [saveHTMLFile(OutputStream stream)](#saveHTMLFile-java.io.OutputStream-) | 将数据保存到 HTML 文件流。 |
| [saveHTMLFile(String targetFile)](#saveHTMLFile-java.lang.String-) | 将数据保存到 HTML 文件。 |
| [saveSpreadSheetMLFile(OutputStream stream)](#saveSpreadSheetMLFile-java.io.OutputStream-) | 将数据保存到 SpreadSheetML 文件流。 |
| [saveSpreadSheetMLFile(String targetFile)](#saveSpreadSheetMLFile-java.lang.String-) | 将数据保存到 SpreadSheetML 文件。 |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | 将工作表保存到 Excel 文件。 |
| [saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)](#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-) | 将工作表保存到 Excel 文件。 |
| [saveToExcelFile(OutputStream stream, int format)](#saveToExcelFile-java.io.OutputStream-int-) | 将工作表保存到 Excel 文件。 |
| [saveToExcelFile(String targetFile)](#saveToExcelFile-java.lang.String-) | 将工作表保存为 Excel 2003 格式的 Excel 文件。 |
| [saveToExcelFile(String targetFile, GridSaveOptions saveOptions)](#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-) | 将工作表保存到 Excel 文件。 |
| [saveToExcelFile(String targetFile, int format)](#saveToExcelFile-java.lang.String-int-) | 将工作表保存到 Excel 文件。 |
| [setACWClientPath(String value)](#setACWClientPath-java.lang.String-) | 设置控件的脚本/图像文件的 Web 路径。 |
| [setACWLanguageFileUrl(String value)](#setACWLanguageFileUrl-java.lang.String-) | 设置控件的语言文件的 Web URL。 |
| [setActiveCell(GridCell value)](#setActiveCell-com.aspose.gridweb.GridCell-) | 设置当前工作表的活动单元格。 |
| [setActiveCellBgColor(Color value)](#setActiveCellBgColor-com.aspose.gridweb.Color-) | 指定活动单元格的背景颜色。 |
| [setActiveCellColor(Color value)](#setActiveCellColor-com.aspose.gridweb.Color-) | 指定活动单元格的颜色。 |
| [setActiveHeaderBgColor(Color value)](#setActiveHeaderBgColor-com.aspose.gridweb.Color-) | 指定活动行/列标题的背景颜色。 |
| [setActiveHeaderColor(Color value)](#setActiveHeaderColor-com.aspose.gridweb.Color-) | 指定活动行/列标题的颜色。 |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | 设置活动工作表索引。 |
| [setActiveTabStyle(GridTableItemStyle value)](#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-) | 指定活动标签页的样式。 |
| [setAutoRefreshChart(boolean value)](#setAutoRefreshChart-boolean-) | 设置在更新单元格值时是否更新图表图像，默认值为 true。 |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | 在 WebControl 中设置 BackColor |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | 在 WebControl 中设置 BorderColor |
| [setBorderStyle(int value)](#setBorderStyle-int-) | 在 WebControl 中设置 BorderStyle |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | 在 WebControl 中设置 BorderWidth |
| [setBottomTableStyle(GridTableStyle value)](#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-) | 设置控件底部栏的样式。 |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | 设置是在单元格值更改后还是在导入文件后计算公式。 |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | 在 WebControl 中设置 CssClass |
| [setCurrentPageIndex(int value)](#setCurrentPageIndex-int-) | 设置分页模式下的当前页索引。 |
| [setCustomCalculationEngine(GridAbstractCalculationEngine value)](#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-) | 表示用户的自定义计算引擎，用于扩展 Aspose.Cells 的默认计算引擎。 |
| [setCustomStyle(InputStream stream)](#setCustomStyle-java.io.InputStream-) | 从流（包括磁盘文件流或内存流）设置自定义样式文件。 |
| [setCustomStyleFileName(String value)](#setCustomStyleFileName-java.lang.String-) | 设置自定义样式文件名。 |
| [setDPI(double value)](#setDPI-double-) | 获取/设置机器的 DPI。 |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | 设置控件的默认字体名称。 |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | 设置控件的默认字体大小。 |
| [setDefaultGridLineColor(Color value)](#setDefaultGridLineColor-com.aspose.gridweb.Color-) | 设置默认网格线的颜色。 |
| [setDisplayCellTip(boolean value)](#setDisplayCellTip-boolean-) | 设置是否显示提示，默认值为 true。 |
| [setEditMode(boolean value)](#setEditMode-boolean-) | 设置控件的编辑模式。 |
| [setEnableAJAX(boolean value)](#setEnableAJAX-boolean-) | 设置是否使用 AJAX 调用，默认值为 true。 |
| [setEnableAsync(boolean value)](#setEnableAsync-boolean-) | 设置是否以异步方式加载单元格数据，建议在单个工作表超过 10000 个单元格时使用。 |
| [setEnableClientColumnOperations(boolean value)](#setEnableClientColumnOperations-boolean-) | 设置是否启用客户端列操作。 |
| [setEnableClientFreeze(boolean value)](#setEnableClientFreeze-boolean-) | 设置是否启用客户端冻结操作。 |
| [setEnableClientMergeOperations(boolean value)](#setEnableClientMergeOperations-boolean-) | 设置是否启用客户端合并操作。 |
| [setEnableClientResizeColumnRow(boolean value)](#setEnableClientResizeColumnRow-boolean-) | 设置是否启用客户端列和行的大小调整。 |
| [setEnableClientRowOperations(boolean value)](#setEnableClientRowOperations-boolean-) | 设置是否启用客户端行操作。 |
| [setEnableDoubleClickEvent(boolean value)](#setEnableDoubleClickEvent-boolean-) | 设置是否启用客户侧双击事件。 |
| [setEnableMetalLightEffect(boolean value)](#setEnableMetalLightEffect-boolean-) | 设置是否应用金属光效。 |
| [setEnablePaging(boolean value)](#setEnablePaging-boolean-) | 设置是否启用控件的分页模式。 |
| [setEnableStyleDialogbox(boolean value)](#setEnableStyleDialogbox-boolean-) | 设置是否启用客户端样式对话框。 |
| [setEnabled(boolean value)](#setEnabled-boolean-) | 在 WebControl 中设置 Enabled |
| [setFilteredPaging(boolean value)](#setFilteredPaging-boolean-) | 设置在数据过滤后是否启用分页，EnablePaging 为 true 时生效。 |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | 设置字体文件夹 |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | 设置字体文件夹 |
| [setForceValidation(boolean value)](#setForceValidation-boolean-) | 设置是否强制客户侧验证。 |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | 在 WebControl 中设置 ForeColor |
| [setFrameTableStyle(GridTableStyle value)](#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-) | 设置控件的框架样式。 |
| [setGoonDefaultSaveOperation(boolean value)](#setGoonDefaultSaveOperation-boolean-) | 设置 GridWeb 是否执行默认保存操作，默认值为 true。 |
| [setHeaderBarHeight(Unit value)](#setHeaderBarHeight-com.aspose.gridweb.Unit-) | 设置控件顶部标题栏的高度（System.Web.UI.WebControl.Unit）。 |
| [setHeaderBarStyle(GridTableItemStyle value)](#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-) | 设置标题栏的样式。 |
| [setHeaderBarTableStyle(GridTableStyle value)](#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-) | 设置控件标题栏的样式。 |
| [setHeaderBarWidth(Unit value)](#setHeaderBarWidth-com.aspose.gridweb.Unit-) | 设置控件左侧标题栏的宽度（System.Web.UI.WebControl.Unit）。 |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | 设置控件的高度（System.Web.UI.WebControl.Unit）。 |
| [setIgnoreStyleWithNoData(boolean value)](#setIgnoreStyleWithNoData-boolean-) | 设置 GridWeb 是否忽略显示没有单元格值但仍具有样式的行或列。 |
| [setLoadOptions(GridLoadOptions value)](#setLoadOptions-com.aspose.gridweb.GridLoadOptions-) | 表示 GridWeb 的加载选项。 |
| [setMaxColumn(int value)](#setMaxColumn-int-) | 设置网页工作表的最大显示列索引（从零开始）。 |
| [setMaxRow(int value)](#setMaxRow-int-) | 设置网页工作表的最大显示行索引（从零开始）。 |
| [setMessage(String value)](#setMessage-java.lang.String-) | 设置网格的消息。 |
| [setMinColumn(int value)](#setMinColumn-int-) | 设置网页工作表的最小显示列索引（从零开始）。 |
| [setMinRow(int value)](#setMinRow-int-) | 设置网页工作表的最小显示行索引（从零开始）。 |
| [setNeedRenderGroupRows(boolean value)](#setNeedRenderGroupRows-boolean-) | 设置是否显示分组行。 |
| [setNoHScroll(boolean value)](#setNoHScroll-boolean-) | 设置一个值，指示水平滚动条是否隐藏。 |
| [setNoScroll(boolean value)](#setNoScroll-boolean-) | 设置是否显示滚动条。 |
| [setNoVScroll(boolean value)](#setNoVScroll-boolean-) | 设置一个值，指示垂直滚动条是否隐藏。 |
| [setOnAjaxCallFinishedClientFunction(String value)](#setOnAjaxCallFinishedClientFunction-java.lang.String-) | 设置 AJAX 调用完成时要调用的客户端函数名称。 |
| [setOnCellErrorClientFunction(String value)](#setOnCellErrorClientFunction-java.lang.String-) | 设置单元格验证失败时要调用的客户端函数名称。 |
| [setOnCellSelectedAjaxCallBackClientFunction(String value)](#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-) | 设置选中单元格时要调用的客户端函数。 |
| [setOnCellSelectedClientFunction(String value)](#setOnCellSelectedClientFunction-java.lang.String-) | 设置选中单元格时要调用的客户端函数。 |
| [setOnCellUnselectedClientFunction(String value)](#setOnCellUnselectedClientFunction-java.lang.String-) | 设置取消选中单元格时要调用的客户端函数。 |
| [setOnCellUpdatedClientFunction(String value)](#setOnCellUpdatedClientFunction-java.lang.String-) | 设置单元格值更新时要调用的客户端函数名称。 |
| [setOnContextMenuShowClientFunction(String value)](#setOnContextMenuShowClientFunction-java.lang.String-) | 设置将显示上下文菜单时要调用的客户端函数。 |
| [setOnDoubleClickCellClientFunction(String value)](#setOnDoubleClickCellClientFunction-java.lang.String-) | 设置双击单元格时要调用的客户端函数。 |
| [setOnDoubleClickRowClientFunction(String value)](#setOnDoubleClickRowClientFunction-java.lang.String-) | 设置双击行时要调用的客户端函数。 |
| [setOnGridInitClientFunction(String value)](#setOnGridInitClientFunction-java.lang.String-) | 设置网格初始化时要调用的客户端函数名称。 |
| [setOnPageChangeClientFunction(String value)](#setOnPageChangeClientFunction-java.lang.String-) | 设置在页面索引更改后调用的客户端函数。仅在 EnablePaging 为 true 时生效。 |
| [setOnPageSubmitClientFunction(String value)](#setOnPageSubmitClientFunction-java.lang.String-) | 设置在页面提交前在客户端调用的函数。 |
| [setOnShapeSelectedClientFunction(String value)](#setOnShapeSelectedClientFunction-java.lang.String-) | 设置在选择形状时调用的客户端函数。 |
| [setOnSubmitClientFunction(String value)](#setOnSubmitClientFunction-java.lang.String-) | 设置在控件提交前在客户端调用的函数。 |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | 设置是否仅适配高度未自定义的行，默认值为 false。 |
| [setPageSize(int value)](#setPageSize-int-) | 设置分页模式下的页面大小。 |
| [setPictureCachePath(String value)](#setPictureCachePath-java.lang.String-) | 设置工作簿的图像存储路径，所有形状和图像将存储在此目录中，默认路径为当前应用程序基目录下的 acwcache，用户需要实现计划服务来清理会话超时的文件。 |
| [setPresetStyle(int value)](#setPresetStyle-int-) | 设置预设样式。 |
| [setRefreshValidation(boolean value)](#setRefreshValidation-boolean-) | 设置在单元格值更改后是否刷新验证值。 |
| [setRenderHiddenRow(boolean value)](#setRenderHiddenRow-boolean-) | 设置在 GridControl 中是否渲染隐藏行，默认值为 false。 |
| [setRowHeightForCSV(double value)](#setRowHeightForCSV-double-) | 设置 CSV 文件的行高（单位为点），默认值为 14.5。 |
| [setScrollBarArrowColor(Color value)](#setScrollBarArrowColor-com.aspose.gridweb.Color-) | 指定滚动条箭头按钮的颜色。 |
| [setScrollBarBaseColor(Color value)](#setScrollBarBaseColor-com.aspose.gridweb.Color-) | 指定控件滚动条的颜色。 |
| [setSelectCellBgColor(Color value)](#setSelectCellBgColor-com.aspose.gridweb.Color-) | 指定多选范围内已选单元格的背景颜色。 |
| [setSelectCellColor(Color value)](#setSelectCellColor-com.aspose.gridweb.Color-) | 指定多选范围内已选单元格的颜色。 |
| [setSessionStorePath(String value)](#setSessionStorePath-java.lang.String-) | 设置会话模式为 File 或 ViewState 时的会话缓存存储路径，例如：gridweb.SessionStorePath="c:/mytempdir/session"；则会将会话数据存储在 c:/mytempdir/session。 |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridweb.GridWorkbookSettings-) | 表示工作簿设置。 |
| [setShowAddButton(boolean value)](#setShowAddButton-boolean-) | 设置是否显示添加工作表按钮。 |
| [setShowBottomBar(boolean value)](#setShowBottomBar-boolean-) | 指定是否在控件底部显示命令栏（包括命令栏和标签栏）。 |
| [setShowCellEditBox(boolean value)](#setShowCellEditBox-boolean-) | 是否在 Gridweb 中显示类似 MS-EXCEL 的编辑框工具栏。启用后，将在 Gridweb 中显示当前单元格的编辑框。 |
| [setShowCommandBarAtTop(boolean value)](#setShowCommandBarAtTop-boolean-) | 指定是否在控件顶部显示命令栏（包括命令栏和标签栏）。 |
| [setShowContextMenu(boolean value)](#setShowContextMenu-boolean-) | 设置是否显示上下文菜单，默认值为 true。 |
| [setShowDefaultGridLine(boolean value)](#setShowDefaultGridLine-boolean-) | 设置是否显示单元格的默认网格线。 |
| [setShowHeaderBar(boolean value)](#setShowHeaderBar-boolean-) | 设置是否显示标题栏。 |
| [setShowLoading(boolean value)](#setShowLoading-boolean-) | 指定在回发到服务器期间是否显示加载对话框。 |
| [setShowLoadingPosition(String value)](#setShowLoadingPosition-java.lang.String-) | 指定在回发到服务器期间显示加载对话框的左、上位置（单位为像素），例如 100,200 表示加载对话框的左、上位置分别为 100px 和 200px。 |
| [setShowSaveButton(boolean value)](#setShowSaveButton-boolean-) | 设置是否显示保存按钮。 |
| [setShowSubmitButton(boolean value)](#setShowSubmitButton-boolean-) | 设置是否显示提交按钮。 |
| [setShowTabBar(boolean value)](#setShowTabBar-boolean-) | 设置是否显示选项卡栏。 |
| [setShowTabNavigation(boolean value)](#setShowTabNavigation-boolean-) | 设置是否显示选项卡导航按钮，默认值为 true。 |
| [setShowUndoButton(boolean value)](#setShowUndoButton-boolean-) | 设置是否显示撤销按钮。 |
| [setSpanWrap(boolean value)](#setSpanWrap-boolean-) | 指定是否在单元格跨越范围内换行内容，默认值为 true。 |
| [setTabIndex(short value)](#setTabIndex-short-) | 在 WebControl 中设置 TabIndex |
| [setTabStyle(GridTableItemStyle value)](#setTabStyle-com.aspose.gridweb.GridTableItemStyle-) | 设置选项卡栏的样式。 |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | 在 WebControl 中设置 ToolTip |
| [setUseClientPageHeight(boolean value)](#setUseClientPageHeight-boolean-) | 设置 gridweb 是否使用客户端页面高度作为控件高度，适用于将 Height="100%" 的情况，默认值为 false。 |
| [setViewPanelScrollLeft(String value)](#setViewPanelScrollLeft-java.lang.String-) | 设置网格视图面板滚动条的位置。 |
| [setViewPanelScrollTop(String value)](#setViewPanelScrollTop-java.lang.String-) | 设置网格视图面板滚动条的位置。 |
| [setViewTableStyle(GridTableStyle value)](#setViewTableStyle-com.aspose.gridweb.GridTableStyle-) | 设置数据视图面板的样式。 |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | 设置控件的宽度( System.Web.UI.WebControl.Unit )。 |
| [setXhtmlMode(boolean value)](#setXhtmlMode-boolean-) | 设置是否使用 XHTML 样式，默认值为 true。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWeb() {#GridWeb--}
```
public GridWeb()
```


### AfterColumnFilter {#AfterColumnFilter}
```
public RowColumnEventHandler AfterColumnFilter
```


在列过滤后发生。

### AjaxCallFinished {#AjaxCallFinished}
```
public WorkbookEventHandler AjaxCallFinished
```


当控件的 ajax 更新完成时触发。(EnableAJAX 应设置为 true)

### BeforeColumnFilter {#BeforeColumnFilter}
```
public RowColumnEventHandler BeforeColumnFilter
```


在列过滤之前发生。

### CellClickOnAjax {#CellClickOnAjax}
```
public CellEventStringHandler CellClickOnAjax
```


当单元格被点击时发生，并且需要为此事件执行 ajax 回调。

### CellClientUpdate {#CellClientUpdate}
```
public CellEventHandler CellClientUpdate
```


当客户端单元格更新发生时触发。当此事件被触发时，其参数 e.Argument 包含命令的名称。

### CellCommand {#CellCommand}
```
public CellEventHandler CellCommand
```


当单元格的命令超链接被点击时触发。当此事件被触发时，其参数 e.Argument 包含命令的名称。

### CellDoubleClick {#CellDoubleClick}
```
public CellEventHandler CellDoubleClick
```


当单元格被双击时发生。

### CellModifiedOnAjax {#CellModifiedOnAjax}
```
public CellEventHandler CellModifiedOnAjax
```


当单元格在 ajax 调用中被修改时发生。

### ColumnDeleted {#ColumnDeleted}
```
public RowColumnEventHandler ColumnDeleted
```


当用户从客户端菜单删除列时发生。

### ColumnDeleting {#ColumnDeleting}
```
public RowColumnEventHandler ColumnDeleting
```


当用户尝试从客户端菜单删除列时触发。您可以处理此事件并将 cancel 参数设为 True，以取消删除操作。

### ColumnDoubleClick {#ColumnDoubleClick}
```
public RowColumnEventHandler ColumnDoubleClick
```


当列标题被双击时发生。

### ColumnInserted {#ColumnInserted}
```
public RowColumnEventHandler ColumnInserted
```


当用户从客户端菜单插入列时发生。

### CustomCommand {#CustomCommand}
```
public CustomCommandEventHandler CustomCommand
```


当用户点击自定义命令按钮时发生。

### LoadCustomData {#LoadCustomData}
```
public WorkbookEventHandler LoadCustomData
```


当控件的 SessionMode 设置为 Custom 并需要加载工作表数据时触发。您可以在自定义会话模式下处理此事件，以从文件或数据库加载工作表数据。

### PageIndexChanged {#PageIndexChanged}
```
public WorkbookEventHandler PageIndexChanged
```


当控件的工作表页面索引更改时发生。

### RowDeleted {#RowDeleted}
```
public RowColumnEventHandler RowDeleted
```


当用户已从客户端菜单删除行时发生。

### RowDeleting {#RowDeleting}
```
public RowColumnEventHandler RowDeleting
```


当用户尝试从客户端菜单删除行时触发。您可以处理此事件并抛出 RejectDeleteException 异常以取消删除操作。

### RowDoubleClick {#RowDoubleClick}
```
public RowColumnEventHandler RowDoubleClick
```


当行标题被双击时发生。

### RowInserted {#RowInserted}
```
public RowColumnEventHandler RowInserted
```


当用户从客户端菜单插入行时发生。

### SaveCommand {#SaveCommand}
```
public WorkbookEventHandler SaveCommand
```


当点击 "save" 按钮时发生。

### SheetAdded {#SheetAdded}
```
public SheetEventHandler SheetAdded
```


当用户从工具栏菜单添加工作表时发生。

### SheetTabClick {#SheetTabClick}
```
public WorkbookEventHandler SheetTabClick
```


当工作表标签被点击时发生。

### SubmitCommand {#SubmitCommand}
```
public WorkbookEventHandler SubmitCommand
```


当单击 \"submit\" 按钮时发生。

### UndoCommand {#UndoCommand}
```
public WorkbookEventHandler UndoCommand
```


当单击 \"undo\" 按钮时发生。

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


计算公式的结果。

### createChildControls() {#createChildControls--}
```
public void createChildControls()
```


实现来自 WebControl 的 CreateChildControls，仅供内部使用。

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getACWClientPath() {#getACWClientPath--}
```
public String getACWClientPath()
```


获取控件脚本/图像文件的 Web 路径。例如："http://localhost/acw\\_client"。您也可以在 web.config 文件中设置此值。将此节添加到 `<configuration>` 节中：
`<appSettings>`
`<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />`
`</appSettings>`


**Returns:**
java.lang.String
### getACWLanguageFileUrl() {#getACWLanguageFileUrl--}
```
public String getACWLanguageFileUrl()
```


获取控件语言文件的 Web URL。例如："/acw\\_client/lang\\_en.js"。
默认情况下，使用内置的英文文件。


**Returns:**
java.lang.String
### getActiveCell() {#getActiveCell--}
```
public GridCell getActiveCell()
```


获取当前工作表的活动单元格。自 1.9.0.1 版本起已改为可写。

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getActiveCellBgColor() {#getActiveCellBgColor--}
```
public Color getActiveCellBgColor()
```


指定活动单元格的背景颜色。

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveCellColor() {#getActiveCellColor--}
```
public Color getActiveCellColor()
```


指定活动单元格的颜色。

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderBgColor() {#getActiveHeaderBgColor--}
```
public Color getActiveHeaderBgColor()
```


指定活动行/列标题的背景颜色。

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderColor() {#getActiveHeaderColor--}
```
public Color getActiveHeaderColor()
```


指定活动行/列标题的颜色。

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveSheet() {#getActiveSheet--}
```
public GridWorksheet getActiveSheet()
```


获取活动工作表

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


获取活动工作表的索引。等于 WebWorksheets.ActiveSheetIndex。

**Returns:**
int
### getActiveTabStyle() {#getActiveTabStyle--}
```
public GridTableItemStyle getActiveTabStyle()
```


指定活动标签页的样式。

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getAutoRefreshChart() {#getAutoRefreshChart--}
```
public boolean getAutoRefreshChart()
```


获取在更新单元格值时是否更新图表图像。默认值为 true。

**Returns:**
boolean
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


获取 WebControl 中的 BackColor

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```


获取 WebControl 中的 BorderColor

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


获取 WebControl 中的 BorderStyle

参见 [BorderStyle](../../com.aspose.gridweb/borderstyle)。

**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```


获取 WebControl 中的 BorderWidth

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomTableStyle() {#getBottomTableStyle--}
```
public GridTableStyle getBottomTableStyle()
```


获取控件底部栏的样式。

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


获取 WebControl 中的 CssClass

**Returns:**
java.lang.String
### getCurrentPageIndex() {#getCurrentPageIndex--}
```
public int getCurrentPageIndex()
```


获取分页模式下的当前页索引。

**Remarks**

在分页模式下，控件一次显示 PageSize 行数据，并在选项卡栏中显示页面选择控件。

**Returns:**
int
### getCustomCalculationEngine() {#getCustomCalculationEngine--}
```
public GridAbstractCalculationEngine getCustomCalculationEngine()
```


表示用户的自定义计算引擎，用于扩展 Aspose.Cells 的默认计算引擎。

**Returns:**
[GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine)
### getCustomCommandButtons() {#getCustomCommandButtons--}
```
public CustomCommandButtonCollection getCustomCommandButtons()
```


获取自定义命令按钮集合。

**Returns:**
[CustomCommandButtonCollection](../../com.aspose.gridweb/customcommandbuttoncollection)
### getCustomStyleFileName() {#getCustomStyleFileName--}
```
public String getCustomStyleFileName()
```


获取自定义样式文件名。

**Remarks**

自定义样式文件是 XML 文件。当设置文件名时，文件将立即加载。这里是 "standard preset style" 的内容 ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

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


获取/设置机器的 DPI。

**Remarks**

**Returns:**
double
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


获取控件的默认字体名称。

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


获取控件的默认字体大小。

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


获取默认网格线的颜色。

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


获取是否显示提示。默认值为 true。

**Returns:**
boolean
### getEditMode() {#getEditMode--}
```
public boolean getEditMode()
```


获取控件的编辑模式。

**Remarks**

当设置为 true 时，控件的单元格可编辑，并显示 "save" 和 "undo" 图标。当设置为 false 时，控件的单元格为只读，并且不显示 "save" 和 "undo" 图标。

**Returns:**
boolean
### getEnableAJAX() {#getEnableAJAX--}
```
public boolean getEnableAJAX()
```


获取是否使用 AJAX 调用。默认值为 true。

**Returns:**
boolean
### getEnableAsync() {#getEnableAsync--}
```
public boolean getEnableAsync()
```


获取是否以异步方式加载单元格数据，建议在单个工作表超过 10000 个单元格时使用。

**Returns:**
boolean
### getEnableClientColumnOperations() {#getEnableClientColumnOperations--}
```
public boolean getEnableClientColumnOperations()
```


获取是否启用客户端列操作。

**Remarks**

当设置为 true 时，用户可以使用右键菜单添加/删除列。

**Returns:**
boolean
### getEnableClientFreeze() {#getEnableClientFreeze--}
```
public boolean getEnableClientFreeze()
```


获取是否启用客户端冻结操作。

**Remarks**

当设置为 true 时，用户可以使用右键菜单冻结/取消冻结窗格。

**Returns:**
boolean
### getEnableClientMergeOperations() {#getEnableClientMergeOperations--}
```
public boolean getEnableClientMergeOperations()
```


获取是否启用客户端合并操作。

**Remarks**

当设置为 true 时，用户可以使用右键菜单合并/拆分单元格。

**Returns:**
boolean
### getEnableClientResizeColumnRow() {#getEnableClientResizeColumnRow--}
```
public boolean getEnableClientResizeColumnRow()
```


获取是否启用客户端列和行的大小调整。

**Remarks**

当设置为 true 时，用户可以在客户端调整列和行的大小。

**Returns:**
boolean
### getEnableClientRowOperations() {#getEnableClientRowOperations--}
```
public boolean getEnableClientRowOperations()
```


获取是否启用客户端行操作。

**Remarks**

当设置为 true 时，用户可以使用右键菜单添加/删除行。

**Returns:**
boolean
### getEnableDoubleClickEvent() {#getEnableDoubleClickEvent--}
```
public boolean getEnableDoubleClickEvent()
```


获取是否启用客户侧双击事件。

**Remarks**

当设置为 true 时，控件将接收客户端双击事件，您可以在服务器端处理这些事件。否则，控件将忽略所有双击事件。

**Returns:**
boolean
### getEnableMetalLightEffect() {#getEnableMetalLightEffect--}
```
public boolean getEnableMetalLightEffect()
```


获取是否应用金属光效。

**Returns:**
boolean
### getEnablePaging() {#getEnablePaging--}
```
public boolean getEnablePaging()
```


获取是否启用控件的分页模式。

**Remarks**

当设置为 true 时，控件一次显示 PageSize 行数据，并在选项卡栏中显示页面选择控件。

**Returns:**
boolean
### getEnableStyleDialogbox() {#getEnableStyleDialogbox--}
```
public boolean getEnableStyleDialogbox()
```


获取是否启用客户端样式对话框。

**Remarks**

当设置为 true 时，用户可以通过在弹出菜单中选择 "Format Cell..." 来使用样式对话框设置单元格的样式。

**Returns:**
boolean
### getEnabled() {#getEnabled--}
```
public boolean getEnabled()
```


获取 WebControl 中的 Enabled

**Returns:**
boolean
### getFilteredPaging() {#getFilteredPaging--}
```
public boolean getFilteredPaging()
```


获取在数据过滤后是否启用分页，EnablePaging 为 true 时生效。

**Remarks**

当设置为 true 时，控件将基于过滤后的数据进行分页，默认值为 false。

**Returns:**
boolean
### getFont() {#getFont--}
```
public FontInfo getFont()
```


获取 WebControl 中的 Font

**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForceValidation() {#getForceValidation--}
```
public boolean getForceValidation()
```


获取是否强制客户侧验证。

**Remarks**

当设置为 true 时，数据将在所有输入字段有效之前不会提交到服务器。

**Returns:**
boolean
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


获取 WebControl 中的 ForeColor

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getFrameTableStyle() {#getFrameTableStyle--}
```
public GridTableStyle getFrameTableStyle()
```


获取控件的框架样式。

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getGoonDefaultSaveOperation() {#getGoonDefaultSaveOperation--}
```
public boolean getGoonDefaultSaveOperation()
```


获取 GridWeb 是否执行默认保存操作，默认值为 true。

**Returns:**
boolean
### getHeaderBarHeight() {#getHeaderBarHeight--}
```
public Unit getHeaderBarHeight()
```


获取控件顶部标题栏的高度（System.Web.UI.WebControl.Unit）。

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


获取标题栏的样式。

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getHeaderBarTableStyle() {#getHeaderBarTableStyle--}
```
public GridTableStyle getHeaderBarTableStyle()
```


获取控件标题栏的样式。

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getHeaderBarWidth() {#getHeaderBarWidth--}
```
public Unit getHeaderBarWidth()
```


获取控件左侧标题栏的宽度（System.Web.UI.WebControl.Unit）。

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


获取控件的高度（System.Web.UI.WebControl.Unit）。

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


获取 GridWeb 是否忽略显示没有单元格值但仍有样式的行或列。如果设置为 true，性能会更好。默认值为 false，这意味着如果最后连续的行/列没有单元格值但有样式，我们仍会显示它们。此选项仅在 EnableAsync 为 false 时有效。当 EnableAsync 为 true 时此选项无效，这意味着 GridWeb 将显示所有带样式的行/列。

**Returns:**
boolean
### getLoadOptions() {#getLoadOptions--}
```
public GridLoadOptions getLoadOptions()
```


表示 GridWeb 的加载选项。

**Returns:**
[GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


获取网页工作表的最大显示列索引（从零开始）。控件使用 MaxColumn 与工作表数据的最大列之间的较大值。

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


获取网页工作表的最大显示行索引（从零开始）。控件使用 MaxRow 与工作表数据的最大行之间的较大值。

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


获取网格的消息。

**Returns:**
java.lang.String
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


获取网页工作表的最小显示列索引（从零开始）。控件使用 MinColumn 与工作表数据的最小列之间的较小值。

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


获取网页工作表的最小显示行索引（从零开始）。控件使用 MinRow 与工作表数据的最小行之间的较小值。

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


获取由客户端修改的单元格集合。

**Returns:**
java.util.ArrayList
### getNeedRenderGroupRows() {#getNeedRenderGroupRows--}
```
public boolean getNeedRenderGroupRows()
```


获取是否显示组行。

**Returns:**
boolean
### getNoHScroll() {#getNoHScroll--}
```
public boolean getNoHScroll()
```


获取指示水平滚动条是否隐藏的值。

**Returns:**
boolean
### getNoScroll() {#getNoScroll--}
```
public boolean getNoScroll()
```


获取是否显示滚动条。

**Returns:**
boolean
### getNoVScroll() {#getNoVScroll--}
```
public boolean getNoVScroll()
```


获取指示垂直滚动条是否隐藏的值。

**Returns:**
boolean
### getOnAjaxCallFinishedClientFunction() {#getOnAjaxCallFinishedClientFunction--}
```
public String getOnAjaxCallFinishedClientFunction()
```


获取在 ajaxcall 完成时调用的客户端函数名称。客户端函数应按如下方式声明：
function GridAjaxcallFinished()
\{
alert(this.id+" ajaxcall finished ");
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Returns:**
java.lang.String
### getOnCellErrorClientFunction() {#getOnCellErrorClientFunction--}
```
public String getOnCellErrorClientFunction()
```


获取在单元格验证失败时调用的客户端函数名称。客户端函数应按如下方式声明：
function MyOnCellError(cell)
\{
alert(this.getCellValueByCell(cell));
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Returns:**
java.lang.String
### getOnCellSelectedAjaxCallBackClientFunction() {#getOnCellSelectedAjaxCallBackClientFunction--}
```
public String getOnCellSelectedAjaxCallBackClientFunction()
```


获取在单元格被选中时调用的客户端函数。客户端函数应按如下方式声明：
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\{

\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Returns:**
java.lang.String
### getOnCellSelectedClientFunction() {#getOnCellSelectedClientFunction--}
```
public String getOnCellSelectedClientFunction()
```


获取在单元格被选中时调用的客户端函数。客户端函数应按如下方式声明：
function MyOnSelectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, "test");
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Returns:**
java.lang.String
### getOnCellUnselectedClientFunction() {#getOnCellUnselectedClientFunction--}
```
public String getOnCellUnselectedClientFunction()
```


获取在单元格被取消选中时调用的客户端函数。客户端函数应按如下方式声明：
function MyOnUnselectCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Returns:**
java.lang.String
### getOnCellUpdatedClientFunction() {#getOnCellUpdatedClientFunction--}
```
public String getOnCellUpdatedClientFunction()
```


获取在单元格的值被更新时调用的客户端函数名称。客户端函数应按如下方式声明：
function MyOnCellUpdated(cell)
\{
alert(this.getCellValueByCell(cell));
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Returns:**
java.lang.String
### getOnContextMenuShowClientFunction() {#getOnContextMenuShowClientFunction--}
```
public String getOnContextMenuShowClientFunction()
```


获取在上下文菜单将显示时调用的客户端函数。客户端函数应按如下方式声明：
function onContextMenuShow()
\{
var menu = event.srcElement;
menu.setItemVisibility("Delete", "block");
menu.setItemVisibility("Update", "none");
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Returns:**
java.lang.String
### getOnDoubleClickCellClientFunction() {#getOnDoubleClickCellClientFunction--}
```
public String getOnDoubleClickCellClientFunction()
```


获取在单元格双击时要调用的客户端函数。客户端函数应如下声明：
function MyOnDoubleClickCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Returns:**
java.lang.String
### getOnDoubleClickRowClientFunction() {#getOnDoubleClickRowClientFunction--}
```
public String getOnDoubleClickRowClientFunction()
```


获取在行双击时要调用的客户端函数。客户端函数应如下声明：
function MyOnRowDoubleClick(row)
\{
alert(row);
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Returns:**
java.lang.String
### getOnGridInitClientFunction() {#getOnGridInitClientFunction--}
```
public String getOnGridInitClientFunction()
```


获取在网格初始化时要调用的客户端函数名称。客户端函数应如下声明：
function MyOnGridInit(grid)
\{
alert("网格已初始化: " + grid.id);
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Returns:**
java.lang.String
### getOnPageChangeClientFunction() {#getOnPageChangeClientFunction--}
```
public String getOnPageChangeClientFunction()
```


获取在页面索引更改后要调用的客户端函数。仅在 EnablePaging 为 true 时生效。客户端函数应如下声明：
function MyOnPageChange(index)
\{
console.log("当前页面是:"+index);
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Returns:**
java.lang.String
### getOnPageSubmitClientFunction() {#getOnPageSubmitClientFunction--}
```
public String getOnPageSubmitClientFunction()
```


获取在页面提交前要在客户端调用的函数。

**Returns:**
java.lang.String
### getOnShapeSelectedClientFunction() {#getOnShapeSelectedClientFunction--}
```
public String getOnShapeSelectedClientFunction()
```


获取在选择形状时要调用的客户端函数。客户端函数应如下声明：
function MyOnSelectShape(shape)
\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Returns:**
java.lang.String
### getOnSubmitClientFunction() {#getOnSubmitClientFunction--}
```
public String getOnSubmitClientFunction()
```


获取在客户端提交控件之前要调用的客户端函数。客户端函数应如下声明：
function MyOnSubmit(arg, cancelEdit)
\{
return true;
\}
arg 是提交参数，包含要发送到服务器的命令。cancelEdit 是布尔值，指示控件在提交前是否已丢弃用户输入。如果函数返回 true，控件将继续提交。
注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Returns:**
java.lang.String
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


获取是否仅适配高度未自定义的行，默认值为 false。

**Returns:**
boolean
### getPageSize() {#getPageSize--}
```
public int getPageSize()
```


获取分页模式下的页面大小。

**Remarks**

在分页模式下，控件一次显示 PageSize 行数据，并在选项卡栏中显示页面选择控件。

**Returns:**
int
### getPictureCachePath() {#getPictureCachePath--}
```
public static String getPictureCachePath()
```


获取工作簿的图像存储路径，所有形状和图像都将存储在此目录中，默认路径是当前应用程序基目录下的 acwcache，用户需要实现一个计划服务来清理超出会话时间的文件。

**Returns:**
java.lang.String
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


获取预设样式。

参见 [PresetStyle](../../com.aspose.gridweb/presetstyle)。

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


获取在单元格值更改后是否刷新验证值。

**Returns:**
boolean
### getRenderHiddenRow() {#getRenderHiddenRow--}
```
public boolean getRenderHiddenRow()
```


获取在 GridControl 中是否渲染隐藏行，默认值为 false。如果需要稍后取消隐藏隐藏行，应将其设置为 true。

**Returns:**
boolean
### getRowHeightForCSV() {#getRowHeightForCSV--}
```
public double getRowHeightForCSV()
```


获取 CSV 文件的行高（单位为点），默认值为 14.5。

**Returns:**
double
### getScrollBarArrowColor() {#getScrollBarArrowColor--}
```
public Color getScrollBarArrowColor()
```


指定滚动条箭头按钮的颜色。

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getScrollBarBaseColor() {#getScrollBarBaseColor--}
```
public Color getScrollBarBaseColor()
```


指定控件滚动条的颜色。

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellBgColor() {#getSelectCellBgColor--}
```
public Color getSelectCellBgColor()
```


指定多选范围内已选单元格的背景颜色。

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellColor() {#getSelectCellColor--}
```
public Color getSelectCellColor()
```


指定多选范围内已选单元格的颜色。

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCells() {#getSelectCells--}
```
public ArrayList getSelectCells()
```


获取已选单元格集合。

**Returns:**
java.util.ArrayList
### getSessionStorePath() {#getSessionStorePath--}
```
public String getSessionStorePath()
```


当会话模式为 File 或 ViewState 等时获取会话缓存存储路径，例如：gridweb.SessionStorePath="c:/mytempdir/session"；此时会将会话数据存储在 c:/mytempdir/session 中。

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


表示工作簿设置。

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings)
### getShowAddButton() {#getShowAddButton--}
```
public boolean getShowAddButton()
```


获取是否显示添加工作表按钮。

**Returns:**
boolean
### getShowBottomBar() {#getShowBottomBar--}
```
public boolean getShowBottomBar()
```


指定是否在控件底部显示命令栏（包括命令栏和标签栏）。

**Returns:**
boolean
### getShowCellEditBox() {#getShowCellEditBox--}
```
public boolean getShowCellEditBox()
```


是否在 Gridweb 中显示类似 MS-EXCEL 的编辑框工具栏。启用后，当前单元格的编辑框将在 Gridweb 中显示。如果启用此功能，需要在你的 aspx 文件中导入 jquery js 库以支持此新功能。所有最新的 jquery 版本均可。等。

**Returns:**
boolean
### getShowCommandBarAtTop() {#getShowCommandBarAtTop--}
```
public boolean getShowCommandBarAtTop()
```


指定是否在控件顶部显示命令栏（包括命令栏和标签栏）。

**Returns:**
boolean
### getShowContextMenu() {#getShowContextMenu--}
```
public boolean getShowContextMenu()
```


获取是否显示上下文菜单。默认值为 true。

**Returns:**
boolean
### getShowDefaultGridLine() {#getShowDefaultGridLine--}
```
public boolean getShowDefaultGridLine()
```


获取是否显示单元格的默认网格线。

**Returns:**
boolean
### getShowHeaderBar() {#getShowHeaderBar--}
```
public boolean getShowHeaderBar()
```


获取是否显示标题栏。

**Returns:**
boolean
### getShowLoading() {#getShowLoading--}
```
public boolean getShowLoading()
```


指定在回发到服务器期间是否显示加载对话框。

**Returns:**
boolean
### getShowLoadingPosition() {#getShowLoadingPosition--}
```
public String getShowLoadingPosition()
```


指定在回发到服务器期间显示加载对话框的左、上位置（单位为像素），例如 100,200 表示加载对话框的左、上位置分别为 100px 和 200px。

**Returns:**
java.lang.String
### getShowSaveButton() {#getShowSaveButton--}
```
public boolean getShowSaveButton()
```


获取是否显示保存按钮。

**Returns:**
boolean
### getShowSubmitButton() {#getShowSubmitButton--}
```
public boolean getShowSubmitButton()
```


获取是否显示提交按钮。

**Returns:**
boolean
### getShowTabBar() {#getShowTabBar--}
```
public boolean getShowTabBar()
```


获取是否显示标签栏。

**Returns:**
boolean
### getShowTabNavigation() {#getShowTabNavigation--}
```
public boolean getShowTabNavigation()
```


获取标签导航按钮是否显示，默认值为 true。

**Returns:**
boolean
### getShowUndoButton() {#getShowUndoButton--}
```
public boolean getShowUndoButton()
```


获取是否显示撤销按钮。

**Returns:**
boolean
### getSpanWrap() {#getSpanWrap--}
```
public boolean getSpanWrap()
```


指定是否在单元格跨越范围内换行内容，默认值为 true。

**Returns:**
boolean
### getTabIndex() {#getTabIndex--}
```
public short getTabIndex()
```


获取 WebControl 中的 TabIndex

**Returns:**
短
### getTabStyle() {#getTabStyle--}
```
public GridTableItemStyle getTabStyle()
```


获取标签栏的样式。

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


获取 WebControl 中的 ToolTip

**Returns:**
java.lang.String
### getUseClientPageHeight() {#getUseClientPageHeight--}
```
public boolean getUseClientPageHeight()
```


获取 Gridweb 是否使用客户端页面高度作为控件高度，适用于设置 Height="100%" 的情况，默认值为 false。

**Returns:**
boolean
### getVersion() {#getVersion--}
```
public static String getVersion()
```


获取发布版本。

**Returns:**
java.lang.String - 发布版本。
### getViewPanelScrollLeft() {#getViewPanelScrollLeft--}
```
public String getViewPanelScrollLeft()
```


获取网格视图面板滚动条的位置。

**Returns:**
java.lang.String
### getViewPanelScrollTop() {#getViewPanelScrollTop--}
```
public String getViewPanelScrollTop()
```


获取网格视图面板滚动条的位置。

**Returns:**
java.lang.String
### getViewTableStyle() {#getViewTableStyle--}
```
public GridTableStyle getViewTableStyle()
```


获取数据视图面板的样式。

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


获取控件的宽度（System.Web.UI.WebControl.Unit）。

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


获取工作表的集合。

**Returns:**
[GridWorksheetCollection](../../com.aspose.gridweb/gridworksheetcollection)
### getXhtmlMode() {#getXhtmlMode--}
```
public boolean getXhtmlMode()
```


获取是否使用 XHTML 样式，默认值为 true。

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


从 Excel 文件流导入，包括磁盘文件流或内存流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.InputStream | Excel 文件的流，包括磁盘文件流或内存流。 |

### importExcelFile(InputStream stream, String passwordtoOpen) {#importExcelFile-java.io.InputStream-java.lang.String-}
```
public void importExcelFile(InputStream stream, String passwordtoOpen)
```


从 Excel 文件流导入，包括磁盘文件流或内存流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.InputStream | Excel 文件的流，包括磁盘文件流或内存流。 |
| passwordtoOpen | java.lang.String | 用于打开已加密文件的打开密码。 |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


从 Excel 文件导入。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | Excel 文件的名称。 |

### importExcelFile(String fileName, String passwordtoOpen) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String fileName, String passwordtoOpen)
```


从 Excel 文件导入。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | Excel 文件的名称。 |
| passwordtoOpen | java.lang.String | 用于打开已加密文件的打开密码。 |

### isCalculateFormula() {#isCalculateFormula--}
```
public boolean isCalculateFormula()
```


获取在单元格值更改或导入文件后是否计算公式。默认值为 true。

**Returns:**
boolean
### loadCSVFile(InputStream stream) {#loadCSVFile-java.io.InputStream-}
```
public void loadCSVFile(InputStream stream)
```


从 CSV 文件流加载数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.InputStream | 文件流。 |

### loadCSVFile(String fileName) {#loadCSVFile-java.lang.String-}
```
public void loadCSVFile(String fileName)
```


从 CSV 文件加载数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 文件的名称。 |

### loadHTMLFile(InputStream stream) {#loadHTMLFile-java.io.InputStream-}
```
public void loadHTMLFile(InputStream stream)
```


从 HTML 文件流加载数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.InputStream | 文件流。 |

### loadHTMLFile(String fileName) {#loadHTMLFile-java.lang.String-}
```
public void loadHTMLFile(String fileName)
```


从 HTML 文件加载数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 文件的名称。 |

### loadSpreadSheetMLFile(InputStream stream) {#loadSpreadSheetMLFile-java.io.InputStream-}
```
public void loadSpreadSheetMLFile(InputStream stream)
```


从 SpreadSheetML 文件流加载数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.InputStream | 文件的流。 |

### loadSpreadSheetMLFile(String fileName) {#loadSpreadSheetMLFile-java.lang.String-}
```
public void loadSpreadSheetMLFile(String fileName)
```


从 SpreadSheetML 文件加载数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 文件的名称。 |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshChartShape() {#refreshChartShape--}
```
public void refreshChartShape()
```


刷新活动工作表的所有图表图像。

### saveCSVFile(OutputStream stream) {#saveCSVFile-java.io.OutputStream-}
```
public void saveCSVFile(OutputStream stream)
```


将数据保存到 CSV 文件流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 文件流。 |

### saveCSVFile(String targetFile) {#saveCSVFile-java.lang.String-}
```
public void saveCSVFile(String targetFile)
```


将数据保存到 CSV 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| targetFile | java.lang.String | 文件的名称。 |

### saveCustomStyleFile(String fileName) {#saveCustomStyleFile-java.lang.String-}
```
public void saveCustomStyleFile(String fileName)
```


将控件的当前样式数据保存到 xml 文件。可用于创建自定义样式文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 样式文件的名称。 |

### saveHTMLFile(OutputStream stream) {#saveHTMLFile-java.io.OutputStream-}
```
public void saveHTMLFile(OutputStream stream)
```


将数据保存到 HTML 文件流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 文件流。 |

### saveHTMLFile(String targetFile) {#saveHTMLFile-java.lang.String-}
```
public void saveHTMLFile(String targetFile)
```


将数据保存到 HTML 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| targetFile | java.lang.String | 文件的名称。 |

### saveSpreadSheetMLFile(OutputStream stream) {#saveSpreadSheetMLFile-java.io.OutputStream-}
```
public void saveSpreadSheetMLFile(OutputStream stream)
```


将数据保存到 SpreadSheetML 文件流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 文件流。 |

### saveSpreadSheetMLFile(String targetFile) {#saveSpreadSheetMLFile-java.lang.String-}
```
public void saveSpreadSheetMLFile(String targetFile)
```


将数据保存到 SpreadSheetML 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| targetFile | java.lang.String | 文件的名称。 |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


将工作表保存到 Excel 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 写入的流。 |

### saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions) {#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)
```


将工作表保存到 Excel 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 写入的流。 |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | 保存选项。 |

### saveToExcelFile(OutputStream stream, int format) {#saveToExcelFile-java.io.OutputStream-int-}
```
public void saveToExcelFile(OutputStream stream, int format)
```


将工作表保存到 Excel 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.OutputStream | 写入的流。 |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat)。文件格式（Excel2003、Excel2007、CSV、SpreadsheetML） |

### saveToExcelFile(String targetFile) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String targetFile)
```


将工作表保存为 Excel 2003 格式的 Excel 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| targetFile | java.lang.String | 写入的目标文件名称。 |

### saveToExcelFile(String targetFile, GridSaveOptions saveOptions) {#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(String targetFile, GridSaveOptions saveOptions)
```


将工作表保存到 Excel 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| targetFile | java.lang.String | 写入的目标文件名称。 |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | 保存选项。 |

### saveToExcelFile(String targetFile, int format) {#saveToExcelFile-java.lang.String-int-}
```
public void saveToExcelFile(String targetFile, int format)
```


将工作表保存到 Excel 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| targetFile | java.lang.String | 写入的目标文件名称。 |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat)。文件格式（Excel2003、Excel2007、CSV、SpreadsheetML） |

### setACWClientPath(String value) {#setACWClientPath-java.lang.String-}
```
public void setACWClientPath(String value)
```


设置控件的脚本/图片文件的 Web 路径。例如："http://localhost/acw\\_client"。你也可以在 web.config 文件中设置此值。将此节添加到 `<configuration>` 节中：
`<appSettings>`
`<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />`
`</appSettings>`


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setACWLanguageFileUrl(String value) {#setACWLanguageFileUrl-java.lang.String-}
```
public void setACWLanguageFileUrl(String value)
```


设置控件语言文件的 Web URL。例如："/acw\\_client/lang\\_en.js"。
默认情况下，使用内置的英文文件。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setActiveCell(GridCell value) {#setActiveCell-com.aspose.gridweb.GridCell-}
```
public void setActiveCell(GridCell value)
```


设置当前工作表的活动单元格。自 1.9.0.1 版起已改为可写。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setActiveCellBgColor(Color value) {#setActiveCellBgColor-com.aspose.gridweb.Color-}
```
public void setActiveCellBgColor(Color value)
```


指定活动单元格的背景颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveCellColor(Color value) {#setActiveCellColor-com.aspose.gridweb.Color-}
```
public void setActiveCellColor(Color value)
```


指定活动单元格的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderBgColor(Color value) {#setActiveHeaderBgColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderBgColor(Color value)
```


指定活动行/列标题的背景颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderColor(Color value) {#setActiveHeaderColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderColor(Color value)
```


指定活动行/列标题的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


设置活动工作表索引。等于 WebWorksheets.ActiveSheetIndex。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setActiveTabStyle(GridTableItemStyle value) {#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setActiveTabStyle(GridTableItemStyle value)
```


指定活动标签页的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setAutoRefreshChart(boolean value) {#setAutoRefreshChart-boolean-}
```
public void setAutoRefreshChart(boolean value)
```


设置在更新单元格值时是否更新图表图像，默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBackColor(Color value) {#setBackColor-com.aspose.gridweb.Color-}
```
public void setBackColor(Color value)
```


在 WebControl 中设置 BackColor

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```


在 WebControl 中设置 BorderColor

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


在 WebControl 中设置 BorderStyle

参见 [BorderStyle](../../com.aspose.gridweb/borderstyle)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```


在 WebControl 中设置 BorderWidth

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setBottomTableStyle(GridTableStyle value) {#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setBottomTableStyle(GridTableStyle value)
```


设置控件底部栏的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


设置在单元格值更改或导入文件后是否计算公式。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```


在 WebControl 中设置 CssClass

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCurrentPageIndex(int value) {#setCurrentPageIndex-int-}
```
public void setCurrentPageIndex(int value)
```


设置分页模式下的当前页索引。

**Remarks**

在分页模式下，控件一次显示 PageSize 行数据，并在选项卡栏中显示页面选择控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setCustomCalculationEngine(GridAbstractCalculationEngine value) {#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-}
```
public void setCustomCalculationEngine(GridAbstractCalculationEngine value)
```


表示用户的自定义计算引擎，用于扩展 Aspose.Cells 的默认计算引擎。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine) |  |

### setCustomStyle(InputStream stream) {#setCustomStyle-java.io.InputStream-}
```
public void setCustomStyle(InputStream stream)
```


从流（包括磁盘文件流或内存流）设置自定义样式文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.InputStream | 文件的流，包括磁盘文件流或内存流。 |

### setCustomStyleFileName(String value) {#setCustomStyleFileName-java.lang.String-}
```
public void setCustomStyleFileName(String value)
```


设置自定义样式文件名。

**Remarks**

自定义样式文件是 XML 文件。当设置文件名时，文件将立即加载。这里是 "standard preset style" 的内容 ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```


获取/设置机器的 DPI。

**Remarks**

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


设置控件的默认字体名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```


设置控件的默认字体大小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |

### setDefaultGridLineColor(Color value) {#setDefaultGridLineColor-com.aspose.gridweb.Color-}
```
public void setDefaultGridLineColor(Color value)
```


设置默认网格线的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setDisplayCellTip(boolean value) {#setDisplayCellTip-boolean-}
```
public void setDisplayCellTip(boolean value)
```


设置是否显示提示，默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEditMode(boolean value) {#setEditMode-boolean-}
```
public void setEditMode(boolean value)
```


设置控件的编辑模式。

**Remarks**

当设置为 true 时，控件的单元格可编辑，并显示 "save" 和 "undo" 图标。当设置为 false 时，控件的单元格为只读，并且不显示 "save" 和 "undo" 图标。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableAJAX(boolean value) {#setEnableAJAX-boolean-}
```
public void setEnableAJAX(boolean value)
```


设置是否使用 AJAX 调用，默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableAsync(boolean value) {#setEnableAsync-boolean-}
```
public void setEnableAsync(boolean value)
```


设置是否以异步方式加载单元格数据，建议在单个工作表超过 10000 个单元格时使用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableClientColumnOperations(boolean value) {#setEnableClientColumnOperations-boolean-}
```
public void setEnableClientColumnOperations(boolean value)
```


设置是否启用客户端列操作。

**Remarks**

当设置为 true 时，用户可以使用右键菜单添加/删除列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableClientFreeze(boolean value) {#setEnableClientFreeze-boolean-}
```
public void setEnableClientFreeze(boolean value)
```


设置是否启用客户端冻结操作。

**Remarks**

当设置为 true 时，用户可以使用右键菜单冻结/取消冻结窗格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableClientMergeOperations(boolean value) {#setEnableClientMergeOperations-boolean-}
```
public void setEnableClientMergeOperations(boolean value)
```


设置是否启用客户端合并操作。

**Remarks**

当设置为 true 时，用户可以使用右键菜单合并/拆分单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableClientResizeColumnRow(boolean value) {#setEnableClientResizeColumnRow-boolean-}
```
public void setEnableClientResizeColumnRow(boolean value)
```


设置是否启用客户端列和行的大小调整。

**Remarks**

当设置为 true 时，用户可以在客户端调整列和行的大小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableClientRowOperations(boolean value) {#setEnableClientRowOperations-boolean-}
```
public void setEnableClientRowOperations(boolean value)
```


设置是否启用客户端行操作。

**Remarks**

当设置为 true 时，用户可以使用右键菜单添加/删除行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableDoubleClickEvent(boolean value) {#setEnableDoubleClickEvent-boolean-}
```
public void setEnableDoubleClickEvent(boolean value)
```


设置是否启用客户侧双击事件。

**Remarks**

当设置为 true 时，控件将接收客户端双击事件，您可以在服务器端处理这些事件。否则，控件将忽略所有双击事件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableMetalLightEffect(boolean value) {#setEnableMetalLightEffect-boolean-}
```
public void setEnableMetalLightEffect(boolean value)
```


设置是否应用金属光效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnablePaging(boolean value) {#setEnablePaging-boolean-}
```
public void setEnablePaging(boolean value)
```


设置是否启用控件的分页模式。

**Remarks**

当设置为 true 时，控件一次显示 PageSize 行数据，并在选项卡栏中显示页面选择控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableStyleDialogbox(boolean value) {#setEnableStyleDialogbox-boolean-}
```
public void setEnableStyleDialogbox(boolean value)
```


设置是否启用客户端样式对话框。

**Remarks**

当设置为 true 时，用户可以通过在弹出菜单中选择 "Format Cell..." 来使用样式对话框设置单元格的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


在 WebControl 中设置 Enabled

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFilteredPaging(boolean value) {#setFilteredPaging-boolean-}
```
public void setFilteredPaging(boolean value)
```


设置在数据过滤后是否启用分页，EnablePaging 为 true 时生效。

**Remarks**

当设置为 true 时，控件将基于过滤后的数据进行分页，默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


设置字体文件夹

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontFolder | java.lang.String | 包含 TrueType 字体的文件夹。 |
| recursive | boolean | 确定是否扫描子文件夹。 |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


设置字体文件夹

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontFolders | java.lang.String[] | 包含 TrueType 字体的文件夹集合。 |
| recursive | boolean | 确定是否扫描子文件夹。 |

### setForceValidation(boolean value) {#setForceValidation-boolean-}
```
public void setForceValidation(boolean value)
```


设置是否强制客户侧验证。

**Remarks**

当设置为 true 时，数据将在所有输入字段有效之前不会提交到服务器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```


在 WebControl 中设置 ForeColor

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setFrameTableStyle(GridTableStyle value) {#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setFrameTableStyle(GridTableStyle value)
```


设置控件的框架样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setGoonDefaultSaveOperation(boolean value) {#setGoonDefaultSaveOperation-boolean-}
```
public void setGoonDefaultSaveOperation(boolean value)
```


设置 GridWeb 是否执行默认保存操作，默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setHeaderBarHeight(Unit value) {#setHeaderBarHeight-com.aspose.gridweb.Unit-}
```
public void setHeaderBarHeight(Unit value)
```


设置控件顶部标题栏的高度（System.Web.UI.WebControl.Unit）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeaderBarStyle(GridTableItemStyle value) {#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setHeaderBarStyle(GridTableItemStyle value)
```


设置标题栏的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setHeaderBarTableStyle(GridTableStyle value) {#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setHeaderBarTableStyle(GridTableStyle value)
```


设置控件标题栏的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setHeaderBarWidth(Unit value) {#setHeaderBarWidth-com.aspose.gridweb.Unit-}
```
public void setHeaderBarWidth(Unit value)
```


设置控件左侧标题栏的宽度（System.Web.UI.WebControl.Unit）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```


设置控件的高度（System.Web.UI.WebControl.Unit）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setIgnoreStyleWithNoData(boolean value) {#setIgnoreStyleWithNoData-boolean-}
```
public void setIgnoreStyleWithNoData(boolean value)
```


设置 GridWeb 是否忽略显示不包含单元格值但仍有样式的行或列。如果设置为 true，性能会更好。默认值为 false，这意味着如果最后连续的行/列没有单元格值但有样式，我们仍会显示它们。此选项仅在 EnableAsync 为 false 时有效。当 EnableAsync 为 true 时，此选项无效，意味着 GridWeb 将显示所有带样式的行/列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLoadOptions(GridLoadOptions value) {#setLoadOptions-com.aspose.gridweb.GridLoadOptions-}
```
public void setLoadOptions(GridLoadOptions value)
```


表示 GridWeb 的加载选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridLoadOptions](../../com.aspose.gridweb/gridloadoptions) |  |

### setMaxColumn(int value) {#setMaxColumn-int-}
```
public void setMaxColumn(int value)
```


设置 Web 工作表的最大显示列索引（从零开始）。控件使用 MaxColumn 与工作表数据最大列之间的较大值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMaxRow(int value) {#setMaxRow-int-}
```
public void setMaxRow(int value)
```


设置 Web 工作表的最大显示行索引（从零开始）。控件使用 MaxRow 与工作表数据最大行之间的较大值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMessage(String value) {#setMessage-java.lang.String-}
```
public void setMessage(String value)
```


设置网格的消息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setMinColumn(int value) {#setMinColumn-int-}
```
public void setMinColumn(int value)
```


设置 Web 工作表的最小显示列索引（从零开始）。控件使用 MinColumn 与工作表数据最小列之间的较小值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMinRow(int value) {#setMinRow-int-}
```
public void setMinRow(int value)
```


设置网页工作表的最小显示行索引（从零开始）。控件使用 MinRow 和工作表数据的最小行之间的较小值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setNeedRenderGroupRows(boolean value) {#setNeedRenderGroupRows-boolean-}
```
public void setNeedRenderGroupRows(boolean value)
```


设置是否显示分组行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setNoHScroll(boolean value) {#setNoHScroll-boolean-}
```
public void setNoHScroll(boolean value)
```


设置一个值，指示水平滚动条是否隐藏。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setNoScroll(boolean value) {#setNoScroll-boolean-}
```
public void setNoScroll(boolean value)
```


设置是否显示滚动条。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setNoVScroll(boolean value) {#setNoVScroll-boolean-}
```
public void setNoVScroll(boolean value)
```


设置一个值，指示垂直滚动条是否隐藏。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setOnAjaxCallFinishedClientFunction(String value) {#setOnAjaxCallFinishedClientFunction-java.lang.String-}
```
public void setOnAjaxCallFinishedClientFunction(String value)
```


设置 AJAX 调用完成后要调用的客户端函数名称。客户端函数应按如下方式声明：
function GridAjaxcallFinished()
\{
alert(this.id+" ajaxcall finished ");
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOnCellErrorClientFunction(String value) {#setOnCellErrorClientFunction-java.lang.String-}
```
public void setOnCellErrorClientFunction(String value)
```


设置当单元格验证失败时要调用的客户端函数名称。客户端函数应按如下方式声明：
function MyOnCellError(cell)
\{
alert(this.getCellValueByCell(cell));
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOnCellSelectedAjaxCallBackClientFunction(String value) {#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-}
```
public void setOnCellSelectedAjaxCallBackClientFunction(String value)
```


设置当选中单元格时要调用的客户端函数。客户端函数应按如下方式声明：
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\{

\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOnCellSelectedClientFunction(String value) {#setOnCellSelectedClientFunction-java.lang.String-}
```
public void setOnCellSelectedClientFunction(String value)
```


设置当选中单元格时要调用的客户端函数。客户端函数应按如下方式声明：
function MyOnSelectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, "test");
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOnCellUnselectedClientFunction(String value) {#setOnCellUnselectedClientFunction-java.lang.String-}
```
public void setOnCellUnselectedClientFunction(String value)
```


设置当取消选中单元格时要调用的客户端函数。客户端函数应按如下方式声明：
function MyOnUnselectCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOnCellUpdatedClientFunction(String value) {#setOnCellUpdatedClientFunction-java.lang.String-}
```
public void setOnCellUpdatedClientFunction(String value)
```


设置当单元格的值更新时要调用的客户端函数名称。客户端函数应按如下方式声明：
function MyOnCellUpdated(cell)
\{
alert(this.getCellValueByCell(cell));
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOnContextMenuShowClientFunction(String value) {#setOnContextMenuShowClientFunction-java.lang.String-}
```
public void setOnContextMenuShowClientFunction(String value)
```


设置当上下文菜单显示时要调用的客户端函数。客户端函数应按如下方式声明：
function onContextMenuShow()
\{
var menu = event.srcElement;
menu.setItemVisibility("Delete", "block");
menu.setItemVisibility("Update", "none");
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOnDoubleClickCellClientFunction(String value) {#setOnDoubleClickCellClientFunction-java.lang.String-}
```
public void setOnDoubleClickCellClientFunction(String value)
```


设置当双击单元格时要调用的客户端函数。客户端函数应按如下方式声明：
function MyOnDoubleClickCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOnDoubleClickRowClientFunction(String value) {#setOnDoubleClickRowClientFunction-java.lang.String-}
```
public void setOnDoubleClickRowClientFunction(String value)
```


设置当双击行时要调用的客户端函数。客户端函数应按如下方式声明：
function MyOnRowDoubleClick(row)
\{
alert(row);
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOnGridInitClientFunction(String value) {#setOnGridInitClientFunction-java.lang.String-}
```
public void setOnGridInitClientFunction(String value)
```


设置网格初始化时要调用的客户端函数名称。客户端函数应按如下方式声明：
function MyOnGridInit(grid)
\{
alert("网格已初始化: " + grid.id);
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOnPageChangeClientFunction(String value) {#setOnPageChangeClientFunction-java.lang.String-}
```
public void setOnPageChangeClientFunction(String value)
```


设置在页面索引更改后要调用的客户端函数。仅在 EnablePaging 为 true 时生效。客户端函数应按如下方式声明：
function MyOnPageChange(index)
\{
console.log("当前页面是:"+index);
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOnPageSubmitClientFunction(String value) {#setOnPageSubmitClientFunction-java.lang.String-}
```
public void setOnPageSubmitClientFunction(String value)
```


设置在页面提交前在客户端调用的函数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOnShapeSelectedClientFunction(String value) {#setOnShapeSelectedClientFunction-java.lang.String-}
```
public void setOnShapeSelectedClientFunction(String value)
```


设置当选中形状时要调用的客户端函数。客户端函数应按如下方式声明：
function MyOnSelectShape(shape)
\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\}

注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOnSubmitClientFunction(String value) {#setOnSubmitClientFunction-java.lang.String-}
```
public void setOnSubmitClientFunction(String value)
```


设置在客户端提交控件之前要调用的客户端函数。客户端函数应按如下方式声明：
function MyOnSubmit(arg, cancelEdit)
\{
return true;
\}
arg 是提交参数，包含要发送到服务器的命令。cancelEdit 是布尔值，指示控件在提交前是否已丢弃用户输入。如果函数返回 true，控件将继续提交。
注意：您可以在客户端函数中使用 "this" 指针指向触发事件的网格控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


设置是否仅适配高度未自定义的行，默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPageSize(int value) {#setPageSize-int-}
```
public void setPageSize(int value)
```


设置分页模式下的页面大小。

**Remarks**

在分页模式下，控件一次显示 PageSize 行数据，并在选项卡栏中显示页面选择控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPictureCachePath(String value) {#setPictureCachePath-java.lang.String-}
```
public static void setPictureCachePath(String value)
```


设置工作簿的图像存储路径，所有形状和图像将存储在此目录中，默认路径为当前应用程序基目录下的 acwcache，用户需要实现计划服务来清理会话超时的文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


设置预设样式。

参见 [PresetStyle](../../com.aspose.gridweb/presetstyle)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setRefreshValidation(boolean value) {#setRefreshValidation-boolean-}
```
public void setRefreshValidation(boolean value)
```


设置在单元格值更改后是否刷新验证值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRenderHiddenRow(boolean value) {#setRenderHiddenRow-boolean-}
```
public void setRenderHiddenRow(boolean value)
```


设置是否在 GridControl 中渲染隐藏行，默认值为 false。如果需要稍后取消隐藏隐藏行，应将其设为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRowHeightForCSV(double value) {#setRowHeightForCSV-double-}
```
public void setRowHeightForCSV(double value)
```


设置 CSV 文件的行高（单位为点），默认值为 14.5。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setScrollBarArrowColor(Color value) {#setScrollBarArrowColor-com.aspose.gridweb.Color-}
```
public void setScrollBarArrowColor(Color value)
```


指定滚动条箭头按钮的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setScrollBarBaseColor(Color value) {#setScrollBarBaseColor-com.aspose.gridweb.Color-}
```
public void setScrollBarBaseColor(Color value)
```


指定控件滚动条的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellBgColor(Color value) {#setSelectCellBgColor-com.aspose.gridweb.Color-}
```
public void setSelectCellBgColor(Color value)
```


指定多选范围内已选单元格的背景颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellColor(Color value) {#setSelectCellColor-com.aspose.gridweb.Color-}
```
public void setSelectCellColor(Color value)
```


指定多选范围内已选单元格的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSessionStorePath(String value) {#setSessionStorePath-java.lang.String-}
```
public void setSessionStorePath(String value)
```


设置会话模式为 File 或 ViewState 时的会话缓存存储路径，例如：gridweb.SessionStorePath="c:/mytempdir/session"；则会将会话数据存储在 c:/mytempdir/session。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridweb.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


表示工作簿设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings) |  |

### setShowAddButton(boolean value) {#setShowAddButton-boolean-}
```
public void setShowAddButton(boolean value)
```


设置是否显示添加工作表按钮。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowBottomBar(boolean value) {#setShowBottomBar-boolean-}
```
public void setShowBottomBar(boolean value)
```


指定是否在控件底部显示命令栏（包括命令栏和标签栏）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowCellEditBox(boolean value) {#setShowCellEditBox-boolean-}
```
public void setShowCellEditBox(boolean value)
```


是否在 Gridweb 中显示类似 MS-EXCEL 的编辑框工具栏。启用后，当前单元格的编辑框将在 Gridweb 中显示。如果启用此功能，需要在你的 aspx 文件中导入 jquery js 库以支持此新功能。所有最新的 jquery 版本均可。等。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowCommandBarAtTop(boolean value) {#setShowCommandBarAtTop-boolean-}
```
public void setShowCommandBarAtTop(boolean value)
```


指定是否在控件顶部显示命令栏（包括命令栏和标签栏）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowContextMenu(boolean value) {#setShowContextMenu-boolean-}
```
public void setShowContextMenu(boolean value)
```


设置是否显示上下文菜单，默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowDefaultGridLine(boolean value) {#setShowDefaultGridLine-boolean-}
```
public void setShowDefaultGridLine(boolean value)
```


设置是否显示单元格的默认网格线。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowHeaderBar(boolean value) {#setShowHeaderBar-boolean-}
```
public void setShowHeaderBar(boolean value)
```


设置是否显示标题栏。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowLoading(boolean value) {#setShowLoading-boolean-}
```
public void setShowLoading(boolean value)
```


指定在回发到服务器期间是否显示加载对话框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowLoadingPosition(String value) {#setShowLoadingPosition-java.lang.String-}
```
public void setShowLoadingPosition(String value)
```


指定在回发到服务器期间显示加载对话框的左、上位置（单位为像素），例如 100,200 表示加载对话框的左、上位置分别为 100px 和 200px。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setShowSaveButton(boolean value) {#setShowSaveButton-boolean-}
```
public void setShowSaveButton(boolean value)
```


设置是否显示保存按钮。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowSubmitButton(boolean value) {#setShowSubmitButton-boolean-}
```
public void setShowSubmitButton(boolean value)
```


设置是否显示提交按钮。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowTabBar(boolean value) {#setShowTabBar-boolean-}
```
public void setShowTabBar(boolean value)
```


设置是否显示选项卡栏。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowTabNavigation(boolean value) {#setShowTabNavigation-boolean-}
```
public void setShowTabNavigation(boolean value)
```


设置是否显示选项卡导航按钮，默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowUndoButton(boolean value) {#setShowUndoButton-boolean-}
```
public void setShowUndoButton(boolean value)
```


设置是否显示撤销按钮。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSpanWrap(boolean value) {#setSpanWrap-boolean-}
```
public void setSpanWrap(boolean value)
```


指定是否在单元格跨越范围内换行内容，默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setTabIndex(short value) {#setTabIndex-short-}
```
public void setTabIndex(short value)
```


在 WebControl 中设置 TabIndex

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 短 |  |

### setTabStyle(GridTableItemStyle value) {#setTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setTabStyle(GridTableItemStyle value)
```


设置选项卡栏的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


在 WebControl 中设置 ToolTip

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setUseClientPageHeight(boolean value) {#setUseClientPageHeight-boolean-}
```
public void setUseClientPageHeight(boolean value)
```


设置 gridweb 是否使用客户端页面高度作为控件高度，适用于将 Height="100%" 的情况，默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setViewPanelScrollLeft(String value) {#setViewPanelScrollLeft-java.lang.String-}
```
public void setViewPanelScrollLeft(String value)
```


设置网格视图面板滚动条的位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setViewPanelScrollTop(String value) {#setViewPanelScrollTop-java.lang.String-}
```
public void setViewPanelScrollTop(String value)
```


设置网格视图面板滚动条的位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setViewTableStyle(GridTableStyle value) {#setViewTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setViewTableStyle(GridTableStyle value)
```


设置数据视图面板的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


设置控件的宽度( System.Web.UI.WebControl.Unit )。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setXhtmlMode(boolean value) {#setXhtmlMode-boolean-}
```
public void setXhtmlMode(boolean value)
```


设置是否使用 XHTML 样式，默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

