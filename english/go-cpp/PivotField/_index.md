---
title: PivotField Class 
linktitle: PivotField
second_title: Aspose.Cells for Go via C++ API Reference
description: 'PivotField class. Encapsulates the object that represents pivotfield in Go.'
type: docs
weight: 200
url: /go-cpp/pivotfield/
---

## PivotField class

Represents a field in a PivotTable report.

```go

type PivotField struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetPivotItems](./getpivotitems/) | Gets the pivot items of the pivot field | 
|[GetMaxValue](./getmaxvalue/) | Gets the max value of this field. | 
|[GetMinValue](./getminvalue/) | Gets the max value of this field. | 
|[GetGroupSettings](./getgroupsettings/) | Gets the group settings of the pivot field. | 
|[InitPivotItems](./initpivotitems/) | Init the pivot items of the pivot field | 
|[Group](./group/) | Automatically group the field. | 
|[Group_PivotFieldGroupOptions](./group_pivotfieldgroupoptions/) | Groups the pivot field with options. | 
|[GroupBy](./groupby/) | Custom group the field. | 
|[Ungroup](./ungroup/) | Ungroup the pivot field. | 
|[GetPivotFilterByType](./getpivotfilterbytype/) | Gets the pivot filter of the pivot field by type | 
|[GetFilters](./getfilters/) | Gets all pivot filters applied for this pivot field. | 
|[ClearFilter](./clearfilter/) | Clears filter setting on this pivot field. | 
|[FilterTop10](./filtertop10/) | Filters by values of data pivot field. | 
|[FilterByValue](./filterbyvalue/) | Filters by values of data pivot field. | 
|[FilterByLabel](./filterbylabel/) | Filters by captions of row or column pivot field. | 
|[FilterByDate](./filterbydate/) | Filters by date values of row or column pivot field. | 
|[IsCalculatedField](./iscalculatedfield/) | Indicates whether the this pivot field is calculated field. | 
|[GetFormula](./getformula/) | Gets the formula of the calculated field .Only works for calculated field. | 
|[IsValuesField](./isvaluesfield/) | Indicates whether this field represents values field. | 
|[GetBaseIndex](./getbaseindex/) | Represents the index in the source pivot fields. | 
|[SetBaseIndex](./setbaseindex/) | Represents the index in the source pivot fields. | 
|[GetPosition](./getposition/) | Represents the index of PivotField in the region. | 
|[GetRegionType](./getregiontype/) | Specifies the region of the pivot table that this field is displayed. | 
|[GetName](./getname/) | Represents the name of PivotField. | 
|[SetName](./setname/) | Represents the name of PivotField. | 
|[GetDisplayName](./getdisplayname/) | Represents the display name of pivot field in the pivot table view. | 
|[SetDisplayName](./setdisplayname/) | Represents the display name of pivot field in the pivot table view. | 
|[SetSubtotals_PivotFieldSubtotalType_Bool](./setsubtotals_pivotfieldsubtotaltype_bool/) | Sets how to subtotal the specified field. | 
|[GetSubtotals_PivotFieldSubtotalType](./getsubtotals_pivotfieldsubtotaltype/) | Indicates whether to show specified subtotal for this pivot field. | 
|[GetSubtotals](./getsubtotals/) | Gets or sets the subtotals of the field. Only for Row or Column pivot field. | 
|[SetSubtotals_PivotFieldSubtotalType](./setsubtotals_pivotfieldsubtotaltype/) | Gets or sets the subtotals of the field. Only for Row or Column pivot field. | 
|[IsAutoSubtotals](./isautosubtotals/) | Indicates whether the specified field shows automatic subtotals. Default is true. | 
|[SetIsAutoSubtotals](./setisautosubtotals/) | Indicates whether the specified field shows automatic subtotals. Default is true. | 
|[GetAllowDraggingToRow](./getallowdraggingtorow/) | Indicates whether the specified field can be dragged to the row region.The default value is true. | 
|[SetAllowDraggingToRow](./setallowdraggingtorow/) | Indicates whether the specified field can be dragged to the row region.The default value is true. | 
|[GetAllowDraggingToColumn](./getallowdraggingtocolumn/) | Indicates whether the specified field can be dragged to the column region.The default value is true. | 
|[SetAllowDraggingToColumn](./setallowdraggingtocolumn/) | Indicates whether the specified field can be dragged to the column region.The default value is true. | 
|[GetAllowDraggingToPage](./getallowdraggingtopage/) | Indicates whether the specified field can be dragged to the page region.The default value is true. | 
|[SetAllowDraggingToPage](./setallowdraggingtopage/) | Indicates whether the specified field can be dragged to the page region.The default value is true. | 
|[GetAllowRemovingFromView](./getallowremovingfromview/) | Indicates whether this pivot field can be removed from the PivotTable view.The default value is true. | 
|[SetAllowRemovingFromView](./setallowremovingfromview/) | Indicates whether this pivot field can be removed from the PivotTable view.The default value is true. | 
|[GetAllowDraggingToData](./getallowdraggingtodata/) | Indicates whether the specified field can be dragged to the values region.The default value is true. | 
|[SetAllowDraggingToData](./setallowdraggingtodata/) | Indicates whether the specified field can be dragged to the values region.The default value is true. | 
|[IsMultipleItemSelectionAllowed](./ismultipleitemselectionallowed/) | Indicates whether multiple items could be selected in the page field.The default value is false. | 
|[SetIsMultipleItemSelectionAllowed](./setismultipleitemselectionallowed/) | Indicates whether multiple items could be selected in the page field.The default value is false. | 
|[IsRepeatItemLabels](./isrepeatitemlabels/) | Indicates whether to repeat labels of the field in the region.The default value is false. | 
|[SetIsRepeatItemLabels](./setisrepeatitemlabels/) | Indicates whether to repeat labels of the field in the region.The default value is false. | 
|[IsIncludeNewItemsInFilter](./isincludenewitemsinfilter/) | Indicates whether to include new items to the field in manual filter.The default value is false. | 
|[SetIsIncludeNewItemsInFilter](./setisincludenewitemsinfilter/) | Indicates whether to include new items to the field in manual filter.The default value is false. | 
|[IsInsertPageBreaksBetweenItems](./isinsertpagebreaksbetweenitems/) | Indicates whether to insert page breaks after each item.The default value is false. | 
|[SetIsInsertPageBreaksBetweenItems](./setisinsertpagebreaksbetweenitems/) | Indicates whether to insert page breaks after each item.The default value is false. | 
|[GetShowAllItems](./getshowallitems/) | Indicates whether to display all items in the PivotTable view,even if they don't contain summary data.The default value is false. | 
|[SetShowAllItems](./setshowallitems/) | Indicates whether to display all items in the PivotTable view,even if they don't contain summary data.The default value is false. | 
|[SortBy_SortOrder](./sortby_sortorder/) | Sorts this pivot field. | 
|[SortBy_SortOrder_Int_String](./sortby_sortorder_int_string/) | Sorts this pivot field. | 
|[GetSortSetting](./getsortsetting/) | Gets all settings of auto sorting | 
|[GetTop10AutoShowSettings](./gettop10autoshowsettings/) | Gets the Top 10 AutoShow settings for a pivot field. | 
|[Top10AutoShow](./top10autoshow/) | Configures Top10 AutoShow settings for this pivot field. | 
|[GetFunction](./getfunction/) | Represents the function used to summarize this PivotTable data field. | 
|[SetFunction](./setfunction/) | Represents the function used to summarize this PivotTable data field. | 
|[ShowValuesAs](./showvaluesas/) | Shows values of data field as different display format when the ShowDataAs calculation is in use. | 
|[GetShowValuesSetting](./getshowvaluessetting/) | Gets the settings of showing values as when the ShowDataAs calculation is in use. | 
|[GetCurrentPageItem](./getcurrentpageitem/) | Represents the current selected page item of the page field to filter data.Only valid for page fields. | 
|[SetCurrentPageItem](./setcurrentpageitem/) | Represents the current selected page item of the page field to filter data.Only valid for page fields. | 
|[GetInsertBlankRow](./getinsertblankrow/) | Indicates whether to insert a blank line after each item.Only for row fields. | 
|[SetInsertBlankRow](./setinsertblankrow/) | Indicates whether to insert a blank line after each item.Only for row fields. | 
|[GetShowSubtotalAtTop](./getshowsubtotalattop/) | Indicates whether to display subtotals at the top or bottom of items when ShowInOutlineForm is true, then | 
|[SetShowSubtotalAtTop](./setshowsubtotalattop/) | Indicates whether to display subtotals at the top or bottom of items when ShowInOutlineForm is true, then | 
|[GetShowInOutlineForm](./getshowinoutlineform/) | Indicates whether to layout this field in outline form on the Pivot Table view. | 
|[SetShowInOutlineForm](./setshowinoutlineform/) | Indicates whether to layout this field in outline form on the Pivot Table view. | 
|[GetNumber](./getnumber/) | Represents the built-in display format of numbers and dates. | 
|[SetNumber](./setnumber/) | Represents the built-in display format of numbers and dates. | 
|[Get_NumberFormat](./get_numberformat/) | Represents the custom display format of numbers and dates. | 
|[SetNumberFormat](./setnumberformat/) | Represents the custom display format of numbers and dates. | 
|[HideAllDetails](./hidealldetails/) | Hides all details | 
|[ShowAllDetails](./showalldetails/) | Show all details | 
|[GetItems](./getitems/) | Get all labels of pivot items in this field. | 
|[GetOriginalItems](./getoriginalitems/) | Get the original base items; | 
|[AddCalculatedItem](./addcalculateditem/) | Add a calculated formula item to the pivot field. | 
|[GetShowCompact](./getshowcompact/) | Indicates whether to display labels of the next field in the same column on the Pivot Table view | 
|[SetShowCompact](./setshowcompact/) | Indicates whether to display labels of the next field in the same column on the Pivot Table view | 
