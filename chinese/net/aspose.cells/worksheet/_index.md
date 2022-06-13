---
title: Worksheet
second_title: Aspose.Cells for .NET API 参考
description: 封装表示单个工作表的对象
type: docs
weight: 6510
url: /zh/net/aspose.cells/worksheet/
---
## Worksheet class

封装表示单个工作表的对象。

```csharp
public class Worksheet : IDisposable
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [ActiveCell](../../aspose.cells/worksheet/activecell) { get; set; } | 获取或设置工作表中的活动单元格。 |
| [AllowEditRanges](../../aspose.cells/worksheet/alloweditranges) { get; } | 获取工作表中的允许编辑范围集合。 |
| [AutoFilter](../../aspose.cells/worksheet/autofilter) { get; } | 表示指定工作表的自动过滤器。 |
| [BackgroundImage](../../aspose.cells/worksheet/backgroundimage) { get; set; } | 获取和设置工作表背景图像。 |
| [Cells](../../aspose.cells/worksheet/cells) { get; } | 获取[`Cells`](./cells)集合。 |
| [CellWatches](../../aspose.cells/worksheet/cellwatches) { get; } | 获取在“监视窗口”中监视的此工作表上的单元格集合。 |
| [Charts](../../aspose.cells/worksheet/charts) { get; } | 获取[`Chart`](../../aspose.cells.charts/chart)集合 |
| [CheckBoxes](../../aspose.cells/worksheet/checkboxes) { get; } | 获取[`CheckBox`](../../aspose.cells.drawing/checkbox)集合。 |
| [CodeName](../../aspose.cells/worksheet/codename) { get; set; } | 获取工作表代码名称。 |
| [Comments](../../aspose.cells/worksheet/comments) { get; } | 获取[`Comment`](../comment)集合。 |
| [ConditionalFormattings](../../aspose.cells/worksheet/conditionalformattings) { get; } | 获取工作表中的 ConditionalFormattings。 |
| [CustomProperties](../../aspose.cells/worksheet/customproperties) { get; } | 获取表示 与工作表关联的标识符信息的对象。 |
| [DisplayRightToLeft](../../aspose.cells/worksheet/displayrighttoleft) { get; set; } | 指示指定的工作表是否从右到左而不是从左到右显示。 默认为假。 |
| [DisplayZeros](../../aspose.cells/worksheet/displayzeros) { get; set; } | 如果显示零值，则为真。 |
| [ErrorCheckOptions](../../aspose.cells/worksheet/errorcheckoptions) { get; } | 获取应用于特定范围的错误检查设置。 |
| [FirstVisibleColumn](../../aspose.cells/worksheet/firstvisiblecolumn) { get; set; } | 表示第一个可见列索引。 |
| [FirstVisibleRow](../../aspose.cells/worksheet/firstvisiblerow) { get; set; } | 表示第一个可见行索引。 |
| [HasAutofilter](../../aspose.cells/worksheet/hasautofilter) { get; } | 指示此工作表是否具有自动过滤器。 |
| [HorizontalPageBreaks](../../aspose.cells/worksheet/horizontalpagebreaks) { get; } | 获取[`HorizontalPageBreakCollection`](../horizontalpagebreakcollection)集合。 |
| [Hyperlinks](../../aspose.cells/worksheet/hyperlinks) { get; } | 获取[`HyperlinkCollection`](../hyperlinkcollection)集合。 |
| [Index](../../aspose.cells/worksheet/index) { get; } | 获取工作表集合中工作表的索引。 |
| [IsGridlinesVisible](../../aspose.cells/worksheet/isgridlinesvisible) { get; set; } | 获取或设置一个值，指示网格线是否可见。默认为 true。 |
| [IsOutlineShown](../../aspose.cells/worksheet/isoutlineshown) { get; set; } | 表示是否显示轮廓。 |
| [IsPageBreakPreview](../../aspose.cells/worksheet/ispagebreakpreview) { get; set; } | 指示指定的工作表是显示在普通视图还是分页预览中。 |
| [IsProtected](../../aspose.cells/worksheet/isprotected) { get; } | 指示工作表是否受保护。 |
| [IsRowColumnHeadersVisible](../../aspose.cells/worksheet/isrowcolumnheadersvisible) { get; set; } | 获取或设置一个值，该值指示工作表是否将显示行和列标题。 默认为真。 |
| [IsRulerVisible](../../aspose.cells/worksheet/isrulervisible) { get; set; } | 表示标尺是否可见。此属性仅适用于分页预览。 |
| [IsSelected](../../aspose.cells/worksheet/isselected) { get; set; } | 表示打开工作簿时是否选择此工作表。 |
| [IsVisible](../../aspose.cells/worksheet/isvisible) { get; set; } | 表示工作表是否可见。 |
| [ListObjects](../../aspose.cells/worksheet/listobjects) { get; } | 获取此工作表中的所有 ListObject。 |
| [Name](../../aspose.cells/worksheet/name) { get; set; } | 获取或设置工作表的名称。 |
| [OleObjects](../../aspose.cells/worksheet/oleobjects) { get; } | 表示工作表中[`OleObject`](../../aspose.cells.drawing/oleobject)的集合。 |
| [Outline](../../aspose.cells/worksheet/outline) { get; } | 获取此工作表的大纲。 |
| [PageSetup](../../aspose.cells/worksheet/pagesetup) { get; } | 表示此表中的页面设置说明。 |
| [PaneState](../../aspose.cells/worksheet/panestate) { get; } | 指示窗格是否有水平或垂直拆分，以及这些拆分是否被冻结。 |
| [Pictures](../../aspose.cells/worksheet/pictures) { get; } | 获取[`Picture`](../../aspose.cells.drawing/picture)集合。 |
| [PivotTables](../../aspose.cells/worksheet/pivottables) { get; } | 获取此工作表中的所有数据透视表。 |
| [Protection](../../aspose.cells/worksheet/protection) { get; } | 表示可用于工作表的各种类型的保护选项。支持 ExcelXP 及以上版本的高级保护选项。 |
| [QueryTables](../../aspose.cells/worksheet/querytables) { get; } | 在工作表中获取[`QueryTableCollection`](../querytablecollection)。 |
| [Scenarios](../../aspose.cells/worksheet/scenarios) { get; } | 获取[`Scenario`](../scenario)的集合。 |
| [Shapes](../../aspose.cells/worksheet/shapes) { get; } | 返回此工作表中的所有绘图形状。 |
| [ShowFormulas](../../aspose.cells/worksheet/showformulas) { get; set; } | 指示是否显示公式或其结果。 |
| [Slicers](../../aspose.cells/worksheet/slicers) { get; } | 获取工作表中的切片器集合 |
| [SmartTagSetting](../../aspose.cells/worksheet/smarttagsetting) { get; } | 获取工作表的所有[`SmartTagCollection`](../../aspose.cells.markup/smarttagcollection)对象。 |
| [SparklineGroupCollection](../../aspose.cells/worksheet/sparklinegroupcollection) { get; } | 获取工作表中的迷你图组集合。 |
| [TabColor](../../aspose.cells/worksheet/tabcolor) { get; set; } | 代表工作表标签颜色。 |
| [TabId](../../aspose.cells/worksheet/tabid) { get; set; } | 指定工作表的内部标识符。 |
| [TextBoxes](../../aspose.cells/worksheet/textboxes) { get; } | 获取[`TextBox`](../../aspose.cells.drawing/textbox)集合。 |
| [Timelines](../../aspose.cells/worksheet/timelines) { get; } | 获取工作表中的 Timeline 集合 |
| [TransitionEntry](../../aspose.cells/worksheet/transitionentry) { get; set; } | 指示是否启用转换公式条目（Lotus 兼容性）选项。 |
| [TransitionEvaluation](../../aspose.cells/worksheet/transitionevaluation) { get; set; } | 指示是否启用转换公式评估（Lotus 兼容性）选项。 |
| [Type](../../aspose.cells/worksheet/type) { get; set; } | 表示工作表类型。 |
| [UniqueId](../../aspose.cells/worksheet/uniqueid) { get; set; } | 获取和设置唯一id，同{15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}。 |
| [Validations](../../aspose.cells/worksheet/validations) { get; } | 获取工作表中的数据验证设置集合。 |
| [VerticalPageBreaks](../../aspose.cells/worksheet/verticalpagebreaks) { get; } | 获取[`VerticalPageBreakCollection`](../verticalpagebreakcollection)集合。 |
| [ViewType](../../aspose.cells/worksheet/viewtype) { get; set; } | 获取和设置视图类型。 |
| [VisibilityType](../../aspose.cells/worksheet/visibilitytype) { get; set; } | 表示此工作表的可见状态。 |
| [Workbook](../../aspose.cells/worksheet/workbook) { get; } | 获取包含此工作表的工作簿对象。 |
| [Zoom](../../aspose.cells/worksheet/zoom) { get; set; } | 以百分比表示比例因子。它应该在 10 到 400 之间。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [AddPageBreaks](../../aspose.cells/worksheet/addpagebreaks)(string) | 添加分页符。 |
| [AdvancedFilter](../../aspose.cells/worksheet/advancedfilter)(bool, string, string, string, bool) | 使用复杂标准过滤数据。 |
| [AutoFitColumn](../../aspose.cells/worksheet/autofitcolumn#autofitcolumn)(int) | 自动调整列宽。 |
| [AutoFitColumn](../../aspose.cells/worksheet/autofitcolumn#autofitcolumn_1)(int, int, int) | 自动调整列宽。 |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns)() | 自动调整此工作表中的所有列。 |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_1)(AutoFitterOptions) | 自动调整此工作表中的所有列。 |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_2)(int, int) | 自动调整列宽。 |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_3)(int, int, AutoFitterOptions) | 自动调整列宽。 |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_4)(int, int, int, int) | 自动调整列宽。 |
| [AutoFitColumns](../../aspose.cells/worksheet/autofitcolumns#autofitcolumns_5)(int, int, int, int, AutoFitterOptions) | 自动调整列宽。 |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow#autofitrow)(int) | 自动调整行高。 |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow#autofitrow_1)(int, int, int) | 自动调整行高。 |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow#autofitrow_2)(int, int, int, AutoFitterOptions) | 自动调整行高。 |
| [AutoFitRow](../../aspose.cells/worksheet/autofitrow#autofitrow_3)(int, int, int, int) | 自动调整矩形范围内的行高。 |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows)() | 自动调整此工作表中的所有行。 |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows_1)(AutoFitterOptions) | 自动调整此工作表中的所有行。 |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows_2)(bool) | 自动调整此工作表中的所有行。 |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows_3)(int, int) | 自动调整范围内的行高。 |
| [AutoFitRows](../../aspose.cells/worksheet/autofitrows#autofitrows_4)(int, int, AutoFitterOptions) | 自动调整范围内的行高。 |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula#calculateformula)(string) | 计算公式。 |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula#calculateformula_2)(CalculationOptions, bool) | 计算此工作表中的所有公式。 |
| [CalculateFormula](../../aspose.cells/worksheet/calculateformula#calculateformula_1)(string, CalculationOptions) | 计算公式。 |
| [ClearComments](../../aspose.cells/worksheet/clearcomments)() | 清除设计器电子表格中的所有注释。 |
| [CloseAccessCache](../../aspose.cells/worksheet/closeaccesscache)(AccessCacheOptions) | 关闭使用缓存访问此工作表中数据的会话。 |
| [Copy](../../aspose.cells/worksheet/copy#copy)(Worksheet) | 从另一个工作表复制内容和格式。 |
| [Copy](../../aspose.cells/worksheet/copy#copy_1)(Worksheet, CopyOptions) | 从另一个工作表复制内容和格式。 |
| [Dispose](../../aspose.cells/worksheet/dispose)() | 执行与释放、释放或 重置非托管资源相关的应用程序定义任务。 |
| [FreezePanes](../../aspose.cells/worksheet/freezepanes#freezepanes_1)(string, int, int) | 在工作表中的指定单元格处冻结窗格。 |
| [FreezePanes](../../aspose.cells/worksheet/freezepanes#freezepanes)(int, int, int, int) | 在工作表中的指定单元格处冻结窗格。 |
| [GetFreezedPanes](../../aspose.cells/worksheet/getfreezedpanes)(out int, out int, out int, out int) | 获取冻结窗格。 |
| [GetPanes](../../aspose.cells/worksheet/getpanes)() | 获取窗口窗格。 |
| [GetPrintingPageBreaks](../../aspose.cells/worksheet/getprintingpagebreaks)(ImageOrPrintOptions) | 获取自动分页符。 |
| [GetSelectedRanges](../../aspose.cells/worksheet/getselectedranges)() | 获取设计器电子表格中选定的单元格范围。 |
| [MoveTo](../../aspose.cells/worksheet/moveto)(int) | 将工作表移动到电子表格中的另一个位置。 |
| [Protect](../../aspose.cells/worksheet/protect#protect)(ProtectionType) | 保护工作表。 |
| [Protect](../../aspose.cells/worksheet/protect#protect_1)(ProtectionType, string, string) | 保护工作表。 |
| [RefreshPivotTables](../../aspose.cells/worksheet/refreshpivottables)() | 刷新此工作表中的所有数据透视表。 |
| [RemoveAllDrawingObjects](../../aspose.cells/worksheet/removealldrawingobjects)() | 删除此工作表中的所有绘图对象。 |
| [RemoveAutoFilter](../../aspose.cells/worksheet/removeautofilter)() | 删除工作表的自动过滤器。 |
| [RemoveSplit](../../aspose.cells/worksheet/removesplit)() | 移除分割窗口。 |
| [Replace](../../aspose.cells/worksheet/replace)(string, string) | 用新字符串替换所有单元格的文本。 |
| [SelectRange](../../aspose.cells/worksheet/selectrange)(int, int, int, int, bool) | 选择一个范围。 |
| [SetVisible](../../aspose.cells/worksheet/setvisible)(bool, bool) | 设置可见选项。 |
| [Split](../../aspose.cells/worksheet/split)() | 拆分窗口。 |
| [StartAccessCache](../../aspose.cells/worksheet/startaccesscache)(AccessCacheOptions) | 启动使用缓存访问此工作表中数据的会话。 |
| override [ToString](../../aspose.cells/worksheet/tostring)() | 返回代表当前 Worksheet 对象的字符串。 |
| [UnFreezePanes](../../aspose.cells/worksheet/unfreezepanes)() | 解冻工作表中的窗格。 |
| [Unprotect](../../aspose.cells/worksheet/unprotect#unprotect)() | 取消保护工作表。 |
| [Unprotect](../../aspose.cells/worksheet/unprotect#unprotect_1)(string) | 取消保护工作表。 |
| [XmlMapQuery](../../aspose.cells/worksheet/xmlmapquery)(string, XmlMap) | 查询映射/链接到xml映射特定路径的单元格区域。 |

### 例子

```csharp
[C#]

Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

 //在“AS40”处冻结10行10列的窗格
sheet.FreezePanes("AS40", 10, 10);

//在单元格A1

sheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

[Visual Basic]

Dim workbook as Workbook = new Workbook()

Dim sheet as Worksheet = workbook.Worksheets(0)

'Freeze panes at "AS40" with 10 rows and 10 columns
sheet.FreezePanes("AS40", 10, 10)

'Add a hyperlink in Cell A1
sheet.Hyperlinks.Add("A1", 1, 1, "http: //www.aspose.com")
```

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
