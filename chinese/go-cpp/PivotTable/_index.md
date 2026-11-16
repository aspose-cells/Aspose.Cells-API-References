---
title: "PivotTable 类"
linktitle: "PivotTable"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PivotTable 类。封装在 Go 中表示 pivottable 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pivottable/
---

## PivotTable class

PivotTable 的摘要描述。

```go

type PivotTable struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [Dispose](./dispose/) | 执行应用程序定义的任务，涉及释放、释放或重置非托管资源。 |
| [GetPivotCache](./getpivotcache/) | 获取数据源。 |
| [IsExcel2003Compatible](./isexcel2003compatible/) | 指定在刷新 PivotTable 时，PivotTable 是否兼容 Excel2003；如果为 true，则字符串必须小于或等于 255 个字符，如果字符串超过 255 个字符，将被截断；如果为 false，则字符串不受上述限制。默认值为 true。 |
| [SetIsExcel2003Compatible](./setisexcel2003compatible/) | 指定在刷新 PivotTable 时，PivotTable 是否兼容 Excel2003；如果为 true，则字符串必须小于或等于 255 个字符，如果字符串超过 255 个字符，将被截断；如果为 false，则字符串不受上述限制。默认值为 true。 |
| [GetRefreshedByWho](./getrefreshedbywho/) | 获取刷新此 PivotTable 的最后用户的名称 |
| [GetRefreshDate](./getrefreshdate/) | 获取 PivotTable 最近一次刷新的日期时间。 |
| [GetPivotTableStyle](./getpivottablestyle/) | 获取此透视表的 TableStyle 设置。 |
| [SetPivotTableStyle](./setpivottablestyle/) | 获取此透视表的 TableStyle 设置。 |
| [GetPivotTableStyleName](./getpivottablestylename/) | 获取或设置透视表的样式名称。 |
| [SetPivotTableStyleName](./setpivottablestylename/) | 获取或设置透视表的样式名称。 |
| [GetPivotTableStyleType](./getpivottablestyletype/) | 获取并设置内置的透视表样式。 |
| [SetPivotTableStyleType](./setpivottablestyletype/) | 获取并设置内置的透视表样式。 |
| [CopyStyle](./copystyle/) | 从另一个透视表复制命名样式。 |
| [ShowReportFilterPage](./showreportfilterpage/) | 根据 PivotField 显示所有报告筛选页面，PivotField 必须位于 PageFields 中。 |
| [ShowReportFilterPageByName](./showreportfilterpagebyname/) | 根据 PivotField 的名称显示所有报告筛选页面，PivotField 必须位于 PageFields 中。 |
| [ShowReportFilterPageByIndex](./showreportfilterpagebyindex/) | 根据 PageFields 中的位置索引显示所有报告筛选页面。 |
| [RemoveField_PivotFieldType_String](./removefield_pivotfieldtype_string/) | 从特定字段区域移除字段。 |
| [RemoveField_PivotFieldType_Int](./removefield_pivotfieldtype_int/) | 从特定透视区域移除字段。 |
| [RemoveField_PivotFieldType_PivotField](./removefield_pivotfieldtype_pivotfield/) | 从特定字段区域移除字段。 |
| [AddFieldToArea_PivotFieldType_String](./addfieldtoarea_pivotfieldtype_string/) | 将字段添加到特定区域。 |
| [AddFieldToArea_PivotFieldType_Int](./addfieldtoarea_pivotfieldtype_int/) | 将字段添加到特定区域。 |
| [AddFieldToArea_PivotFieldType_PivotField](./addfieldtoarea_pivotfieldtype_pivotfield/) | 将字段添加到特定区域。 |
| [AddCalculatedField_String_String_Bool](./addcalculatedfield_string_string_bool/) | 向透视字段添加计算字段。 |
| [AddCalculatedField_String_String](./addcalculatedfield_string_string/) | 向透视字段添加计算字段并将其拖动到数据区域。 |
| [GetFields](./getfields/) | 根据区域获取特定的透视字段列表。 |
| [GetColumnFields](./getcolumnfields/) | 返回当前显示为列字段的 PivotFields 对象。 |
| [GetRowFields](./getrowfields/) | 返回当前显示为行字段的 PivotFields 对象。 |
| [GetPageFields](./getpagefields/) | 返回当前显示为页面字段的 PivotFields 对象。 |
| [GetDataFields](./getdatafields/) | 获取一个表示 PivotTable 中所有数据字段的 PivotField 对象。只读。当 DataPiovtFiels 中有两个或以上数据字段时才会初始化。仅用于将 DataPivotField 添加到 PivotTable 的行/列区域。默认位于行区域。 |
| [GetValuesField](./getvaluesfield/) | 获取一个表示 PivotTable 中所有数据字段的 PivotField 对象。只读。当 Data 区域中有两个或以上数据字段时才会创建。默认位于行区域。您可以使用 PivotTable.AddFieldToArea() 方法将其拖动到行/列区域。 |
| [GetBaseFields](./getbasefields/) | 返回 PivotTable 中的所有基础透视字段。 |
| [GetPivotFilters](./getpivotfilters/) | 返回透视表中透视字段的所有筛选器。 |
| [GetButtonArea](./getbuttonarea/) | 获取包含字段按钮的区域。 |
| [GetTopRightArea](./gettoprightarea/) | 表示 PivotTable 右上角的空白区域（在 RTL 工作表中为左上角）。 |
| [GetFilterArea](./getfilterarea/) | 获取筛选区域的范围。 |
| [GetColumnRange](./getcolumnrange/) | 返回一个 CellArea 对象，表示包含 PivotTable 报表中列区域的范围。只读。 |
| [GetRowRange](./getrowrange/) | 返回一个 CellArea 对象，表示包含 PivotTable 报表中行区域的范围。只读。 |
| [GetDataBodyRange](./getdatabodyrange/) | 返回一个 CellArea 对象，表示列表中位于标题行和插入行之间的数据区域的范围。只读。 |
| [GetTableRange1](./gettablerange1/) | 返回一个 CellArea 对象，表示包含整个 PivotTable 报表的范围，但不包括页面字段。只读。 |
| [GetTableRange2](./gettablerange2/) | 返回一个 CellArea 对象，表示包含整个 PivotTable 报表的范围，包括页面字段。只读。 |
| [MoveTo_Int_Int](./moveto_int_int/) | 将 PivotTable 移动到工作表中的其他位置。 |
| [MoveTo_Int_Int_Int](./moveto_int_int_int/) | 将 PivotTable 移动到工作表中的其他位置。 |
| [MoveTo_String](./moveto_string/) | 将 PivotTable 移动到工作表中的其他位置。 |
| [IsGridDropZones](./isgriddropzones/) | 指示 PivotTable 报表是否显示经典透视表布局。（在网格中启用字段拖动） |
| [SetIsGridDropZones](./setisgriddropzones/) | 指示 PivotTable 报表是否显示经典透视表布局。（在网格中启用字段拖动） |
| [GetShowColumnGrandTotals](./getshowcolumngrandtotals/) | 指示是否显示此透视表列的总计。 |
| [SetShowColumnGrandTotals](./setshowcolumngrandtotals/) | 指示是否显示此透视表列的总计。 |
| [GetShowRowGrandTotals](./getshowrowgrandtotals/) | 指示是否显示此透视表行的总计。 |
| [SetShowRowGrandTotals](./setshowrowgrandtotals/) | 指示是否显示此透视表行的总计。 |
| [GetDisplayNullString](./getdisplaynullstring/) | 指示 PivotTable 报表在值为 null 时是否显示自定义字符串。 |
| [SetDisplayNullString](./setdisplaynullstring/) | 指示 PivotTable 报表在值为 null 时是否显示自定义字符串。 |
| [GetNullString](./getnullstring/) | 获取在包含 null 值的单元格中显示的字符串（当 DisplayNullString 属性为 true 时）。默认值为空字符串。 |
| [SetNullString](./setnullstring/) | 获取在包含 null 值的单元格中显示的字符串（当 DisplayNullString 属性为 true 时）。默认值为空字符串。 |
| [GetDisplayErrorString](./getdisplayerrorstring/) | 指示 PivotTable 报表在包含错误的单元格中是否显示自定义字符串。 |
| [SetDisplayErrorString](./setdisplayerrorstring/) | 指示 PivotTable 报表在包含错误的单元格中是否显示自定义字符串。 |
| [GetDataFieldHeaderName](./getdatafieldheadername/) | 获取和设置 PivotTable 中值区域字段标题的名称。 |
| [SetDataFieldHeaderName](./setdatafieldheadername/) | 获取和设置 PivotTable 中值区域字段标题的名称。 |
| [GetErrorString](./geterrorstring/) | 获取在包含错误的单元格中显示的字符串（当 DisplayErrorString 属性为 true 时）。默认值为空字符串。 |
| [SetErrorString](./seterrorstring/) | 获取在包含错误的单元格中显示的字符串（当 DisplayErrorString 属性为 true 时）。默认值为空字符串。 |
| [IsAutoFormat](./isautoformat/) | 指示 PivotTable 报表是否自动格式化。复选框 "autoformat table"，位于 Excel 2003 的透视表选项中。 |
| [SetIsAutoFormat](./setisautoformat/) | 指示 PivotTable 报表是否自动格式化。复选框 "autoformat table"，位于 Excel 2003 的透视表选项中。 |
| [GetAutofitColumnWidthOnUpdate](./getautofitcolumnwidthonupdate/) | 指示在更新时是否自动调整列宽。 |
| [SetAutofitColumnWidthOnUpdate](./setautofitcolumnwidthonupdate/) | 指示在更新时是否自动调整列宽。 |
| [GetAutoFormatType](./getautoformattype/) | 获取和设置 PivotTable 的自动格式类型。 |
| [SetAutoFormatType](./setautoformattype/) | 获取和设置 PivotTable 的自动格式类型。 |
| [GetMergeLabels](./getmergelabels/) | 指示跨越多个单元格的行或列标题是否应合并为单个单元格。 |
| [SetMergeLabels](./setmergelabels/) | 指示跨越多个单元格的行或列标题是否应合并为单个单元格。 |
| [GetPreserveCellFormattingOnUpdate](./getpreservecellformattingonupdate/) | 指示在刷新或重新计算透视表时是否保留单元格格式（PivotTableFormat）。 |
| [SetPreserveCellFormattingOnUpdate](./setpreservecellformattingonupdate/) | 指示在刷新或重新计算透视表时是否保留单元格格式（PivotTableFormat）。 |
| [GetShowDrill](./getshowdrill/) | 获取和设置是否显示展开/折叠按钮。 |
| [SetShowDrill](./setshowdrill/) | 获取和设置是否显示展开/折叠按钮。 |
| [GetEnableDrilldown](./getenabledrilldown/) | 指示是否启用下钻功能。 |
| [SetEnableDrilldown](./setenabledrilldown/) | 指示是否启用下钻功能。 |
| [GetEnableFieldDialog](./getenablefielddialog/) | 指示当用户双击 PivotTable 字段时，PivotTable 字段对话框是否可用。 |
| [SetEnableFieldDialog](./setenablefielddialog/) | 指示当用户双击 PivotTable 字段时，PivotTable 字段对话框是否可用。 |
| [GetEnableFieldList](./getenablefieldlist/) | 指示在 Excel 视图中是否可用 PivotTable 的字段列表。 |
| [SetEnableFieldList](./setenablefieldlist/) | 指示在 Excel 视图中是否可用 PivotTable 的字段列表。 |
| [GetEnableWizard](./getenablewizard/) | 指示是否可用 PivotTable 向导。 |
| [SetEnableWizard](./setenablewizard/) | 指示是否可用 PivotTable 向导。 |
| [GetSubtotalHiddenPageItems](./getsubtotalhiddenpageitems/) | 指示 PivotTable 报表中隐藏的页面字段项是否包含在行和列小计、块总计以及总计中。默认值为 False。 |
| [SetSubtotalHiddenPageItems](./setsubtotalhiddenpageitems/) | 指示 PivotTable 报表中隐藏的页面字段项是否包含在行和列小计、块总计以及总计中。默认值为 False。 |
| [GetGrandTotalName](./getgrandtotalname/) | 返回在总计列或行标题中显示的标签。默认值是字符串 "Grand Total"。 |
| [SetGrandTotalName](./setgrandtotalname/) | 返回在总计列或行标题中显示的标签。默认值是字符串 "Grand Total"。 |
| [GetManualUpdate](./getmanualupdate/) | 指示是否仅在用户请求时重新计算 PivotTable 报表。 |
| [SetManualUpdate](./setmanualupdate/) | 指示是否仅在用户请求时重新计算 PivotTable 报表。 |
| [GetAllowMultipleFiltersPerField](./getallowmultiplefiltersperfield/) | 指定一个布尔值，指示 PivotTable 的字段是否可以设置多个筛选器。 |
| [SetAllowMultipleFiltersPerField](./setallowmultiplefiltersperfield/) | 指定一个布尔值，指示 PivotTable 的字段是否可以设置多个筛选器。 |
| [GetEnableDataValueEditing](./getenabledatavalueediting/) | 指定一个布尔值，指示是否允许用户编辑 PivotTable 数据区域中的单元格。启用值区域的单元格编辑 |
| [SetEnableDataValueEditing](./setenabledatavalueediting/) | 指定一个布尔值，指示是否允许用户编辑 PivotTable 数据区域中的单元格。启用值区域的单元格编辑 |
| [GetShowDataTips](./getshowdatatips/) | 指示是否应为 PivotTable 数据单元格显示工具提示。 |
| [SetShowDataTips](./setshowdatatips/) | 指示是否应为 PivotTable 数据单元格显示工具提示。 |
| [GetShowMemberPropertyTips](./getshowmemberpropertytips/) | 指定一个布尔值，指示是否应从 PivotTable 工具提示中省略成员属性信息。 |
| [SetShowMemberPropertyTips](./setshowmemberpropertytips/) | 指定一个布尔值，指示是否应从 PivotTable 工具提示中省略成员属性信息。 |
| [GetShowValuesRow](./getshowvaluesrow/) | 指示是否显示值行。 |
| [SetShowValuesRow](./setshowvaluesrow/) | 指示是否显示值行。 |
| [GetShowEmptyCol](./getshowemptycol/) | 指示是否在表中包含空列 |
| [SetShowEmptyCol](./setshowemptycol/) | 指示是否在表中包含空列 |
| [GetShowEmptyRow](./getshowemptyrow/) | 指示是否在表中包含空行。 |
| [SetShowEmptyRow](./setshowemptyrow/) | 指示是否在表中包含空行。 |
| [GetFieldListSortAscending](./getfieldlistsortascending/) | 指示 PivotTable 中的字段是否在字段列表中以非默认顺序排序。 |
| [SetFieldListSortAscending](./setfieldlistsortascending/) | 指示 PivotTable 中的字段是否在字段列表中以非默认顺序排序。 |
| [GetPrintDrill](./getprintdrill/) | 指定一个布尔值，指示是否应打印钻取指示器。打印在 PivotTable 上显示的展开/折叠按钮。 |
| [SetPrintDrill](./setprintdrill/) | 指定一个布尔值，指示是否应打印钻取指示器。打印在 PivotTable 上显示的展开/折叠按钮。 |
| [GetAltTextTitle](./getalttexttitle/) | 获取并设置替代文本的标题。 |
| [SetAltTextTitle](./setalttexttitle/) | 获取并设置替代文本的标题。 |
| [GetAltTextDescription](./getalttextdescription/) | 获取替代文本的描述。 |
| [SetAltTextDescription](./setalttextdescription/) | 获取替代文本的描述。 |
| [GetName](./getname/) | 获取 PivotTable 的名称 |
| [SetName](./setname/) | 获取 PivotTable 的名称 |
| [GetColumnHeaderCaption](./getcolumnheadercaption/) | 获取并设置 PivotTable 列标题的自定义标题。 |
| [SetColumnHeaderCaption](./setcolumnheadercaption/) | 获取并设置 PivotTable 列标题的自定义标题。 |
| [GetIndent](./getindent/) | 指定紧凑轴的缩进增量，可用于将报表布局设置为紧凑形式。 |
| [SetIndent](./setindent/) | 指定紧凑轴的缩进增量，可用于将报表布局设置为紧凑形式。 |
| [GetRowHeaderCaption](./getrowheadercaption/) | 获取并设置此 PivotTable 行标题的自定义标题。 |
| [SetRowHeaderCaption](./setrowheadercaption/) | 获取并设置此 PivotTable 行标题的自定义标题。 |
| [GetShowHeaders](./getshowheaders/) | 是否在 PivotTable 视图的行轴和列轴上显示数据字段标题和透视字段标题。 |
| [SetShowHeaders](./setshowheaders/) | 是否在 PivotTable 视图的行轴和列轴上显示数据字段标题和透视字段标题。 |
| [GetCustomListSort](./getcustomlistsort/) | 指示在排序数据时是否考虑内置的自定义列表。 |
| [SetCustomListSort](./setcustomlistsort/) | 指示在排序数据时是否考虑内置的自定义列表。 |
| [GetConditionalFormats](./getconditionalformats/) | 获取透视表的条件格式。 |
| [GetPageFieldOrder](./getpagefieldorder/) | 获取并设置页面字段添加到 PivotTable 报表布局中的顺序。 |
| [SetPageFieldOrder](./setpagefieldorder/) | 获取并设置页面字段添加到 PivotTable 报表布局中的顺序。 |
| [GetPageFieldWrapCount](./getpagefieldwrapcount/) | 获取 PivotTable 报表中每列或每行的页面字段数量。 |
| [SetPageFieldWrapCount](./setpagefieldwrapcount/) | 获取 PivotTable 报表中每列或每行的页面字段数量。 |
| [GetTag](./gettag/) | 获取并设置与此 PivotTable 视图关联的用户定义字符串。 |
| [SetTag](./settag/) | 获取并设置与此 PivotTable 视图关联的用户定义字符串。 |
| [GetSaveData](./getsavedata/) | 指示 PivotTable 报表的数据是否随工作簿一起保存。 |
| [SetSaveData](./setsavedata/) | 指示 PivotTable 报表的数据是否随工作簿一起保存。 |
| [GetRefreshDataOnOpeningFile](./getrefreshdataonopeningfile/) | 指示在打开文件时是否刷新数据。 |
| [SetRefreshDataOnOpeningFile](./setrefreshdataonopeningfile/) | 指示在打开文件时是否刷新数据。 |
| [GetSourceType](./getsourcetype/) | 获取数据透视表的数据源类型。 |
| [GetSourceDataConnections](./getsourcedataconnections/) | 获取外部连接的数据源。 |
| [GetNamesOfSourceDataConnections](./getnamesofsourcedataconnections/) | 获取外部源数据连接的名称。 |
| [GetDataSource](./getdatasource/) | 获取并设置数据透视表的数据源。 |
| [SetDataSource](./setdatasource/) | 获取并设置数据透视表的数据源。 |
| [ChangeDataSource](./changedatasource/) | 更改数据透视表的数据源。 |
| [GetSource](./getsource/) | 获取此数据透视表的数据源。 |
| [GetSource_Bool](./getsource_bool/) | 获取此数据透视表的数据源。 |
| [Refresh](./refresh/) | 从数据源刷新 PivotCache 并计算数据和样式以用于数据透视视图。 |
| [CalculateData](./calculatedata/) | 将数据透视表的数据计算到单元格中。 |
| [CalculateData_PivotTableCalculateOption](./calculatedata_pivottablecalculateoption/) | 使用选项计算数据透视表。 |
| [GetPivotTablesWithSamePivotCache](./getpivottableswithsamepivotcache/) | 获取所有使用相同 PivotCache 的数据透视表。 |
| [ClearData](./cleardata/) | 清除数据透视表视图的数据和格式。 |
| [ClearFilters](./clearfilters/) | 清除此数据透视表的所有筛选器。 |
| [ClearAll](./clearall/) | 从区域中移除所有字段。 |
| [CalculateRange](./calculaterange/) | 计算数据透视表的范围。 |
| [FormatAll](./formatall/) | 格式化数据透视表区域中的所有单元格 |
| [FormatRow](./formatrow/) | 格式化数据透视表区域中的行数据 |
| [Format_PivotArea_Style](./format_pivotarea_style/) | 格式化数据透视表的选定区域。 |
| [Format_CellArea_Style](./format_cellarea_style/) | 格式化数据透视表的选定区域。 |
| [Format_Int_Int_Style](./format_int_int_style/) | 格式化数据透视表区域中的单元格 |
| [SelectArea](./selectarea/) | 选择数据透视表视图的一个区域。 |
| [ShowDetail](./showdetail/) | 在新表中显示数据区域中某个项目的详细信息。 |
| [GetPivotFormats](./getpivotformats/) | 获取应用于数据透视表的所有格式。 |
| [GetRepeatItemsOnEachPrintedPage](./getrepeatitemsoneachprintedpage/) | 指示在表格形式的透视字段中，行区域的透视项标题是否在每页打印时重复。 |
| [SetRepeatItemsOnEachPrintedPage](./setrepeatitemsoneachprintedpage/) | 指示在表格形式的透视字段中，行区域的透视项标题是否在每页打印时重复。 |
| [GetPrintTitles](./getprinttitles/) | 指示工作表的打印标题是否基于数据透视表报告设置。默认值为 false。 |
| [SetPrintTitles](./setprinttitles/) | 指示工作表的打印标题是否基于数据透视表报告设置。默认值为 false。 |
| [GetDisplayImmediateItems](./getdisplayimmediateitems/) | 指示当数据透视表的数据区域为空时，行和列区域的项目是否可见。默认值为 true。 |
| [SetDisplayImmediateItems](./setdisplayimmediateitems/) | 指示当数据透视表的数据区域为空时，行和列区域的项目是否可见。默认值为 true。 |
| [IsSelected](./isselected/) | 指示此数据透视表是否已被选中。 |
| [SetIsSelected](./setisselected/) | 指示此数据透视表是否已被选中。 |
| [GetShowPivotStyleRowHeader](./getshowpivotstylerowheader/) | 指示透视表中的行标题是否应应用样式。 |
| [SetShowPivotStyleRowHeader](./setshowpivotstylerowheader/) | 指示透视表中的行标题是否应应用样式。 |
| [GetShowPivotStyleColumnHeader](./getshowpivotstylecolumnheader/) | 指示透视表中的列标题是否应应用样式。 |
| [SetShowPivotStyleColumnHeader](./setshowpivotstylecolumnheader/) | 指示透视表中的列标题是否应应用样式。 |
| [GetShowPivotStyleRowStripes](./getshowpivotstylerowstripes/) | 指示是否已应用行条纹格式化。 |
| [SetShowPivotStyleRowStripes](./setshowpivotstylerowstripes/) | 指示是否已应用行条纹格式化。 |
| [GetShowPivotStyleColumnStripes](./getshowpivotstylecolumnstripes/) | 指示是否已对列应用条纹格式化。 |
| [SetShowPivotStyleColumnStripes](./setshowpivotstylecolumnstripes/) | 指示是否已对列应用条纹格式化。 |
| [GetShowPivotStyleLastColumn](./getshowpivotstylelastcolumn/) | 指示是否已应用列格式化。 |
| [SetShowPivotStyleLastColumn](./setshowpivotstylelastcolumn/) | 指示是否已应用列格式化。 |
| [GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | 获取此透视表的水平分页符。 |
| [ShowInCompactForm](./showincompactform/) | 以紧凑形式布局透视表视图。 |
| [ShowInOutlineForm](./showinoutlineform/) | 以大纲形式布局透视表。 |
| [ShowInTabularForm](./showintabularform/) | 以表格形式布局透视表。 |
| [GetCellByDisplayName](./getcellbydisplayname/) | 通过 PivotField 的显示名称获取 Cell 对象。 |
| [GetDependentPivotTables](./getdependentpivottables/) | 获取所有使用此透视表作为数据源的透视表。 |
| [ExportViewToJson](./exportviewtojson/) | 将透视视图导出为 JSON。 |
