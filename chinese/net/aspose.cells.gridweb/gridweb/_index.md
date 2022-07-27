---
title: GridWeb
second_title: Aspose.Cells for .NET API 参考
description: 
type: docs
weight: 800
url: /zh/net/aspose.cells.gridweb/gridweb/
---
## GridWeb class

```csharp
public class GridWeb : MainWeb
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [GridWeb](gridweb)() | 默认构造函数。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb/mainweb/activecell) { get; set; } | 获取或设置当前工作表的活动单元格。 从版本 1.9.0.1 开始更改为可写。 |
| [ActiveCellBgColor](../../aspose.cells.gridweb/mainweb/activecellbgcolor) { get; set; } | 指定活动单元格的背景颜色。 |
| [ActiveCellColor](../../aspose.cells.gridweb/mainweb/activecellcolor) { get; set; } | 指定活动单元格的颜色。 |
| [ActiveHeaderBgColor](../../aspose.cells.gridweb/mainweb/activeheaderbgcolor) { get; set; } | 指定活动行/列标题的背景颜色。 |
| [ActiveHeaderColor](../../aspose.cells.gridweb/mainweb/activeheadercolor) { get; set; } | 指定活动行/列标题的颜色。 |
| [ActiveSheet](../../aspose.cells.gridweb/mainweb/activesheet) { get; } | 获取活动工作表 |
| [ActiveSheetIndex](../../aspose.cells.gridweb/mainweb/activesheetindex) { get; set; } | 获取或设置活动工作表索引。等于 WebWorksheets.ActiveSheetIndex. |
| [ActiveTabStyle](../../aspose.cells.gridweb/mainweb/activetabstyle) { get; set; } | 指定活动选项卡的样式。 |
| [ACWClientPath](../../aspose.cells.gridweb/mainweb/acwclientpath) { get; set; } | 获取或设置控件的脚本/图像文件的网络路径。例如：“http://localhost/acw_client”. 您也可以在 web.config 文件中设置此值。将此部分添加到 &lt;configuration&gt; 部分： &lt;应用设置&gt;&lt;add key="aspose.cells.gridweb.acw_client_path" value="/acw_client/" /&gt;&lt;/app设置&gt; |
| [ACWLanguageFileUrl](../../aspose.cells.gridweb/mainweb/acwlanguagefileurl) { get; set; } | 获取或设置控件语言文件的网址。例如：“/acw_client/lang_en.js”. 默认情况下，使用内置的英文文件。 |
| [AutoRefreshChart](../../aspose.cells.gridweb/mainweb/autorefreshchart) { get; set; } | 获取或设置更新单元格值时是否更新图表图像。默认为true |
| [BottomTableStyle](../../aspose.cells.gridweb/mainweb/bottomtablestyle) { get; set; } | 获取或设置控件底栏的样式。 |
| [CurrentPageIndex](../../aspose.cells.gridweb/mainweb/currentpageindex) { get; set; } |  |
| [CustomCalculationEngine](../../aspose.cells.gridweb/mainweb/customcalculationengine) { get; set; } | 代表用户自定义计算引擎，扩展Aspose.Cells的默认计算引擎。 |
| [CustomCommandButtons](../../aspose.cells.gridweb/mainweb/customcommandbuttons) { get; } |  |
| [CustomStyleFileName](../../aspose.cells.gridweb/mainweb/customstylefilename) { get; set; } | 获取或设置自定义样式文件名。 |
| [DefaultFontName](../../aspose.cells.gridweb/mainweb/defaultfontname) { get; set; } | 获取或设置控件的默认字体名称。 |
| [DefaultFontSize](../../aspose.cells.gridweb/mainweb/defaultfontsize) { get; set; } | 获取或设置控件的默认字体大小。 |
| [DefaultGridLineColor](../../aspose.cells.gridweb/mainweb/defaultgridlinecolor) { get; set; } | 获取或设置默认网格线的颜色。 |
| [DisplayCellTip](../../aspose.cells.gridweb/mainweb/displaycelltip) { get; set; } |  |
| [EditMode](../../aspose.cells.gridweb/mainweb/editmode) { get; set; } | 获取或设置控件的编辑模式。 |
| [EnableAJAX](../../aspose.cells.gridweb/mainweb/enableajax) { get; set; } |  |
| [EnableAsync](../../aspose.cells.gridweb/mainweb/enableasync) { get; set; } | 获取或设置是否异步加载cells数据，建议申请10000以上cells的一张表 |
| [EnableClientColumnOperations](../../aspose.cells.gridweb/mainweb/enableclientcolumnoperations) { get; set; } | 获取或设置是否开启客户端列操作 |
| [EnableClientFreeze](../../aspose.cells.gridweb/mainweb/enableclientfreeze) { get; set; } | 获取或设置是否开启客户端冻结操作 |
| [EnableClientMergeOperations](../../aspose.cells.gridweb/mainweb/enableclientmergeoperations) { get; set; } | 获取或设置是否开启客户端合并操作 |
| [EnableClientResizeColumnRow](../../aspose.cells.gridweb/mainweb/enableclientresizecolumnrow) { get; set; } | 获取或设置是否启用客户端调整列和行大小。 |
| [EnableClientRowOperations](../../aspose.cells.gridweb/mainweb/enableclientrowoperations) { get; set; } | 获取或设置是否启用客户端行操作。 |
| [EnableDoubleClickEvent](../../aspose.cells.gridweb/mainweb/enabledoubleclickevent) { get; set; } | 获取或设置是否开启客户端双击事件 |
| [EnableMetalLightEffect](../../aspose.cells.gridweb/mainweb/enablemetallighteffect) { get; set; } | 获取或设置是否应用金属光效果。 |
| [EnablePaging](../../aspose.cells.gridweb/mainweb/enablepaging) { get; set; } | 获取或设置是否启用控件的分页模式。 |
| [EnableStyleDialogbox](../../aspose.cells.gridweb/mainweb/enablestyledialogbox) { get; set; } | 获取或设置是否启用客户端样式对话框。 |
| [FilteredPaging](../../aspose.cells.gridweb/mainweb/filteredpaging) { get; set; } | 获取或设置数据过滤后是否开启分页，当EnablePaging为true时生效 |
| [ForceValidation](../../aspose.cells.gridweb/mainweb/forcevalidation) { get; set; } | 获取或设置是否强制客户端验证。 |
| [FrameTableStyle](../../aspose.cells.gridweb/mainweb/frametablestyle) { get; set; } | 获取或设置控件的边框样式 |
| [GoonDefaultSaveOperation](../../aspose.cells.gridweb/mainweb/goondefaultsaveoperation) { get; set; } | 获取或设置GridWeb是否会做默认的保存操作，默认值为true。 |
| [HeaderBarHeight](../../aspose.cells.gridweb/mainweb/headerbarheight) { get; set; } | 获取或设置控件顶部标题栏的高度（System.Web.UI.WebControl.Unit）。 |
| [HeaderBarStyle](../../aspose.cells.gridweb/mainweb/headerbarstyle) { get; set; } | 获取或设置标题栏的样式。 |
| [HeaderBarTableStyle](../../aspose.cells.gridweb/mainweb/headerbartablestyle) { get; set; } | 获取或设置控件的标题栏样式。 |
| [HeaderBarWidth](../../aspose.cells.gridweb/mainweb/headerbarwidth) { get; set; } | 获取或设置控件的宽度（System.Web.UI.WebControl.Unit）或左侧标题栏。 |
| override [Height](../../aspose.cells.gridweb/mainweb/height) { get; set; } | 获取或设置控件的高度（System.Web.UI.WebControl.Unit）。 |
| [IsCalculateFormula](../../aspose.cells.gridweb/mainweb/iscalculateformula) { get; set; } | 获取或设置是否在单元格值更改后或导入文件后计算公式。默认值为真。 |
| [IsPostBack](../../aspose.cells.gridweb/mainweb/ispostback) { get; } | 获取一个值，该值指示是否正在加载 gridweb 以响应客户端回发， 还是第一次加载和访问它。 |
| [LinksTable](../../aspose.cells.gridweb/mainweb/linkstable) { get; } |  |
| [MaxColumn](../../aspose.cells.gridweb/mainweb/maxcolumn) { get; set; } | 获取或设置网页表格的最大显示列索引（从零开始）。 控件使用MaxColumn和表格数据最大列的较大值。 |
| [MaxRow](../../aspose.cells.gridweb/mainweb/maxrow) { get; set; } | 获取或设置 web sheet 的最大显示行索引（从零开始）。 控件使用 MaxRow 和工作表数据的最大行的较大值。 |
| [Message](../../aspose.cells.gridweb/mainweb/message) { get; set; } |  |
| [MinColumn](../../aspose.cells.gridweb/mainweb/mincolumn) { get; set; } |  |
| [MinRow](../../aspose.cells.gridweb/mainweb/minrow) { get; set; } | 获取或设置网页表格的最小显示行索引（从零开始）。 控件使用MinRow和表格数据最小行的较小值。 |
| [ModifiedCells](../../aspose.cells.gridweb/mainweb/modifiedcells) { get; } | 获取客户端修改的单元格的集合。 |
| [NeedRenderGroupRows](../../aspose.cells.gridweb/mainweb/needrendergrouprows) { get; set; } | 获取或设置是否显示 grouprows . |
| [NoHScroll](../../aspose.cells.gridweb/mainweb/nohscroll) { get; set; } | 获取或设置水平滚动条是否隐藏的值。 |
| [NoScroll](../../aspose.cells.gridweb/mainweb/noscroll) { get; set; } |  |
| [NoVScroll](../../aspose.cells.gridweb/mainweb/novscroll) { get; set; } | 获取或设置垂直滚动条是否隐藏的值。 |
| [OnAjaxCallFinishedClientFunction](../../aspose.cells.gridweb/mainweb/onajaxcallfinishedclientfunction) { get; set; } | 获取或设置 ajaxcall 完成时要调用的客户端函数名称。 客户端函数应声明如下： 函数 GridAjaxcallFinished() { alert(this.id+" ajaxcall 完成"); }注意：您可以在客户端函数中使用“this”指针来指向触发事件的网格控件。 |
| [OnCellErrorClientFunction](../../aspose.cells.gridweb/mainweb/oncellerrorclientfunction) { get; set; } | 获取或设置单元格验证失败时要调用的客户端函数名称。 客户端函数应声明如下： 函数 MyOnCellError（单元格） { alert(GridWeb1.getCellValueByCell(cell)); }注意：您可以在客户端函数中使用“this”指针来指向触发事件的网格控件。 |
| [OnCellSelectedAjaxCallBackClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedajaxcallbackclientfunction) { get; set; } | 获取或设置选择单元格时要调用的客户端函数。 客户端函数应声明如下： 函数 MyOnSelectCellAjaxCallBack(cell,customerdata) { }注意：您可以在客户端函数中使用“this”指针来指向触发事件的网格控件。 |
| [OnCellSelectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellselectedclientfunction) { get; set; } | 获取或设置选择单元格时要调用的客户端函数。 客户端函数应声明如下： 函数 MyOnSelectCell（单元格） { GridWeb1.setCellValueByCell(cell, "test"); }注意：您可以在客户端函数中使用“this”指针来指向触发事件的网格控件。 |
| [OnCellUnselectedClientFunction](../../aspose.cells.gridweb/mainweb/oncellunselectedclientfunction) { get; set; } | 获取或设置取消选择单元格时要调用的客户端函数。 客户端函数应声明如下： 函数 MyOnUnselectCell（单元格） { GridWeb1.setCellValueByCell(cell, "test"); }注意：您可以在客户端函数中使用“this”指针来指向触发事件的网格控件。 |
| [OnCellUpdatedClientFunction](../../aspose.cells.gridweb/mainweb/oncellupdatedclientfunction) { get; set; } | 获取或设置更新单元格值时要调用的客户端函数名称。 客户端函数应声明如下： 函数 MyOnCellUpdated（单元格） { alert(this.getCellValueByCell(cell)); }注意：您可以在客户端函数中使用“this”指针来指向触发事件的网格控件。 |
| [OnContextMenuShowClientFunction](../../aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction) { get; set; } | 获取或设置显示上下文菜单时要调用的客户端函数。 客户端函数应声明如下： 函数 onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("删除", "块"); menu.setItemVisibility("更新", "无"); }注意：您可以在客户端函数中使用“this”指针来指向触发事件的网格控件。 |
| [OnDoubleClickCellClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickcellclientfunction) { get; set; } | 获取或设置双击单元格时要调用的客户端函数。 客户端函数应声明如下： 函数 MyOnDoubleClickCell（单元格） { GridWeb1.setCellValueByCell(cell, "test"); }注意：您可以在客户端函数中使用“this”指针来指向触发事件的网格控件。 |
| [OnDoubleClickRowClientFunction](../../aspose.cells.gridweb/mainweb/ondoubleclickrowclientfunction) { get; set; } | 获取或设置双击行时调用的客户端函数。 客户端函数应声明如下： 函数 MyOnRowDoubleClick(row) { 警报（行）； }注意：您可以在客户端函数中使用“this”指针来指向触发事件的网格控件。 |
| [OnGridInitClientFunction](../../aspose.cells.gridweb/mainweb/ongridinitclientfunction) { get; set; } | 获取或设置网格初始化时要调用的客户端函数名称。 客户端函数应声明如下： 函数 MyOnGridInit（网格） { alert("网格初始化：" + grid.id); }注意：您可以在客户端函数中使用“this”指针来指向触发事件的网格控件。 |
| [OnlyAuto](../../aspose.cells.gridweb/mainweb/onlyauto) { get; set; } | 获取或设置是否只适合不自定义高度的行，默认值为false |
| [OnPageChangeClientFunction](../../aspose.cells.gridweb/mainweb/onpagechangeclientfunction) { get; set; } | 获取或设置页面索引改变后调用的客户端函数。仅在EnablePaging为true时生效。 客户端函数声明如下： 函数 MyOnPageChange(index) { console.log("当前页面是："+index); }注意：您可以在客户端函数中使用“this”指针来指向触发事件的网格控件。 |
| [OnPageSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onpagesubmitclientfunction) { get; set; } | 获取或设置在客户端提交页面之前要调用的客户端函数。 |
| [OnShapeSelectedClientFunction](../../aspose.cells.gridweb/mainweb/onshapeselectedclientfunction) { get; set; } | 获取或设置选择形状时要调用的客户端函数。 客户端函数应声明如下： 函数 MyOnSelectShape（形状） { var name=shape.getAttribute("namevalue") var text=shape.getAttribute("textvalue") var value=shape.getAttribute("controlvalue") var type=shape.getAttribute("msotype") }注意：您可以在客户端函数中使用“this”指针来指向触发事件的网格控件。 |
| [OnSubmitClientFunction](../../aspose.cells.gridweb/mainweb/onsubmitclientfunction) { get; set; } | 获取或设置在客户端提交控件之前要调用的客户端函数。 客户端函数应声明如下： 函数 MyOnSubmit(arg, cancelEdit) {返回真；} arg 是提交参数，包含要提交到服务器的命令。 cancelEdit 是布尔值，表示控件在提交之前是否丢弃了用户输入。 如果函数返回true，控件将继续提交。 注意：您可以在客户端函数中使用“this”指针来指向触发事件的网格控件。 |
| [PageSize](../../aspose.cells.gridweb/mainweb/pagesize) { get; set; } | 获取或设置分页模式下的页面大小。 |
| [PicturesTable](../../aspose.cells.gridweb/mainweb/picturestable) { get; } |  |
| [PresetStyle](../../aspose.cells.gridweb/mainweb/presetstyle) { get; set; } | 获取或设置预设样式 |
| [RefreshValidation](../../aspose.cells.gridweb/mainweb/refreshvalidation) { get; set; } | 获取或设置单元格值改变后是否刷新验证值。 |
| [RenderHiddenRow](../../aspose.cells.gridweb/mainweb/renderhiddenrow) { get; set; } | 获取或设置是否在GridControl中渲染隐藏行，默认为false。 如果后面需要取消隐藏隐藏行，设置为true |
| [ScrollBarArrowColor](../../aspose.cells.gridweb/mainweb/scrollbararrowcolor) { get; set; } | 指定滚动条箭头按钮的颜色。 |
| [ScrollBarBaseColor](../../aspose.cells.gridweb/mainweb/scrollbarbasecolor) { get; set; } | 指定控件滚动条的颜色。 |
| [SelectCellBgColor](../../aspose.cells.gridweb/mainweb/selectcellbgcolor) { get; set; } | 指定多选范围内选定单元格的背景颜色。 |
| [SelectCellColor](../../aspose.cells.gridweb/mainweb/selectcellcolor) { get; set; } | 指定多选范围内选定单元格的颜色。 |
| [SelectCells](../../aspose.cells.gridweb/gridweb/selectcells) { get; } | 获取选择单元格集合。 |
| [SessionLoaded](../../aspose.cells.gridweb/mainweb/sessionloaded) { get; set; } |  |
| [SessionMode](../../aspose.cells.gridweb/mainweb/sessionmode) { get; set; } | 获取或设置网格的会话模式。 会话模式有 4 种类型： 1. 会话（默认）：使用系统会话存储工作表数据。 一般asp.net 使用InProc 会话状态。网格还支持“StateServer”出进程会话 state 和 SQLServer 会话状态。 2. ViewState：使用页面的视图状态来存储工作表数据。 3. 自定义：使用 LoadCustomData 和 SheetDataUpdated 事件来存储/恢复工作表数据。 4. 文件：在 SessionStorePath 中存储/恢复工作表数据。 |
| [SessionSaved](../../aspose.cells.gridweb/mainweb/sessionsaved) { get; set; } |  |
| [SessionStorePath](../../aspose.cells.gridweb/mainweb/sessionstorepath) { get; set; } | 获取或设置会话模式为File或ViewState时的会话缓存存储路径， 等：gridweb.SessionStorePath="c:/mytempdir/session"; 然后它将会话数据存储在 c:/mytempdir/session |
| [Settings](../../aspose.cells.gridweb/mainweb/settings) { get; set; } | 表示工作簿设置。 |
| [ShapesTable](../../aspose.cells.gridweb/mainweb/shapestable) { get; } |  |
| [ShowAddButton](../../aspose.cells.gridweb/mainweb/showaddbutton) { get; set; } | 获取或设置是否显示添加工作表按钮。 |
| [ShowBottomBar](../../aspose.cells.gridweb/mainweb/showbottombar) { get; set; } |  |
| [ShowCellEditBox](../../aspose.cells.gridweb/mainweb/showcelleditbox) { get; set; } | Gridweb 是否像 MS-EXCEL 一样显示编辑框工具栏。如果启用，当前单元格的编辑框将显示在 Gridweb 中。 如果我们启用此功能，我们需要在您的 aspx 文件中导入 jquery js 库以支持此新功能。所有最新的 jquery 版本都可以。等等 |
| [ShowCommandBarAtTop](../../aspose.cells.gridweb/mainweb/showcommandbarattop) { get; set; } | 指定是否在控件顶部显示命令栏（包括命令栏和标签栏）。 |
| [ShowContextMenu](../../aspose.cells.gridweb/mainweb/showcontextmenu) { get; set; } |  |
| [ShowDefaultGridLine](../../aspose.cells.gridweb/mainweb/showdefaultgridline) { get; set; } | 获取或设置是否显示单元格的默认网格线。 |
| [ShowHeaderBar](../../aspose.cells.gridweb/mainweb/showheaderbar) { get; set; } |  |
| [ShowLoading](../../aspose.cells.gridweb/mainweb/showloading) { get; set; } | 指定回发到服务器时是否显示加载对话框。 |
| [ShowLoadingPosition](../../aspose.cells.gridweb/mainweb/showloadingposition) { get; set; } | 指定左上角（以 px 为单位）以在回发到服务器等时显示加载对话框。 100,200 表示加载对话框的左侧，顶部位置在 100px,200px . |
| [ShowSaveButton](../../aspose.cells.gridweb/mainweb/showsavebutton) { get; set; } | 获取或设置是否显示保存按钮。 |
| [ShowSubmitButton](../../aspose.cells.gridweb/mainweb/showsubmitbutton) { get; set; } | 获取或设置是否显示提交按钮。 |
| [ShowTabBar](../../aspose.cells.gridweb/mainweb/showtabbar) { get; set; } |  |
| [ShowTabNavigation](../../aspose.cells.gridweb/mainweb/showtabnavigation) { get; set; } | 获取或设置tab导航按钮是否显示，默认为true。 |
| [ShowUndoButton](../../aspose.cells.gridweb/mainweb/showundobutton) { get; set; } | 获取或设置是否显示撤消按钮。 |
| [SpanWrap](../../aspose.cells.gridweb/mainweb/spanwrap) { get; set; } | 指定是否在单元格范围内换行。默认值为 true。 |
| [TabStyle](../../aspose.cells.gridweb/mainweb/tabstyle) { get; set; } | 获取或设置标签栏的样式。 |
| [UseClientPageHeight](../../aspose.cells.gridweb/mainweb/useclientpageheight) { get; set; } | 获取或设置gridweb是否使用客户端页面高度作为控件高度，适用于设置Height="100%"时，默认值为false |
| [ValidationsTable](../../aspose.cells.gridweb/mainweb/validationstable) { get; } |  |
| [ViewPanelScrollLeft](../../aspose.cells.gridweb/mainweb/viewpanelscrollleft) { get; set; } | 获取或设置网格视图面板滚动条的位置。 |
| [ViewPanelScrollTop](../../aspose.cells.gridweb/mainweb/viewpanelscrolltop) { get; set; } | 获取或设置网格视图面板滚动条的位置。 |
| [ViewTableStyle](../../aspose.cells.gridweb/mainweb/viewtablestyle) { get; set; } | 获取或设置数据视图面板的样式。 |
| [WebWorksheets](../../aspose.cells.gridweb/mainweb/webworksheets) { get; } |  |
| override [Width](../../aspose.cells.gridweb/mainweb/width) { get; set; } | 获取或设置控件的宽度（System.Web.UI.WebControl.Unit）。 |
| [WorkSheets](../../aspose.cells.gridweb/mainweb/worksheets) { get; } |  |
| [XhtmlMode](../../aspose.cells.gridweb/mainweb/xhtmlmode) { get; set; } |  |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [CalculateFormula](../../aspose.cells.gridweb/mainweb/calculateformula)() | 计算公式的结果。 |
| override [DataBind](../../aspose.cells.gridweb/mainweb/databind)() | 将控件及其所有子控件绑定到其数据源。 |
| override [Dispose](../../aspose.cells.gridweb/mainweb/dispose)() |  |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile)(Stream) | 从excel文件流导入，包括磁盘文件流或内存流。 |
| [ImportExcelFile](../../aspose.cells.gridweb/mainweb/importexcelfile)(string) | 从 excel 文件导入。 |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile)(Stream) | 从 CSV 文件流加载数据。 |
| [LoadCSVFile](../../aspose.cells.gridweb/mainweb/loadcsvfile)(string) | 从 CSV 文件加载数据。 |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile)(Stream) | 从 HTML 文件流加载数据。 |
| [LoadHTMLFile](../../aspose.cells.gridweb/mainweb/loadhtmlfile)(string) | 从 HTML 文件加载数据。 |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile)(Stream) | 从 SpreadSheetML 文件流加载数据。 |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/loadspreadsheetmlfile)(string) | 从 SpreadSheetML 文件加载数据。 |
| [RefreshChartShape](../../aspose.cells.gridweb/mainweb/refreshchartshape)() | 刷新活动工作表的所有图表图像。 |
| override [RenderBeginTag](../../aspose.cells.gridweb/mainweb/renderbegintag)(HtmlTextWriter) |  |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile)(Stream) | 将数据保存到 CSV 文件流。 |
| [SaveCSVFile](../../aspose.cells.gridweb/mainweb/savecsvfile)(string) | 将数据保存到 CSV 文件。 |
| [SaveCustomStyleFile](../../aspose.cells.gridweb/gridweb/savecustomstylefile#savecustomstylefile)(string) | 将控件的当前样式数据保存到 xml 文件中。 可用于创建您的自定义样式文件。 (2 methods) |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile)(Stream) | 将数据保存到 HTML 文件流中。 |
| [SaveHTMLFile](../../aspose.cells.gridweb/mainweb/savehtmlfile)(string) | 将数据保存到 HTML 文件中。 |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile)(Stream) | 将数据保存到 SpreadSheetML 文件流。 |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb/mainweb/savespreadsheetmlfile)(string) | 将数据保存到 SpreadSheetML 文件。 |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile)(Stream) | 将工作表保存到 excel 文件中。 |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile)(string) | 将工作表保存到 Excel 2003 格式的 excel 文件中。 |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile)(Stream, GridSaveFormat) | 将工作表保存到 excel 文件中。 |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile)(Stream, GridSaveOptions) | 将工作表保存到 excel 文件中。 |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile)(string, GridSaveFormat) | 将工作表保存到 excel 文件中。 |
| [SaveToExcelFile](../../aspose.cells.gridweb/mainweb/savetoexcelfile)(string, GridSaveOptions) | 将工作表保存到 excel 文件中。 |
| [SetCustomStyle](../../aspose.cells.gridweb/mainweb/setcustomstyle)(Stream) | 从流中设置自定义样式文件，包括磁盘文件流或内存流。 |
| static [GetVersion](../../aspose.cells.gridweb/gridweb/getversion)() | 获取发布版本。 |
| static [SetFontFolder](../../aspose.cells.gridweb/gridweb/setfontfolder)(string, bool) | 设置字体文件夹 |
| static [SetFontFolders](../../aspose.cells.gridweb/gridweb/setfontfolders)(string[], bool) | 设置字体文件夹 |

### 也可以看看

* class [MainWeb](../mainweb)
* 命名空间 [Aspose.Cells.GridWeb](../../aspose.cells.gridweb)
* 部件 [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
