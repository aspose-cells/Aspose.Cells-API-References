##PivotField Class
'PivotField class. Encapsulates the object that represents pivotfield in Go.'
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
|[GetGroupSettings](./getgroupsettings/) | Gets the group settings of the pivot field. |
|[InitPivotItems](./initpivotitems/) | Init the pivot items of the pivot field |
|[GroupBy_Double_Bool](./groupby_double_bool/) | Automatically group the field with internal |
|[GroupBy_Date_Date_PivotGroupByTypeArray_Double_Bool](./groupby_date_date_pivotgroupbytypearray_double_bool/) | Group the file by the date group types. |
|[GroupBy_Double_Double_Double_Bool](./groupby_double_double_double_bool/) | Group the file by number. |
|[GroupBy_CustomPiovtFieldGroupItemArray_Bool](./groupby_custompiovtfieldgroupitemarray_bool/) | Custom group the field. |
|[Ungroup](./ungroup/) | Ungroup the pivot field. |
|[GetPivotFilterByType](./getpivotfilterbytype/) | Gets the pivot filter of the pivot field by type |
|[GetFilters](./getfilters/) | Gets all pivot filters of this pivot field. |
|[ClearFilter](./clearfilter/) | Clears filter setting on this pivot field. |
|[FilterTop10](./filtertop10/) | Filters by values of data pivot field. |
|[FilterByValue](./filterbyvalue/) | Filters by values of data pivot field. |
|[FilterByLabel](./filterbylabel/) | Filters by captions of row or column pivot field. |
|[FilterByDate](./filterbydate/) | Filters by date setting of row or column pivot field. |
|[IsCalculatedField](./iscalculatedfield/) | Indicates whether the specified PivotTable field is calculated field. |
|[GetFormula](./getformula/) | Gets formula of the calculated field . |
|[IsValueFields](./isvaluefields/) | Indicates whether this field represents values fields. |
|[GetBaseIndex](./getbaseindex/) | Represents the PivotField index in the base PivotFields. |
|[SetBaseIndex](./setbaseindex/) | Represents the PivotField index in the base PivotFields. |
|[GetPosition](./getposition/) | Represents the index of PivotField in the region. |
|[GetRegionType](./getregiontype/) | Specifies the region of the PivotTable that this field is displayed. |
|[GetName](./getname/) | Represents the name of PivotField. |
|[SetName](./setname/) | Represents the name of PivotField. |
|[GetDisplayName](./getdisplayname/) | Represents the PivotField display name. |
|[SetDisplayName](./setdisplayname/) | Represents the PivotField display name. |
|[SetSubtotals](./setsubtotals/) | Sets whether the specified field shows that subtotals. |
|[GetSubtotals](./getsubtotals/) | Indicates whether showing specified subtotal. |
|[IsAutoSubtotals](./isautosubtotals/) | Indicates whether the specified field shows automatic subtotals. Default is true. |
|[SetIsAutoSubtotals](./setisautosubtotals/) | Indicates whether the specified field shows automatic subtotals. Default is true. |
|[GetDragToColumn](./getdragtocolumn/) | Indicates whether the specified field can be dragged to the column position.The default value is true. |
|[SetDragToColumn](./setdragtocolumn/) | Indicates whether the specified field can be dragged to the column position.The default value is true. |
|[GetDragToHide](./getdragtohide/) | Indicates whether the specified field can be dragged to the hide position.The default value is true. |
|[SetDragToHide](./setdragtohide/) | Indicates whether the specified field can be dragged to the hide position.The default value is true. |
|[GetDragToRow](./getdragtorow/) | Indicates whether the specified field can be dragged to the row position.The default value is true. |
|[SetDragToRow](./setdragtorow/) | Indicates whether the specified field can be dragged to the row position.The default value is true. |
|[GetDragToPage](./getdragtopage/) | Indicates whether the specified field can be dragged to the page position.The default value is true. |
|[SetDragToPage](./setdragtopage/) | Indicates whether the specified field can be dragged to the page position.The default value is true. |
|[GetDragToData](./getdragtodata/) | Indicates whether the specified field can be dragged to the data position.The default value is true. |
|[SetDragToData](./setdragtodata/) | Indicates whether the specified field can be dragged to the data position.The default value is true. |
|[IsMultipleItemSelectionAllowed](./ismultipleitemselectionallowed/) | indicates whether the field can have multiple itemsselected in the page fieldThe default value is false. |
|[SetIsMultipleItemSelectionAllowed](./setismultipleitemselectionallowed/) | indicates whether the field can have multiple itemsselected in the page fieldThe default value is false. |
|[IsRepeatItemLabels](./isrepeatitemlabels/) | Indicates whether repeating labels of the field in the region.The default value is false. |
|[SetIsRepeatItemLabels](./setisrepeatitemlabels/) | Indicates whether repeating labels of the field in the region.The default value is false. |
|[IsIncludeNewItemsInFilter](./isincludenewitemsinfilter/) | Indicates whether including new items to the field in manual filter.The default value is false. |
|[SetIsIncludeNewItemsInFilter](./setisincludenewitemsinfilter/) | Indicates whether including new items to the field in manual filter.The default value is false. |
|[IsInsertPageBreaksBetweenItems](./isinsertpagebreaksbetweenitems/) | Indicates whether inserting page breaks after each item.The default value is false. |
|[SetIsInsertPageBreaksBetweenItems](./setisinsertpagebreaksbetweenitems/) | Indicates whether inserting page breaks after each item.The default value is false. |
|[GetShowAllItems](./getshowallitems/) | Indicates whether all items displays in the PivotTable report,even if they don't contain summary data.show items with no dataThe default value is false. |
|[SetShowAllItems](./setshowallitems/) | Indicates whether all items displays in the PivotTable report,even if they don't contain summary data.show items with no dataThe default value is false. |
|[SortBy_SortOrder_Int](./sortby_sortorder_int/) | Sorts this pivot field. |
|[SortBy_SortOrder_Int_PivotLineType_String](./sortby_sortorder_int_pivotlinetype_string/) | Sorts this pivot field. |
|[GetNonAutoSortDefault](./getnonautosortdefault/) | Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort. |
|[SetNonAutoSortDefault](./setnonautosortdefault/) | Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort. |
|[IsAutoSort](./isautosort/) | Indicates whether the specified PivotTable field is automatically sorted. |
|[SetIsAutoSort](./setisautosort/) | Indicates whether the specified PivotTable field is automatically sorted. |
|[IsAscendSort](./isascendsort/) | Indicates whether the specified PivotTable field is autosorted ascending. |
|[SetIsAscendSort](./setisascendsort/) | Indicates whether the specified PivotTable field is autosorted ascending. |
|[GetSortSetting](./getsortsetting/) | Gets all settings of auto sorting |
|[GetAutoSortField](./getautosortfield/) | Represents the index of field which is auto sorted.-1 means PivotField itself,others means the position of the data fields. |
|[SetAutoSortField](./setautosortfield/) | Represents the index of field which is auto sorted.-1 means PivotField itself,others means the position of the data fields. |
|[IsAutoShow](./isautoshow/) | Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003. |
|[SetIsAutoShow](./setisautoshow/) | Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003. |
|[IsAscendShow](./isascendshow/) | Indicates whether the specified PivotTable field is autoshown ascending. |
|[SetIsAscendShow](./setisascendshow/) | Indicates whether the specified PivotTable field is autoshown ascending. |
|[GetAutoShowCount](./getautoshowcount/) | Represent the number of top or bottom itemsthat are automatically shown in the specified PivotTable field. |
|[SetAutoShowCount](./setautoshowcount/) | Represent the number of top or bottom itemsthat are automatically shown in the specified PivotTable field. |
|[GetAutoShowField](./getautoshowfield/) | Represents auto show field index. -1 means PivotField itself.It should be the index of the data fields. |
|[SetAutoShowField](./setautoshowfield/) | Represents auto show field index. -1 means PivotField itself.It should be the index of the data fields. |
|[GetFunction](./getfunction/) | Represents the function used to summarize the PivotTable data field. |
|[SetFunction](./setfunction/) | Represents the function used to summarize the PivotTable data field. |
|[ShowValuesAs](./showvaluesas/) | Shows values of data field as different display format when the ShowDataAs calculation is in use. |
|[GetShowValuesSetting](./getshowvaluessetting/) | Gets the settings of showing values as when the ShowDataAs calculation is in use. |
|[GetCurrentPageItem](./getcurrentpageitem/) | Represents the current page item showing for the page field (valid only for page fields). |
|[SetCurrentPageItem](./setcurrentpageitem/) | Represents the current page item showing for the page field (valid only for page fields). |
|[GetNumber](./getnumber/) | Represents the built-in display format of numbers and dates. |
|[SetNumber](./setnumber/) | Represents the built-in display format of numbers and dates. |
|[GetInsertBlankRow](./getinsertblankrow/) | Indicates whether inserting blank line after each item. |
|[SetInsertBlankRow](./setinsertblankrow/) | Indicates whether inserting blank line after each item. |
|[GetShowSubtotalAtTop](./getshowsubtotalattop/) | when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom |
|[SetShowSubtotalAtTop](./setshowsubtotalattop/) | when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom |
|[GetShowInOutlineForm](./getshowinoutlineform/) | Indicates whether layout this field in outline form on the Pivot Table view |
|[SetShowInOutlineForm](./setshowinoutlineform/) | Indicates whether layout this field in outline form on the Pivot Table view |
|[Get_NumberFormat](./get_numberformat/) | Represents the custom display format of numbers and dates. |
|[SetNumberFormat](./setnumberformat/) | Represents the custom display format of numbers and dates. |
|[IsHiddenItem](./ishiddenitem/) | Gets whether the specific PivotItem is hidden. |
|[HideItem_Int_Bool](./hideitem_int_bool/) | Sets whether the specific PivotItem in a data field is hidden. |
|[IsHiddenItemDetail](./ishiddenitemdetail/) | Gets whether hidding the detail of  the specific PivotItem.. |
|[HideItemDetail](./hideitemdetail/) | Sets whether the specific PivotItem in a pivot field is hidden detail. |
|[HideDetail](./hidedetail/) | Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field. |
|[HideItem_String_Bool](./hideitem_string_bool/) | Sets whether the specific PivotItem in a data field is hidden. |
|[GetItems](./getitems/) | Get all labels of pivot items in this field. |
|[GetOriginalItems](./getoriginalitems/) | Get the original base items; |
|[GetItemCount](./getitemcount/) | Gets the count of the base items in this pivot field. |
|[AddCalculatedItem](./addcalculateditem/) | Add a calculated formula item to the pivot field. |
|[GetShowCompact](./getshowcompact/) | Indicates whether display labels from the next field in the same column on the Pivot Table view |
|[SetShowCompact](./setshowcompact/) | Indicates whether display labels from the next field in the same column on the Pivot Table view |
