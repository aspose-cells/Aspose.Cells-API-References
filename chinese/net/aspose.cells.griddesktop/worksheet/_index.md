---
title: Worksheet
second_title: Aspose.Cells for .NET API 参考
description: 封装表示单个工作表的对象
type: docs
weight: 1080
url: /zh/net/aspose.cells.griddesktop/worksheet/
---
## Worksheet class

封装表示单个工作表的对象。

```csharp
public class Worksheet
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [ActiveCell](../../aspose.cells.griddesktop/worksheet/activecell) { get; set; } |  |
| [AllowSelectingLockedCell](../../aspose.cells.griddesktop/worksheet/allowselectinglockedcell) { get; set; } | 表示是否允许用户选择受保护工作表上的锁定单元格。 |
| [BackgroundImage](../../aspose.cells.griddesktop/worksheet/backgroundimage) { get; set; } | 获取和设置工作表背景图片。 |
| [Cells](../../aspose.cells.griddesktop/worksheet/cells) { get; } |  |
| [CodeName](../../aspose.cells.griddesktop/worksheet/codename) { get; } | 代表工作表代号。 |
| [Columns](../../aspose.cells.griddesktop/worksheet/columns) { get; } |  |
| [ColumnsCount](../../aspose.cells.griddesktop/worksheet/columnscount) { get; set; } |  |
| [Comments](../../aspose.cells.griddesktop/worksheet/comments) { get; } |  |
| [Controls](../../aspose.cells.griddesktop/worksheet/controls) { get; } | 获取单元格控件集合。 |
| [CustomColumnCaption](../../aspose.cells.griddesktop/worksheet/customcolumncaption) { get; set; } | 获取或设置工作表的自定义列标题。 |
| [CustomRowCaption](../../aspose.cells.griddesktop/worksheet/customrowcaption) { get; set; } | 获取或设置工作表的自定义行标题。 |
| [DataMember](../../aspose.cells.griddesktop/worksheet/datamember) { get; } | 获取工作表对象为其显示数据的数据源。 |
| [DataSource](../../aspose.cells.griddesktop/worksheet/datasource) { get; } | 获取工作表对象的数据源中的特定列表。 |
| [DisplayRightToLeft](../../aspose.cells.griddesktop/worksheet/displayrighttoleft) { get; set; } |  |
| [DisplayZeros](../../aspose.cells.griddesktop/worksheet/displayzeros) { get; set; } | 如果显示零值则为真。 |
| [FirstVisibleColumn](../../aspose.cells.griddesktop/worksheet/firstvisiblecolumn) { get; set; } |  |
| [FirstVisibleRow](../../aspose.cells.griddesktop/worksheet/firstvisiblerow) { get; set; } | 表示第一个可见行索引。 |
| [FrozenCols](../../aspose.cells.griddesktop/worksheet/frozencols) { get; set; } | 获取或设置工作表的冻结列数。 冻结将从第一列开始。 |
| [FrozenRows](../../aspose.cells.griddesktop/worksheet/frozenrows) { get; set; } | 获取或设置工作表的冻结行数。 冻结将从第一行开始。 |
| [GridDesktop](../../aspose.cells.griddesktop/worksheet/griddesktop) { get; } | 获取 Sheet 的 GridDesktop 对象。 |
| [GridlinesVisible](../../aspose.cells.griddesktop/worksheet/gridlinesvisible) { get; set; } | 获取或设置网格线是否可见。默认为真。 |
| [Hyperlinks](../../aspose.cells.griddesktop/worksheet/hyperlinks) { get; } | 获取HyperlinkCollection集合. |
| [Index](../../aspose.cells.griddesktop/worksheet/index) { get; } | 获取工作表集合中工作表的索引。 |
| [IsVeryHidden](../../aspose.cells.griddesktop/worksheet/isveryhidden) { get; set; } | 指示工作表是否隐藏并且无法在用户界面 (UI) 中显示。 |
| [IsVisible](../../aspose.cells.griddesktop/worksheet/isvisible) { get; set; } |  |
| [MergesCount](../../aspose.cells.griddesktop/worksheet/mergescount) { get; } | 获取合并的计数 |
| [Name](../../aspose.cells.griddesktop/worksheet/name) { get; set; } | 获取或设置工作表的名称。 |
| [OutlineShown](../../aspose.cells.griddesktop/worksheet/outlineshown) { get; set; } | 表示是否显示大纲。 |
| [Pictures](../../aspose.cells.griddesktop/worksheet/pictures) { get; } | 得到一个[`Pictures`](./pictures)集合. |
| [PivotTables](../../aspose.cells.griddesktop/worksheet/pivottables) { get; } | 获取工作表中的数据透视表。 |
| [Protected](../../aspose.cells.griddesktop/worksheet/protected) { get; set; } |  |
| [RowFilter](../../aspose.cells.griddesktop/worksheet/rowfilter) { get; } | 获取工作表的 RowFilterSettings 对象。 |
| [Rows](../../aspose.cells.griddesktop/worksheet/rows) { get; } |  |
| [RowsCount](../../aspose.cells.griddesktop/worksheet/rowscount) { get; set; } |  |
| [Selected](../../aspose.cells.griddesktop/worksheet/selected) { get; set; } | 表示打开工作簿时是否选择此工作表。 |
| [Shapes](../../aspose.cells.griddesktop/worksheet/shapes) { get; } | 得到一个[`Pictures`](./pictures)集合. |
| [ShowGridlines](../../aspose.cells.griddesktop/worksheet/showgridlines) { get; set; } |  |
| [TabColor](../../aspose.cells.griddesktop/worksheet/tabcolor) { get; set; } | 代表工作表标签颜色。 |
| [Validations](../../aspose.cells.griddesktop/worksheet/validations) { get; } | 获取工作表中的数据验证设置集合。 |
| [Visible](../../aspose.cells.griddesktop/worksheet/visible) { get; set; } | 表示工作表是否可见。 |
| [Workbook](../../aspose.cells.griddesktop/worksheet/workbook) { get; } |  |
| [Zoom](../../aspose.cells.griddesktop/worksheet/zoom) { get; set; } | 以百分比表示比例因子。它应该在 10 到 400 之间。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [AddAutoFilter](../../aspose.cells.griddesktop/worksheet/addautofilter)(int, int, int) | 设置应用指定自动筛选的范围。 |
| [AddColumn](../../aspose.cells.griddesktop/worksheet/addcolumn)() | 添加一个新列。 |
| [AddCustomFilter](../../aspose.cells.griddesktop/worksheet/addcustomfilter#addcustomfilter_1)(int, string) | 为指定行添加自定义过滤器。 |
| [AddCustomFilter](../../aspose.cells.griddesktop/worksheet/addcustomfilter#addcustomfilter)(int, int, object[], GridFilterOperatorType[]) | 为从开始行到结束行的指定行范围添加自定义过滤器。 |
| [AddRow](../../aspose.cells.griddesktop/worksheet/addrow)() | 添加一个新行。 |
| [AddSelectedRange](../../aspose.cells.griddesktop/worksheet/addselectedrange)(CellRange) | 向工作表添加一个新的选定范围。 |
| [AutoFitColumn](../../aspose.cells.griddesktop/worksheet/autofitcolumn#autofitcolumn)(int) | 自动调整列宽。 |
| [AutoFitColumn](../../aspose.cells.griddesktop/worksheet/autofitcolumn#autofitcolumn_1)(int, int, int) | 自动调整列宽。 |
| [AutoFitColumns](../../aspose.cells.griddesktop/worksheet/autofitcolumns#autofitcolumns)() | 自动调整此工作表中的所有列。 |
| [AutoFitColumns](../../aspose.cells.griddesktop/worksheet/autofitcolumns#autofitcolumns_1)(int, int) | 自动调整列宽。 |
| [AutoFitColumns](../../aspose.cells.griddesktop/worksheet/autofitcolumns#autofitcolumns_2)(int, int, int, int) | 自动调整列宽。 |
| [AutoFitRow](../../aspose.cells.griddesktop/worksheet/autofitrow#autofitrow)(int) | 自动调整行高。 |
| [AutoFitRow](../../aspose.cells.griddesktop/worksheet/autofitrow#autofitrow_1)(int, int, int) | 自动调整行高。 |
| [AutoFitRow](../../aspose.cells.griddesktop/worksheet/autofitrow#autofitrow_2)(int, int, int, int) | 在矩形范围内自动调整行高。 |
| [AutoFitRows](../../aspose.cells.griddesktop/worksheet/autofitrows#autofitrows)() | 自动调整此工作表中的所有行。 |
| [AutoFitRows](../../aspose.cells.griddesktop/worksheet/autofitrows#autofitrows_1)(int, int) | 自动调整范围内的行高。 |
| [AutoFitRowsMerged](../../aspose.cells.griddesktop/worksheet/autofitrowsmerged)() | 自动调整此工作表中的所有行。当单元格合并成一行时，它也会自动调整行高。 |
| [CalculateFormula](../../aspose.cells.griddesktop/worksheet/calculateformula)(string) | 计算公式。 |
| [CellInMerged](../../aspose.cells.griddesktop/worksheet/cellinmerged)(CellLocation) | 获取指定单元格位置是否在合并中的值。 |
| [CellRangeInMerge](../../aspose.cells.griddesktop/worksheet/cellrangeinmerge)(CellRange) | 获取一个值，该值指示指定单元格范围是否合并。 |
| [ClearComments](../../aspose.cells.griddesktop/worksheet/clearcomments)() | 清除设计器电子表格中的所有注释。 |
| [ClearMerges](../../aspose.cells.griddesktop/worksheet/clearmerges)() | 清除所有合并。 |
| [ClearSelection](../../aspose.cells.griddesktop/worksheet/clearselection)() | 清除工作表中的选择。 |
| [ColInMerged](../../aspose.cells.griddesktop/worksheet/colinmerged)(int) | 获取一个值，该值指示是否合并中的指定列。 |
| [ColInSelection](../../aspose.cells.griddesktop/worksheet/colinselection)(int) | 判断索引处的指定列是否处于选中状态。 |
| [Copy](../../aspose.cells.griddesktop/worksheet/copy)(Worksheet) | 从另一个工作表复制内容和格式。 |
| [CreateRange](../../aspose.cells.griddesktop/worksheet/createrange#createrange_1)(string, string) |  |
| [CreateRange](../../aspose.cells.griddesktop/worksheet/createrange#createrange)(int, int, int, int) |  |
| [DataBind](../../aspose.cells.griddesktop/worksheet/databind)(object, string) | 将数据源对象中的数据与 Worksheet 对象绑定。 |
| [DataUnbind](../../aspose.cells.griddesktop/worksheet/dataunbind)() | 将数据源对象中的数据与 Worksheet 对象解除绑定。 |
| [ExportDataTable](../../aspose.cells.griddesktop/worksheet/exportdatatable#exportdatatable_1)(DataTable, int, int, int, int, bool) | 将 Worksheet 的 Cells 集合中的数据导出到指定的 DataTable 对象。 |
| [ExportDataTable](../../aspose.cells.griddesktop/worksheet/exportdatatable#exportdatatable)(int, int, int, int, bool, bool) | 将工作表的 Cells 集合中的数据导出到新的 DataTable 对象。 |
| [FilterString](../../aspose.cells.griddesktop/worksheet/filterstring)(int, string) | 为列设置过滤器。请注意，我们将在调用 filterString 过滤条件字符串之前调用 AddAutoFilter。注意我们使用 comma-&gt;"," 作为拆分字符，因此您要过滤的单元格值不应包含 comma filterString(10,"123,456") 表示第 10 列应包含 123 或 456，filterString(10,"123" ) 表示第 10 列应包含 123 用逗号分隔值，例如。 123,456,789 或 abc |
| [FreezePanes](../../aspose.cells.griddesktop/worksheet/freezepanes#freezepanes_1)(string, int, int) | 在工作表中的指定单元格处冻结窗格。 |
| [FreezePanes](../../aspose.cells.griddesktop/worksheet/freezepanes#freezepanes)(int, int, int, int) | 在工作表中的指定单元格处冻结窗格。 |
| [GetAllSelectedRanges](../../aspose.cells.griddesktop/worksheet/getallselectedranges)() | 获取此工作表的所有选定范围。 |
| [GetCellLocationByClientPoint](../../aspose.cells.griddesktop/worksheet/getcelllocationbyclientpoint)(Point) | 通过客户端坐标点获取单元格位置。 |
| [GetColumnCaption](../../aspose.cells.griddesktop/worksheet/getcolumncaption)(int) | 获取列标题。如果未设置标题，则返回空字符串。 |
| [GetFirstVisibleColumn](../../aspose.cells.griddesktop/worksheet/getfirstvisiblecolumn)() | 获取工作表视图的第一个可见列索引。 |
| [GetFirstVisibleRow](../../aspose.cells.griddesktop/worksheet/getfirstvisiblerow)() | 获取工作表视图的第一个可见行索引。 |
| [GetFocusedCell](../../aspose.cells.griddesktop/worksheet/getfocusedcell)() | 获取焦点单元格。 |
| [GetFocusedCellLocation](../../aspose.cells.griddesktop/worksheet/getfocusedcelllocation)() | 获取一个被聚焦的单元格位置。 |
| [GetFreezedPanes](../../aspose.cells.griddesktop/worksheet/getfreezedpanes)(out int, out int, out int, out int) | 获取冻结窗格。 |
| [GetIsReadonly](../../aspose.cells.griddesktop/worksheet/getisreadonly)(int, int) | 获取单元格是否为只读。这是GridWeb的扩展属性，不会保留在实际的excel文件中 |
| [GetLastSelection](../../aspose.cells.griddesktop/worksheet/getlastselection)() | 获取上次选择的单元格范围。 |
| [GetMerge](../../aspose.cells.griddesktop/worksheet/getmerge)(int) | 获取指定索引处合并的单元格范围。 |
| [GetMergeByCell](../../aspose.cells.griddesktop/worksheet/getmergebycell)(int, int) | 获取包含行、列位置单元格的合并区域，如果所有合并区域都不包含该单元格位置，则返回null |
| [GroupColumns](../../aspose.cells.griddesktop/worksheet/groupcolumns#groupcolumns)(int, int) | 对列进行分组。 |
| [GroupColumns](../../aspose.cells.griddesktop/worksheet/groupcolumns#groupcolumns_1)(int, int, bool, bool) | 对列进行分组。 |
| [GroupColumns](../../aspose.cells.griddesktop/worksheet/groupcolumns#groupcolumns_2)(int, int, int, bool) | 对列进行分组。 |
| [GroupRows](../../aspose.cells.griddesktop/worksheet/grouprows#grouprows)(int, int) | 对行进行分组。 |
| [GroupRows](../../aspose.cells.griddesktop/worksheet/grouprows#grouprows_1)(int, int, bool) | 对行进行分组。 |
| [GroupRows](../../aspose.cells.griddesktop/worksheet/grouprows#grouprows_2)(int, int, bool, bool) | 对行进行分组。 |
| [GroupRows](../../aspose.cells.griddesktop/worksheet/grouprows#grouprows_3)(int, int, int, bool) | 对行进行分组。 |
| [GroupRows](../../aspose.cells.griddesktop/worksheet/grouprows#grouprows_4)(int, int, int, bool, bool) | 对行进行分组。 |
| [ImportDataTable](../../aspose.cells.griddesktop/worksheet/importdatatable)(DataTable, bool, int, int) | 将 DataTable 对象导入工作表。 |
| [InSelection](../../aspose.cells.griddesktop/worksheet/inselection)(CellLocation) | 判断指定的单元格位置是否处于选中状态 |
| [InsertColumn](../../aspose.cells.griddesktop/worksheet/insertcolumn)(int) | 插入一个新列。 |
| [InsertRow](../../aspose.cells.griddesktop/worksheet/insertrow)(int) | 插入新行。 |
| [IsCellFocused](../../aspose.cells.griddesktop/worksheet/iscellfocused)() | 确定单元格是否被聚焦。 |
| [IsProtected](../../aspose.cells.griddesktop/worksheet/isprotected)() | 指示工作表是否受保护。 |
| [Merge](../../aspose.cells.griddesktop/worksheet/merge)(CellRange) | 将指定范围的单元格合并为一个单元格。 |
| [MergeFocused](../../aspose.cells.griddesktop/worksheet/mergefocused)(CellLocation) | 获取焦点合并的索引。 |
| [MoveTo](../../aspose.cells.griddesktop/worksheet/moveto)(int) | 将工作表移动到电子表格中的另一个位置。 |
| [RefreshFilter](../../aspose.cells.griddesktop/worksheet/refreshfilter)() | 刷新自动过滤器以隐藏或取消隐藏行。 |
| [RemoveAutoFilter](../../aspose.cells.griddesktop/worksheet/removeautofilter)() | 移除工作表的自动过滤器。 |
| [RemoveColumn](../../aspose.cells.griddesktop/worksheet/removecolumn)(int) | 删除指定索引处的列。 |
| [RemoveRow](../../aspose.cells.griddesktop/worksheet/removerow)(int) | 删除指定索引处的行。 |
| [ResetFilter](../../aspose.cells.griddesktop/worksheet/resetfilter)(int) | 将过滤器类型重置为无 |
| [ResetFilters](../../aspose.cells.griddesktop/worksheet/resetfilters)(int, int) | 将过滤器类型重置为无 |
| [RowInMerged](../../aspose.cells.griddesktop/worksheet/rowinmerged)(int) | 获取一个值，该值指示是否合并中的指定行。 |
| [RowInSelection](../../aspose.cells.griddesktop/worksheet/rowinselection)(int) | 判断索引处的指定行是否处于选中状态。 |
| [SetAllCellsEditable](../../aspose.cells.griddesktop/worksheet/setallcellseditable)() | 使所有单元格可编辑。这是扩展属性 |
| [SetAllCellsReadonly](../../aspose.cells.griddesktop/worksheet/setallcellsreadonly)() | 使所有单元格只读。这是扩展属性 注意此属性不能保留在实际单元格中，如果要保留保护请使用 setProtect |
| [SetColumnCaption](../../aspose.cells.griddesktop/worksheet/setcolumncaption)(int, string) | 为列设置标题。请注意这是一个扩展属性，不能保留在 excel 文件中 |
| [SetFirstVisibleColumn](../../aspose.cells.griddesktop/worksheet/setfirstvisiblecolumn)(int) | 设置工作表视图的第一个可见列索引。 |
| [SetFirstVisibleRow](../../aspose.cells.griddesktop/worksheet/setfirstvisiblerow)(int) | 设置工作表视图的第一个可见行索引。 |
| [SetFocusedCell](../../aspose.cells.griddesktop/worksheet/setfocusedcell#setfocusedcell)(CellLocation) | 将单元格焦点设置在指定位置。 |
| [SetFocusedCell](../../aspose.cells.griddesktop/worksheet/setfocusedcell#setfocusedcell_1)(int, int) | 将单元格焦点设置在指定的列和行。 |
| [SetFont](../../aspose.cells.griddesktop/worksheet/setfont)(CellRange, Font) | 将字体对象设置为 cellRange. |
| [SetFontColor](../../aspose.cells.griddesktop/worksheet/setfontcolor)(CellRange, Color) | 将字体颜色设置为 cellRange. |
| [SetIsReadonly](../../aspose.cells.griddesktop/worksheet/setisreadonly)(int, int, bool) | 设置单元格是否为只读。这是一个扩展属性，它不会保留在实际的excel文件中 |
| [SetProtect](../../aspose.cells.griddesktop/worksheet/setprotect)() | 保护工作表。 |
| [SetProtected](../../aspose.cells.griddesktop/worksheet/setprotected)(CellRange, bool) | 设置cellRange是否受保护。这是一个扩展方法，只在Grid中使用。 该方法与cell.Style.CellLocked属性无关 保存到excel文件后不会生效。 |
| [SetStyle](../../aspose.cells.griddesktop/worksheet/setstyle#setstyle)(CellRange, Style) | 将样式对象设置为 cellRange. |
| [SetStyle](../../aspose.cells.griddesktop/worksheet/setstyle#setstyle_1)(GridCellArea, Style) | 将样式对象设置为 cellRange. |
| [UnFreezePanes](../../aspose.cells.griddesktop/worksheet/unfreezepanes)() | 解冻工作表中的窗格。 |
| [UngroupColumns](../../aspose.cells.griddesktop/worksheet/ungroupcolumns#ungroupcolumns)(int, int) | 取消组合列。 |
| [UngroupColumns](../../aspose.cells.griddesktop/worksheet/ungroupcolumns#ungroupcolumns_1)(int, int, bool) | 取消组合列。 |
| [UngroupRows](../../aspose.cells.griddesktop/worksheet/ungrouprows#ungrouprows)(int, int) | 取消组合行。 |
| [UngroupRows](../../aspose.cells.griddesktop/worksheet/ungrouprows#ungrouprows_1)(int, int, bool) | 取消组合行。 |
| [Unmerge](../../aspose.cells.griddesktop/worksheet/unmerge#unmerge)(CellLocation) | 从合并中删除指定的单元格位置。 |
| [Unmerge](../../aspose.cells.griddesktop/worksheet/unmerge#unmerge_1)(CellRange) | 将指定范围的单元格取消合并为单个单元格。 |
| [Unmerge](../../aspose.cells.griddesktop/worksheet/unmerge#unmerge_2)(int, int) | 从合并中删除指定的单元格行列索引。 |
| [UnProtect](../../aspose.cells.griddesktop/worksheet/unprotect)() | 取消保护工作表。 |
| static [CellIndexToR1C1](../../aspose.cells.griddesktop/worksheet/cellindextor1c1)(int, int) | 根据行列索引获取单元格r1c1样式名称。 |

## 字段

| 姓名 | 描述 |
| --- | --- |
| static [DEFAULT_COLUMNSCOUNT](../../aspose.cells.griddesktop/worksheet/default_columnscount) | 工作表的默认列数。 |
| static [DEFAULT_ROWSCOUNT](../../aspose.cells.griddesktop/worksheet/default_rowscount) | 工作表的默认行数。 |

### 也可以看看

* 命名空间 [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop)
* 部件 [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
