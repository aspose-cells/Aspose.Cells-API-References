---
title: PivotTable
second_title: Aspose.Cells for .NET API 参考
description: 数据透视表的摘要描述
type: docs
weight: 4690
url: /zh/net/aspose.cells.pivot/pivottable/
---
## PivotTable class

数据透视表的摘要描述。

```csharp
public class PivotTable : IDisposable
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [AltTextDescription](../../aspose.cells.pivot/pivottable/alttextdescription) { get; set; } | 获取替代文本的描述 |
| [AltTextTitle](../../aspose.cells.pivot/pivottable/alttexttitle) { get; set; } | 获取替代文本的标题 |
| [AutoFormatType](../../aspose.cells.pivot/pivottable/autoformattype) { get; set; } | 获取数据透视表自动格式类型。 |
| [BaseFields](../../aspose.cells.pivot/pivottable/basefields) { get; } | 返回一个 PivotFields 对象，该对象包括数据透视表报告中的所有字段 |
| [ColumnFields](../../aspose.cells.pivot/pivottable/columnfields) { get; } | 返回当前显示为列字段的 PivotFields 对象。 |
| [ColumnGrand](../../aspose.cells.pivot/pivottable/columngrand) { get; set; } | 指示数据透视表是否显示列的总计。 |
| [ColumnHeaderCaption](../../aspose.cells.pivot/pivottable/columnheadercaption) { get; set; } | 获取数据透视表的列标题标题。 |
| [ColumnRange](../../aspose.cells.pivot/pivottable/columnrange) { get; } | 返回代表范围 的 CellArea 对象，该范围包含数据透视表中的列区域。只读。 |
| [CustomListSort](../../aspose.cells.pivot/pivottable/customlistsort) { get; set; } | 表示排序数据时是否考虑内置自定义列表 |
| [DataBodyRange](../../aspose.cells.pivot/pivottable/databodyrange) { get; } | 返回一个 CellArea 对象，该对象表示在标题行和插入行之间的列表中包含数据区域 的范围。只读。 |
| [DataField](../../aspose.cells.pivot/pivottable/datafield) { get; } | 获取一个 PivotField 对象，该对象表示数据透视表中的所有数据字段。 只读。只有当 DataPiovtFiels 中有两个或多个数据字段时才会初始化。 它仅用于将 DataPivotField 添加到数据透视表的行/列区域。默认在行区域。 |
| [DataFields](../../aspose.cells.pivot/pivottable/datafields) { get; } | 获取一个 PivotField 对象，该对象表示数据透视表中的所有数据字段。 只读。只有当 DataPiovtFiels 中有两个或多个数据字段时才会初始化。 它仅用于将 DataPivotField 添加到数据透视表的行/列区域。默认在行区域。 |
| [DataSource](../../aspose.cells.pivot/pivottable/datasource) { get; set; } | 获取和设置数据透视表的数据源。 |
| [DisplayErrorString](../../aspose.cells.pivot/pivottable/displayerrorstring) { get; set; } | 指示数据透视表是否在包含错误的单元格中显示自定义字符串。 |
| [DisplayImmediateItems](../../aspose.cells.pivot/pivottable/displayimmediateitems) { get; set; } | 表示当数据透视表的数据区域为空时，行和列区域中的项目是否可见 。默认值是true。 |
| [DisplayNullString](../../aspose.cells.pivot/pivottable/displaynullstring) { get; set; } | 指示数据透视表是否在包含空值的单元格中显示自定义字符串 。 |
| [EnableDataValueEditing](../../aspose.cells.pivot/pivottable/enabledatavalueediting) { get; set; } | 指定一个布尔值，指示是否允许用户编辑数据透视表数据区域中的单元格。 在值区域启用单元格编辑 |
| [EnableDrilldown](../../aspose.cells.pivot/pivottable/enabledrilldown) { get; set; } | 获取是否启用向下钻取。 |
| [EnableFieldDialog](../../aspose.cells.pivot/pivottable/enablefielddialog) { get; set; } | 指示当用户双击数据透视表字段时，数据透视表字段对话框是否可用 。 |
| [EnableFieldList](../../aspose.cells.pivot/pivottable/enablefieldlist) { get; set; } | 获取是否启用数据透视表的字段列表。 |
| [EnableWizard](../../aspose.cells.pivot/pivottable/enablewizard) { get; set; } | 指示数据透视表向导是否可用。 |
| [ErrorString](../../aspose.cells.pivot/pivottable/errorstring) { get; set; } | 当 DisplayErrorString 属性为 true 时，获取包含错误 的单元格中显示的字符串。默认值为空字符串。 |
| [ExternalConnectionDataSource](../../aspose.cells.pivot/pivottable/externalconnectiondatasource) { get; } | 获取外部连接数据源。 |
| [FieldListSortAscending](../../aspose.cells.pivot/pivottable/fieldlistsortascending) { get; set; } | 指定一个布尔值，指示数据透视表中的字段是否按字段列表中的非默认顺序排序。 |
| [GrandTotalName](../../aspose.cells.pivot/pivottable/grandtotalname) { get; set; } | 返回显示在总计列或行标题中的文本字符串标签。 默认值为字符串“Grand Total”。 |
| [HasBlankRows](../../aspose.cells.pivot/pivottable/hasblankrows) { get; set; } | 表示是否添加空行。 该属性仅适用于需要添加空白行的数据透视表自动格式类型。 |
| [Indent](../../aspose.cells.pivot/pivottable/indent) { get; set; } | 指定紧凑轴的缩进增量，可用于将报表布局设置为紧凑形式。 |
| [IsAutoFormat](../../aspose.cells.pivot/pivottable/isautoformat) { get; set; } | 指示数据透视表是否自动格式化。 复选框“自动格式化表格”，位于 Excel 2003 的数据透视表选项中 复选框“更新时自动调整列宽”，位于数据透视表选项中:Excel 2007 的布局格式 |
| [IsExcel2003Compatible](../../aspose.cells.pivot/pivottable/isexcel2003compatible) { get; set; } | 指定刷新数据透视表时数据透视表是否兼容Excel2003， 如果为true，则字符串必须小于或等于255个字符，所以如果字符串大于 255 个字符， 将被截断。如果为 false，则字符串将没有上述限制。 默认值为真。 |
| [IsGridDropZones](../../aspose.cells.pivot/pivottable/isgriddropzones) { get; set; } | 指示数据透视表是否显示经典数据透视表布局。 （允许在网格中拖动字段） |
| [IsMultipleFieldFilters](../../aspose.cells.pivot/pivottable/ismultiplefieldfilters) { get; set; } | 指定一个布尔值，指示数据透视表的字段是否可以设置多个过滤器。 |
| [IsSelected](../../aspose.cells.pivot/pivottable/isselected) { get; set; } | 表示是否选择了数据透视表。 |
| [ItemPrintTitles](../../aspose.cells.pivot/pivottable/itemprinttitles) { get; set; } | 指定行轴 上的枢轴项目标题是否在每个打印页面上以表格形式重复枢轴字段。 |
| [ManualUpdate](../../aspose.cells.pivot/pivottable/manualupdate) { get; set; } | 指示是否仅应用户请求重新计算数据透视表。 |
| [MergeLabels](../../aspose.cells.pivot/pivottable/mergelabels) { get; set; } | 指示指定数据透视表的外行项、列项、小计、 和总计标签是否使用合并单元格。 |
| [MissingItemsLimit](../../aspose.cells.pivot/pivottable/missingitemslimit) { get; set; } | 指定一个布尔值，指示数据透视表的字段是否可以设置多个过滤器。 |
| [Name](../../aspose.cells.pivot/pivottable/name) { get; set; } | 获取数据透视表的名称 |
| [NullString](../../aspose.cells.pivot/pivottable/nullstring) { get; set; } | 当 DisplayNullString 属性为 true 时，获取在包含空值 的单元格中显示的字符串。默认值为空字符串。 |
| [PageFieldOrder](../../aspose.cells.pivot/pivottable/pagefieldorder) { get; set; } | 获取页面字段添加到数据透视表布局的顺序。 |
| [PageFields](../../aspose.cells.pivot/pivottable/pagefields) { get; } | 返回当前显示为页面字段的 PivotFields 对象。 |
| [PageFieldWrapCount](../../aspose.cells.pivot/pivottable/pagefieldwrapcount) { get; set; } | 获取数据透视表中每列或每行的页字段数。 |
| [PivotFilters](../../aspose.cells.pivot/pivottable/pivotfilters) { get; } | 返回一个 PivotFilterCollection 对象。 |
| [PivotFormatConditions](../../aspose.cells.pivot/pivottable/pivotformatconditions) { get; } | 获取数据透视表的格式条件。 |
| [PivotTableStyleName](../../aspose.cells.pivot/pivottable/pivottablestylename) { get; set; } | 获取和设置可透视的样式名称。 |
| [PivotTableStyleType](../../aspose.cells.pivot/pivottable/pivottablestyletype) { get; set; } | 获取和设置内置数据透视表样式。 |
| [PreserveFormatting](../../aspose.cells.pivot/pivottable/preserveformatting) { get; set; } | 表示刷新或重新计算数据透视表时是否保留格式。 |
| [PrintDrill](../../aspose.cells.pivot/pivottable/printdrill) { get; set; } | 指定一个布尔值，指示是否应打印钻孔指示符。 显示在数据透视表上时打印展开/折叠按钮。 |
| [PrintTitles](../../aspose.cells.pivot/pivottable/printtitles) { get; set; } | 指示是否根据数据透视表上的 设置工作表的打印标题。默认值为假。 |
| [RefreshDataFlag](../../aspose.cells.pivot/pivottable/refreshdataflag) { get; set; } | 表示是否刷新数据。 |
| [RefreshDataOnOpeningFile](../../aspose.cells.pivot/pivottable/refreshdataonopeningfile) { get; set; } | 表示打开文件时是否刷新数据。 |
| [RefreshDate](../../aspose.cells.pivot/pivottable/refreshdate) { get; } | 获取上次刷新数据透视表的日期。 |
| [RefreshedByWho](../../aspose.cells.pivot/pivottable/refreshedbywho) { get; } | 获取上次刷新数据透视表的用户名 |
| [RowFields](../../aspose.cells.pivot/pivottable/rowfields) { get; } | 返回当前显示为行字段的 PivotFields 对象。 |
| [RowGrand](../../aspose.cells.pivot/pivottable/rowgrand) { get; set; } | 指示数据透视表是否显示行的总计。 |
| [RowHeaderCaption](../../aspose.cells.pivot/pivottable/rowheadercaption) { get; set; } | 获取数据透视表的行标题标题。 |
| [RowRange](../../aspose.cells.pivot/pivottable/rowrange) { get; } | 返回代表范围 的 CellArea 对象，该范围包含数据透视表中的行区域。只读。 |
| [SaveData](../../aspose.cells.pivot/pivottable/savedata) { get; set; } | 指示数据透视表的数据是否与工作簿一起保存。 |
| [ShowDataTips](../../aspose.cells.pivot/pivottable/showdatatips) { get; set; } | 指定一个布尔值，指示是否应为数据透视表数据单元格显示工具提示。 |
| [ShowDrill](../../aspose.cells.pivot/pivottable/showdrill) { get; set; } | 获取是否显示展开/折叠按钮。 |
| [ShowEmptyCol](../../aspose.cells.pivot/pivottable/showemptycol) { get; set; } | 指定一个布尔值，指示是否在表中包含空列 |
| [ShowEmptyRow](../../aspose.cells.pivot/pivottable/showemptyrow) { get; set; } | 指定一个布尔值，指示是否在表中包含空行。 |
| [ShowMemberPropertyTips](../../aspose.cells.pivot/pivottable/showmemberpropertytips) { get; set; } | 指定一个布尔值，指示是否应从数据透视表工具提示中省略成员属性信息。 |
| [ShowPivotStyleColumnHeader](../../aspose.cells.pivot/pivottable/showpivotstylecolumnheader) { get; set; } | 指示数据透视表中的列标题是否应应用样式。 |
| [ShowPivotStyleColumnStripes](../../aspose.cells.pivot/pivottable/showpivotstylecolumnstripes) { get; set; } | 指示是否应用列带格式。 |
| [ShowPivotStyleLastColumn](../../aspose.cells.pivot/pivottable/showpivotstylelastcolumn) { get; set; } | 指示是否应用列带格式。 |
| [ShowPivotStyleRowHeader](../../aspose.cells.pivot/pivottable/showpivotstylerowheader) { get; set; } | 指示数据透视表中的行标题是否应应用样式。 |
| [ShowPivotStyleRowStripes](../../aspose.cells.pivot/pivottable/showpivotstylerowstripes) { get; set; } | 指示是否应用行条纹格式。 |
| [ShowRowHeaderCaption](../../aspose.cells.pivot/pivottable/showrowheadercaption) { get; set; } | 指示是否在数据透视表中显示行标题标题 指示是否显示字段标题和过滤器下拉列表 |
| [ShowValuesRow](../../aspose.cells.pivot/pivottable/showvaluesrow) { get; set; } | 指定一个布尔值，指示是否显示值行。 显示值行 |
| [SubtotalHiddenPageItems](../../aspose.cells.pivot/pivottable/subtotalhiddenpageitems) { get; set; } | 指示数据透视表中的隐藏页面字段项 是否包含在行和列小计、块总计和总计中。 默认值为 False。 |
| [TableRange1](../../aspose.cells.pivot/pivottable/tablerange1) { get; } | 返回一个 CellArea 对象，该对象表示包含整个数据透视表的范围， 但不包括页面字段。只读。 |
| [TableRange2](../../aspose.cells.pivot/pivottable/tablerange2) { get; } | 返回一个 CellArea 对象，该对象表示包含整个数据透视表的范围， 包括页面字段。只读。 |
| [Tag](../../aspose.cells.pivot/pivottable/tag) { get; set; } | 获取与数据透视表一起保存的字符串。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield)(string, string) | 将计算字段添加到数据透视字段并将其拖动到数据区域。 |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield_1)(string, string, bool) | 将计算字段添加到数据透视字段。 |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_1)(PivotFieldType, int) | 将字段添加到特定区域。 |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea)(PivotFieldType, PivotField) | 将字段添加到特定区域。 |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_2)(PivotFieldType, string) | 将字段添加到特定区域。 |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata)() | 将数据透视表的数据计算到单元格。 |
| [CalculateRange](../../aspose.cells.pivot/pivottable/calculaterange)() | 计算数据透视表的范围。 |
| [ChangeDataSource](../../aspose.cells.pivot/pivottable/changedatasource)(string[]) | 设置数据透视表的源数据。 Sheet1!$A$1:$C$3 |
| [ClearData](../../aspose.cells.pivot/pivottable/cleardata)() | 清除数据透视表的数据和格式 |
| [CopyStyle](../../aspose.cells.pivot/pivottable/copystyle)(PivotTable) | 从另一个数据透视表复制命名样式。 |
| [Dispose](../../aspose.cells.pivot/pivottable/dispose)() | 执行与释放、释放或 重置非托管资源相关的应用程序定义任务。 |
| [Fields](../../aspose.cells.pivot/pivottable/fields)(PivotFieldType) | 按字段类型获取具体字段。 |
| [Format](../../aspose.cells.pivot/pivottable/format)(int, int, Style) | 格式化可透视区域中的单元格 |
| [FormatAll](../../aspose.cells.pivot/pivottable/formatall)(Style) | 格式化可透视区域中的所有单元格 |
| [FormatRow](../../aspose.cells.pivot/pivottable/formatrow)(int, Style) | 格式化数据透视区中的行数据 |
| [GetCellByDisplayName](../../aspose.cells.pivot/pivottable/getcellbydisplayname)(string) | 通过 PivotField |
| [GetChildren](../../aspose.cells.pivot/pivottable/getchildren)() | 获取使用此数据透视表数据作为数据源的子数据透视表。 |
| [GetHorizontalBreaks](../../aspose.cells.pivot/pivottable/gethorizontalbreaks)() | 获取水平分页符的数据透视表行索引列表 |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource)() | 获取数据透视表的源数据。 |
| [Move](../../aspose.cells.pivot/pivottable/move#move_1)(string) | 将数据透视表移动到工作表中的不同位置。 |
| [Move](../../aspose.cells.pivot/pivottable/move#move)(int, int) | 将数据透视表移动到工作表中的不同位置。 |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata)() | 从数据源刷新数据透视表的数据和设置。 |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_1)(PivotFieldType, int) | 从特定字段区域删除字段 |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield)(PivotFieldType, PivotField) | 从特定字段区域中删除字段 |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_2)(PivotFieldType, string) | 从特定字段区域删除字段 |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield_1)(int) | 通过数据透视表设置自动字段组。 |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield)(PivotField) | 通过数据透视表设置自动字段组。 |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_3)(int, DateTime, DateTime, ArrayList, int) | 通过数据透视表设置手动字段组。 |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_2)(int, double, double, ArrayList, double) | 通过数据透视表设置手动字段组。 |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_1)(PivotField, DateTime, DateTime, ArrayList, int) | 通过数据透视表设置手动字段组。 |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield)(PivotField, double, double, ArrayList, double) | 通过数据透视表设置手动字段组。 |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup_1)(int) | 设置按数据透视表取消分组 |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup)(PivotField) | 设置按数据透视表取消分组 |
| [ShowInCompactForm](../../aspose.cells.pivot/pivottable/showincompactform)() | 以紧凑的形式布局数据透视表。 |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivottable/showinoutlineform)() | 以大纲形式布局数据透视表。 |
| [ShowInTabularForm](../../aspose.cells.pivot/pivottable/showintabularform)() | 以表格形式布局数据透视表。 |
| [ShowReportFilterPage](../../aspose.cells.pivot/pivottable/showreportfilterpage)(PivotField) | 根据 PivotField 显示所有报表过滤页面，PivotField 必须位于 PageFields 中。 |
| [ShowReportFilterPageByIndex](../../aspose.cells.pivot/pivottable/showreportfilterpagebyindex)(int) | 根据PageFields中的位置索引显示所有报表过滤页面 |
| [ShowReportFilterPageByName](../../aspose.cells.pivot/pivottable/showreportfilterpagebyname)(string) | 根据 PivotField 的名称显示所有报表过滤页面，PivotField 必须位于 PageFields 中。 |

### 例子

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

 //改变PivotField的属性
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

 //添加PivotFilter
int index = pivot.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivot.PivotFilters[index];
filter.AutoFilter.FilterTop10(0, false, false, 2);

 //添加PivotFormatCondition
int formatIndex = pivot.PivotFormatConditions.Add();
PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
FormatConditionCollection fcc = pfc.FormatConditions;
fcc.AddArea(pivot.DataBodyRange);
int idx = fcc.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = fcc[idx];
fc.Formula1 = "100";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundColor = Color.Red;

pivot.RefreshData();
pivot.CalculateData();

 //做你的事

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'改变PivotField的属性
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

'添加PivotFilter
Dim filterIndex As Int32 = pivot.PivotFilters.Add(0, PivotFilterType.Count)
Dim filter As PivotFilter = pivot.PivotFilters(filterIndex)
filter.AutoFilter.FilterTop10(0, False, False, 2)

'添加PivotFormatCondition
Dim formatIndex As Int32 = pivot.PivotFormatConditions.Add()
Dim pfc As PivotFormatCondition = pivot.PivotFormatConditions(formatIndex)
Dim fcc As FormatConditionCollection = pfc.FormatConditions
fcc.AddArea(pivot.DataBodyRange)
Dim idx As Int32 = fcc.AddCondition(FormatConditionType.CellValue)
Dim fc As FormatCondition = fcc(idx)
fc.Formula1 = "100"
fc.Operator = OperatorType.GreaterOrEqual
fc.Style.BackgroundColor = Color.Red

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### 也可以看看

* 命名空间 [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
