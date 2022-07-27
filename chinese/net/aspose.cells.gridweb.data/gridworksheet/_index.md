---
title: GridWorksheet
second_title: Aspose.Cells for .NET API 参考
description: 封装表示单个工作表的对象
type: docs
weight: 570
url: /zh/net/aspose.cells.gridweb.data/gridworksheet/
---
## GridWorksheet class

封装表示单个工作表的对象。

```csharp
public class GridWorksheet : Control, ISerializable
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [ActiveCell](../../aspose.cells.gridweb.data/gridworksheet/activecell) { get; set; } |  |
| [BackgroundImage](../../aspose.cells.gridweb.data/gridworksheet/backgroundimage) { get; set; } | 获取和设置工作表背景图片。 |
| [BindColumns](../../aspose.cells.gridweb.data/gridworksheet/bindcolumns) { get; } | 绑定列集合。 |
| [BindingSource](../../aspose.cells.gridweb.data/gridworksheet/bindingsource) { get; } | 在运行时实际绑定的数据源对象。当 DataSource 属性是 DataSet、DataTable 或 DataView 对象时，它是一个 DataView 对象。 |
| [BindStartColumn](../../aspose.cells.gridweb.data/gridworksheet/bindstartcolumn) { get; set; } | 在数据绑定模式下，BindStartRow 和 BindStartColumn 表示网格的位置来绑定数据源。 |
| [BindStartRow](../../aspose.cells.gridweb.data/gridworksheet/bindstartrow) { get; set; } | 在数据绑定模式下，BindStartRow 和 BindStartColumn 表示网格的位置来绑定数据源。 |
| [Cells](../../aspose.cells.gridweb.data/gridworksheet/cells) { get; } |  |
| [CodeName](../../aspose.cells.gridweb.data/gridworksheet/codename) { get; } | 代表工作表代号。 |
| [Comments](../../aspose.cells.gridweb.data/gridworksheet/comments) { get; } |  |
| [CurrentBindRows](../../aspose.cells.gridweb.data/gridworksheet/currentbindrows) { get; set; } | 获取数据绑定模式下的绑定行数。 |
| [DataMember](../../aspose.cells.gridweb.data/gridworksheet/datamember) { get; set; } | 从多成员DataSource中获取或设置DataMember。 一般表示DataSet的DataTable对象。 |
| [DataSource](../../aspose.cells.gridweb.data/gridworksheet/datasource) { get; set; } | 获取或设置DataSource。 一般是DataSet对象。 |
| [DisplayRightToLeft](../../aspose.cells.gridweb.data/gridworksheet/displayrighttoleft) { get; set; } |  |
| [DisplayZeros](../../aspose.cells.gridweb.data/gridworksheet/displayzeros) { get; set; } | 如果显示零值则为真。 |
| [EnableCreateBindColumnHeader](../../aspose.cells.gridweb.data/gridworksheet/enablecreatebindcolumnheader) { get; set; } | 在数据绑定模式下，表示是否在工作表中创建绑定列标题标题。 |
| [FirstVisibleColumn](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblecolumn) { get; set; } |  |
| [FirstVisibleRow](../../aspose.cells.gridweb.data/gridworksheet/firstvisiblerow) { get; set; } |  |
| [GridActiveCell](../../aspose.cells.gridweb.data/gridworksheet/gridactivecell) { get; set; } |  |
| [Hyperlinks](../../aspose.cells.gridweb.data/gridworksheet/hyperlinks) { get; } | 获取HyperlinkCollection集合. |
| [Index](../../aspose.cells.gridweb.data/gridworksheet/index) { get; } |  |
| [IsGridlinesVisible](../../aspose.cells.gridweb.data/gridworksheet/isgridlinesvisible) { get; set; } | 获取或设置网格线是否可见的值。默认为true。 |
| [IsSummaryRowBelow](../../aspose.cells.gridweb.data/gridworksheet/issummaryrowbelow) { get; set; } | 指示摘要行是否将位于大纲中的详细信息行下方。 |
| [Name](../../aspose.cells.gridweb.data/gridworksheet/name) { get; set; } | 获取或设置工作表的名称。 |
| [OutlineShown](../../aspose.cells.gridweb.data/gridworksheet/outlineshown) { get; set; } | 表示是否显示大纲。 |
| [Pictures](../../aspose.cells.gridweb.data/gridworksheet/pictures) { get; } | 得到一个[`Pictures`](./pictures)集合. |
| [PivotTables](../../aspose.cells.gridweb.data/gridworksheet/pivottables) { get; } | 获取工作表中的数据透视表。 |
| [Selected](../../aspose.cells.gridweb.data/gridworksheet/selected) { get; set; } | 表示打开工作簿时是否选择此工作表。 |
| [Shapes](../../aspose.cells.gridweb.data/gridworksheet/shapes) { get; } | 得到一个[`Pictures`](./pictures)集合. |
| [StandardHeight](../../aspose.cells.gridweb.data/gridworksheet/standardheight) { get; set; } | 获取或设置此工作表的默认行高，以点为单位。 |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridworksheet/standardheightpixels) { get; set; } | 获取或设置此工作表中的默认行高，以像素为单位。 |
| [TabColor](../../aspose.cells.gridweb.data/gridworksheet/tabcolor) { get; set; } | 代表工作表标签颜色。 |
| [Validations](../../aspose.cells.gridweb.data/gridworksheet/validations) { get; } | 获取工作表中的数据验证设置集合。 |
| override [Visible](../../aspose.cells.gridweb.data/gridworksheet/visible) { get; set; } | 指示此工作表的名称是否显示在控件的工作表选项卡中。 |
| [Workbook](../../aspose.cells.gridweb.data/gridworksheet/workbook) { get; } |  |
| [Zoom](../../aspose.cells.gridweb.data/gridworksheet/zoom) { get; set; } |  |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [AddAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/addautofilter)(int, int, int) | 设置应用指定自动筛选的范围。 |
| [AddCustomFilter](../../aspose.cells.gridweb.data/gridworksheet/addcustomfilter)(int, string) | 为指定行添加自定义过滤器。 |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn#autofitcolumn)(int) | 自动调整列宽。 |
| [AutoFitColumn](../../aspose.cells.gridweb.data/gridworksheet/autofitcolumn#autofitcolumn_1)(int, int, int) | 自动调整列宽。 |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow#autofitrow)(int) | 自动调整行高。 |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow#autofitrow_1)(int, int, int) | 自动调整行高。 |
| [AutoFitRow](../../aspose.cells.gridweb.data/gridworksheet/autofitrow#autofitrow_2)(int, int, int, int) | 在矩形范围内自动调整行高。 |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows#autofitrows)() | 自动调整此工作表中的所有行。 |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows#autofitrows_1)(bool) | 自动调整此工作表中的所有行。 |
| [AutoFitRows](../../aspose.cells.gridweb.data/gridworksheet/autofitrows#autofitrows_2)(int, int) | 自动调整范围内的行高。 |
| [CalculateFormula](../../aspose.cells.gridweb.data/gridworksheet/calculateformula)(string) | 计算公式。 |
| [CancelNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/cancelnewbindrow)() | 取消并删除新添加的绑定行。 |
| [ClearComments](../../aspose.cells.gridweb.data/gridworksheet/clearcomments)() | 清除设计器电子表格中的所有注释。 |
| [CommitNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/commitnewbindrow)() | 提交新添加的绑定行并将其添加到数据源。 |
| [Copy](../../aspose.cells.gridweb.data/gridworksheet/copy)(GridWorksheet) | 从另一个工作表复制内容和格式。 |
| [CreateAutoGenratedColumns](../../aspose.cells.gridweb.data/gridworksheet/createautogenratedcolumns)() | 为工作表设置数据源后，调用该方法自动生成绑定列 |
| [CreateNewBindRow](../../aspose.cells.gridweb.data/gridworksheet/createnewbindrow)() | 创建一个新的绑定行并绑定到数据源。 |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal#createsubtotal)(int, int, int, SubtotalFunction, int[]) | 在工作表中创建小计。 |
| [CreateSubtotal](../../aspose.cells.gridweb.data/gridworksheet/createsubtotal#createsubtotal_1)(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) | 在工作表中创建小计。 |
| override [DataBind](../../aspose.cells.gridweb.data/gridworksheet/databind)() | 将工作表绑定到数据源。 |
| [DataSourceControlUpdate](../../aspose.cells.gridweb.data/gridworksheet/datasourcecontrolupdate)(AccessDataSource) | 将工作表绑定到数据源。 |
| [DeleteBindRow](../../aspose.cells.gridweb.data/gridworksheet/deletebindrow)(int) | 删除绑定行。 |
| [FilterString](../../aspose.cells.gridweb.data/gridworksheet/filterstring)(int, string) | 为列设置过滤器。请注意，我们将在调用 filterString 过滤条件字符串之前调用 AddAutoFilter。注意我们使用 comma-&gt;"," 作为拆分字符，因此您要过滤的单元格值不应包含 comma filterString(10,"123,456") 表示第 10 列应包含 123 或 456，filterString(10,"123" ) 表示第 10 列应包含 123 用逗号分隔值，例如。 123,456,789 或 abc |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes#freezepanes_1)(string, int, int) | 在工作表中的指定单元格处冻结窗格。 |
| [FreezePanes](../../aspose.cells.gridweb.data/gridworksheet/freezepanes#freezepanes)(int, int, int, int) | 在工作表中的指定单元格处冻结窗格。 |
| [GetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/getcolumncaption)(int) | 获取列标题。如果未设置标题，则返回空字符串。 |
| [GetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getcolumnheadertooltip)(int) | 获取列标题的工具提示文本。 |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/getcolumnreadonly)(int) | 获取列是否为只读。 这是GridWeb专门的扩展方法，在实际的excel文件中不会保留和生效 |
| [GetFreezedPanes](../../aspose.cells.gridweb.data/gridworksheet/getfreezedpanes)(out int, out int, out int, out int) | 获取冻结窗格。 |
| [GetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/getisreadonly)(int, int) | 获取单元格是否为只读。这是GridWeb的扩展属性，不会保留在实际的excel文件中 |
| [GetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/getrowcaption)(int) | 获取行标题。如果未设置标题，则返回空字符串。 |
| [GetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/getrowheadertooltip)(int) | 获取行标题的工具提示文本。 |
| [GetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/getrowreadonly)(int) | 获取一行是否为只读。 这是GridWeb专门的扩展方法，在实际的excel文件中不会保留和生效 |
| [GroupRows](../../aspose.cells.gridweb.data/gridworksheet/grouprows)(int, int, bool) | 对行进行分组。 |
| [IsProtected](../../aspose.cells.gridweb.data/gridworksheet/isprotected)() | 指示工作表是否受保护。 |
| [MoveTo](../../aspose.cells.gridweb.data/gridworksheet/moveto)(int) | 将工作表移动到电子表格中的另一个位置。 |
| [RefreshFilter](../../aspose.cells.gridweb.data/gridworksheet/refreshfilter)() | 刷新自动过滤器以隐藏或取消隐藏行。 |
| [RemoveAutoFilter](../../aspose.cells.gridweb.data/gridworksheet/removeautofilter)() | 移除工作表的自动过滤器。 |
| [RemoveSubtotal](../../aspose.cells.gridweb.data/gridworksheet/removesubtotal)() | 删除工作表中由 CreateSubtotal 方法创建的小计。 |
| [ResetFilter](../../aspose.cells.gridweb.data/gridworksheet/resetfilter)(int) | 您要应用的字段的整数偏移量，基于第一个过滤器 column （从列表的左侧开始；最左侧的字段是字段 0）。 |
| [SetAllCellsEditable](../../aspose.cells.gridweb.data/gridworksheet/setallcellseditable)() | 使所有单元格可编辑。这是扩展属性 |
| [SetAllCellsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setallcellsreadonly)() | 使所有单元格只读。这是扩展属性 注意此属性不能保留在实际单元格中，如果要保留保护请使用 setProtect |
| [SetColumnCaption](../../aspose.cells.gridweb.data/gridworksheet/setcolumncaption)(int, string) | 为列设置标题。请注意这是一个扩展属性，不能保留在 excel 文件中 |
| [SetColumnHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setcolumnheadertooltip)(int, string) | 设置列标题的工具提示文本。 |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/gridworksheet/setcolumnreadonly)(int, bool) | 将列设置为只读，因此用户不能从客户端删除它。 这是GridWeb专门的扩展方法，在实际的excel文件中不会保留和生效 |
| [SetEditableRange](../../aspose.cells.gridweb.data/gridworksheet/seteditablerange)(int, int, int, int) | 使一系列单元格可编辑。 http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells 通过调用SetAllCellsReadonly方法使所有单元格只读。 然后调用此方法指定可编辑的单元格范围 |
| [SetIsReadonly](../../aspose.cells.gridweb.data/gridworksheet/setisreadonly)(int, int, bool) | 设置单元格是否为只读。这是GridWeb的扩展属性，不会保留在实际的excel文件中 |
| [SetProtect](../../aspose.cells.gridweb.data/gridworksheet/setprotect)() | 保护工作表。 |
| [SetReadonlyRange](../../aspose.cells.gridweb.data/gridworksheet/setreadonlyrange)(int, int, int, int) | 使一系列单元格只读。 http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells 首先通过调用SetAllCellsEditable方法使所有单元格可编辑。 然后调用此方法指定要只读的单元格范围 |
| [SetRowCaption](../../aspose.cells.gridweb.data/gridworksheet/setrowcaption)(int, string) | 设置行的标题。 |
| [SetRowHeaderToolTip](../../aspose.cells.gridweb.data/gridworksheet/setrowheadertooltip)(int, string) | 设置行标题的工具提示文本。 |
| [SetRowReadonly](../../aspose.cells.gridweb.data/gridworksheet/setrowreadonly)(int, bool) | 将一行设置为只读，因此用户不能从客户端删除它。 这是GridWeb专门的扩展方法，在实际的excel文件中不会保留和生效 |
| [UnFreezePanes](../../aspose.cells.gridweb.data/gridworksheet/unfreezepanes)() | 解冻工作表中的窗格。 |
| [UnGroupRows](../../aspose.cells.gridweb.data/gridworksheet/ungrouprows)(int, int) | 取消组合行。 |
| [UnProtect](../../aspose.cells.gridweb.data/gridworksheet/unprotect)() | 取消保护工作表。 |

### 也可以看看

* 命名空间 [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* 部件 [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
