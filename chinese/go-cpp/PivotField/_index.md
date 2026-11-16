---
title: "PivotField 类"
linktitle: "PivotField"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PivotField 类。封装在 Go 中表示 pivotfield 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pivotfield/
---

## PivotField class

表示 PivotTable 报表中的字段。

```go

type PivotField struct  {
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
| [GetPivotItems](./getpivotitems/) | 获取透视字段的透视项 |
| [GetMaxValue](./getmaxvalue/) | 获取此字段的最大值。 |
| [GetMinValue](./getminvalue/) | 获取此字段的最大值。 |
| [GetGroupSettings](./getgroupsettings/) | 获取透视字段的分组设置。 |
| [InitPivotItems](./initpivotitems/) | 初始化透视字段的透视项 |
| [Group](./group/) | 自动对字段进行分组。 |
| [Group_PivotFieldGroupOptions](./group_pivotfieldgroupoptions/) | 使用选项对透视字段进行分组。 |
| [GroupBy](./groupby/) | 自定义分组字段。 |
| [Ungroup](./ungroup/) | 取消对透视字段的分组。 |
| [GetPivotFilterByType](./getpivotfilterbytype/) | 获取指定类型的透视字段的透视过滤器 |
| [GetFilters](./getfilters/) | 获取此透视字段已应用的所有透视过滤器。 |
| [ClearFilter](./clearfilter/) | 清除此透视字段的过滤设置。 |
| [FilterTop10](./filtertop10/) | 按数据透视字段的值进行过滤。 |
| [FilterByValue](./filterbyvalue/) | 按数据透视字段的值进行过滤。 |
| [FilterByLabel](./filterbylabel/) | 按行或列透视字段的标题进行过滤。 |
| [FilterByDate](./filterbydate/) | 按行或列透视字段的日期值进行过滤。 |
| [IsCalculatedField](./iscalculatedfield/) | 指示此透视字段是否为计算字段。 |
| [GetFormula](./getformula/) | 获取计算字段的公式。仅适用于计算字段。 |
| [IsValuesField](./isvaluesfield/) | 指示此字段是否表示数值字段。 |
| [GetBaseIndex](./getbaseindex/) | 表示源透视字段中的索引。 |
| [SetBaseIndex](./setbaseindex/) | 表示源透视字段中的索引。 |
| [GetPosition](./getposition/) | 表示该区域中 PivotField 的索引。 |
| [GetRegionType](./getregiontype/) | 指定此字段在透视表中显示的区域。 |
| [GetName](./getname/) | 表示 PivotField 的名称。 |
| [SetName](./setname/) | 表示 PivotField 的名称。 |
| [GetDisplayName](./getdisplayname/) | 表示透视表视图中透视字段的显示名称。 |
| [SetDisplayName](./setdisplayname/) | 表示透视表视图中透视字段的显示名称。 |
| [SetSubtotals_PivotFieldSubtotalType_Bool](./setsubtotals_pivotfieldsubtotaltype_bool/) | 设置指定字段的汇总方式。 |
| [GetSubtotals_PivotFieldSubtotalType](./getsubtotals_pivotfieldsubtotaltype/) | 指示是否为此透视字段显示指定的汇总。 |
| [GetSubtotals](./getsubtotals/) | 获取或设置该字段的汇总。仅适用于行或列透视字段。 |
| [SetSubtotals_PivotFieldSubtotalType](./setsubtotals_pivotfieldsubtotaltype/) | 获取或设置该字段的汇总。仅适用于行或列透视字段。 |
| [IsAutoSubtotals](./isautosubtotals/) | 指示指定字段是否显示自动汇总。默认值为 true。 |
| [SetIsAutoSubtotals](./setisautosubtotals/) | 指示指定字段是否显示自动汇总。默认值为 true。 |
| [GetAllowDraggingToRow](./getallowdraggingtorow/) | 指示指定字段是否可以拖动到行区域。默认值为 true。 |
| [SetAllowDraggingToRow](./setallowdraggingtorow/) | 指示指定字段是否可以拖动到行区域。默认值为 true。 |
| [GetAllowDraggingToColumn](./getallowdraggingtocolumn/) | 指示指定字段是否可以拖动到列区域。默认值为 true。 |
| [SetAllowDraggingToColumn](./setallowdraggingtocolumn/) | 指示指定字段是否可以拖动到列区域。默认值为 true。 |
| [GetAllowDraggingToPage](./getallowdraggingtopage/) | 指示指定字段是否可以拖动到页面区域。默认值为 true。 |
| [SetAllowDraggingToPage](./setallowdraggingtopage/) | 指示指定字段是否可以拖动到页面区域。默认值为 true。 |
| [GetAllowRemovingFromView](./getallowremovingfromview/) | 指示此透视字段是否可以从 PivotTable 视图中移除。默认值为 true。 |
| [SetAllowRemovingFromView](./setallowremovingfromview/) | 指示此透视字段是否可以从 PivotTable 视图中移除。默认值为 true。 |
| [GetAllowDraggingToData](./getallowdraggingtodata/) | 指示指定字段是否可以拖动到数值区域。默认值为 true。 |
| [SetAllowDraggingToData](./setallowdraggingtodata/) | 指示指定字段是否可以拖动到数值区域。默认值为 true。 |
| [IsMultipleItemSelectionAllowed](./ismultipleitemselectionallowed/) | 指示页面字段中是否可以选择多个项目。默认值为 false。 |
| [SetIsMultipleItemSelectionAllowed](./setismultipleitemselectionallowed/) | 指示页面字段中是否可以选择多个项目。默认值为 false。 |
| [IsRepeatItemLabels](./isrepeatitemlabels/) | 指示是否在该区域重复字段标签。默认值为 false。 |
| [SetIsRepeatItemLabels](./setisrepeatitemlabels/) | 指示是否在该区域重复字段标签。默认值为 false。 |
| [IsIncludeNewItemsInFilter](./isincludenewitemsinfilter/) | 指示在手动过滤中是否将新项目包含到字段中。默认值为 false。 |
| [SetIsIncludeNewItemsInFilter](./setisincludenewitemsinfilter/) | 指示在手动过滤中是否将新项目包含到字段中。默认值为 false。 |
| [IsInsertPageBreaksBetweenItems](./isinsertpagebreaksbetweenitems/) | 指示是否在每个项目后插入分页符。默认值为 false。 |
| [SetIsInsertPageBreaksBetweenItems](./setisinsertpagebreaksbetweenitems/) | 指示是否在每个项目后插入分页符。默认值为 false。 |
| [GetShowAllItems](./getshowallitems/) | 指示是否在 PivotTable 视图中显示所有项目，即使它们不包含汇总数据。默认值为 false。 |
| [SetShowAllItems](./setshowallitems/) | 指示是否在 PivotTable 视图中显示所有项目，即使它们不包含汇总数据。默认值为 false。 |
| [SortBy_SortOrder](./sortby_sortorder/) | 对该透视字段进行排序。 |
| [SortBy_SortOrder_Int_String](./sortby_sortorder_int_string/) | 对该透视字段进行排序。 |
| [GetSortSetting](./getsortsetting/) | 获取自动排序的所有设置 |
| [GetTop10AutoShowSettings](./gettop10autoshowsettings/) | 获取透视字段的前 10 项自动显示设置。 |
| [Top10AutoShow](./top10autoshow/) | 配置此透视字段的前 10 项自动显示设置。 |
| [GetFunction](./getfunction/) | 表示用于汇总此 PivotTable 数据字段的函数。 |
| [SetFunction](./setfunction/) | 表示用于汇总此 PivotTable 数据字段的函数。 |
| [ShowValuesAs](./showvaluesas/) | 当使用 ShowDataAs 计算时，以不同的显示格式显示数据字段的值。 |
| [GetShowValuesSetting](./getshowvaluessetting/) | 获取在使用 ShowDataAs 计算时显示值的设置。 |
| [GetCurrentPageItem](./getcurrentpageitem/) | 表示页面字段当前选定的页面项，用于过滤数据。仅对页面字段有效。 |
| [SetCurrentPageItem](./setcurrentpageitem/) | 表示页面字段当前选定的页面项，用于过滤数据。仅对页面字段有效。 |
| [GetInsertBlankRow](./getinsertblankrow/) | 指示是否在每个项目后插入空行。仅适用于行字段。 |
| [SetInsertBlankRow](./setinsertblankrow/) | 指示是否在每个项目后插入空行。仅适用于行字段。 |
| [GetShowSubtotalAtTop](./getshowsubtotalattop/) | 指示在 ShowInOutlineForm 为 true 时，是否在项目的顶部或底部显示小计，然后 |
| [SetShowSubtotalAtTop](./setshowsubtotalattop/) | 指示在 ShowInOutlineForm 为 true 时，是否在项目的顶部或底部显示小计，然后 |
| [GetShowInOutlineForm](./getshowinoutlineform/) | 指示是否在 Pivot Table 视图中以大纲形式布局此字段。 |
| [SetShowInOutlineForm](./setshowinoutlineform/) | 指示是否在 Pivot Table 视图中以大纲形式布局此字段。 |
| [GetNumber](./getnumber/) | 表示数字和日期的内置显示格式。 |
| [SetNumber](./setnumber/) | 表示数字和日期的内置显示格式。 |
| [Get_NumberFormat](./get_numberformat/) | 表示数字和日期的自定义显示格式。 |
| [SetNumberFormat](./setnumberformat/) | 表示数字和日期的自定义显示格式。 |
| [HideAllDetails](./hidealldetails/) | 隐藏所有细节 |
| [ShowAllDetails](./showalldetails/) | 显示所有细节 |
| [GetItems](./getitems/) | 获取此字段中透视项的所有标签。 |
| [GetOriginalItems](./getoriginalitems/) | 获取原始基础项； |
| [AddCalculatedItem](./addcalculateditem/) | 向透视字段添加计算公式项。 |
| [GetShowCompact](./getshowcompact/) | 指示是否在 Pivot Table 视图的同一列中显示下一个字段的标签 |
| [SetShowCompact](./setshowcompact/) | 指示是否在 Pivot Table 视图的同一列中显示下一个字段的标签 |
