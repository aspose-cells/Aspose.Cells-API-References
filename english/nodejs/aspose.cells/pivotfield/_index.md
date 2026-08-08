---
title: "PivotField"
linktitle: "PivotField"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents a field in a PivotTable report."
type: docs
weight: 2750
url: /nodejs/aspose.cells/pivotfield/
---

## PivotField class

Represents a field in a PivotTable report.

## Methods

| Name | Description |
| --- | --- |
| [addCalculatedItem(name, formula)](#addcalculateditem) | Add a calculated formula item to the pivot field. Only supports to add calculated item to Row/Column field. |
| [clearFilter()](#clearfilter) |  |
| [filterByDate()](#filterbydate) |  |
| [filterByLabel()](#filterbylabel) |  |
| [filterByValue()](#filterbyvalue) |  |
| [filterTop10()](#filtertop10) |  |
| [getAutoShowCount()](#getautoshowcount) | Represent the number of top or bottom items that are automatically shown in the specified PivotTable field. |
| [getAutoShowField()](#getautoshowfield) | Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields. |
| [getAutoSortField()](#getautosortfield) | Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fie |
| [getBaseFieldIndex()](#getbasefieldindex) | Represents the base field for a custom calculation when the ShowDataAs calculation is in use. NOTE: This property is now |
| [getBaseIndex()](#getbaseindex) | Represents the PivotField index in the base PivotFields. |
| [getBaseItemIndex()](#getbaseitemindex) | Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for |
| [getBaseItemPosition()](#getbaseitemposition) | Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for |
| [getCalculatedFieldFormula()](#getcalculatedfieldformula) | Get the formula string of the specified calculated field . |
| [getCurrentPageItem()](#getcurrentpageitem) | Represents the current page item showing for the page field (valid only for page fields). |
| [getDataDisplayFormat()](#getdatadisplayformat) | Represents how to display the values in a data field of the pivot report. The value of the property is PivotFieldDataDis |
| [getDisplayName()](#getdisplayname) | Represents the PivotField display name. |
| [getDragToColumn()](#getdragtocolumn) | Indicates whether the specified field can be dragged to the column position. The default value is true. |
| [getDragToData()](#getdragtodata) | Indicates whether the specified field can be dragged to the data position. The default value is true. |
| [getDragToHide()](#getdragtohide) | Indicates whether the specified field can be dragged to the hide position. The default value is true. |
| [getDragToPage()](#getdragtopage) | Indicates whether the specified field can be dragged to the page position. The default value is true. |
| [getDragToRow()](#getdragtorow) | Indicates whether the specified field can be dragged to the row position. The default value is true. |
| [getFilters()](#getfilters) | Gets all pivot filters of this pivot field. |
| [getFormula()](#getformula) |  |
| [getFunction()](#getfunction) | Represents the function used to summarize the PivotTable data field. The value of the property is ConsolidationFunction  |
| [getGroupSettings()](#getgroupsettings) | Gets the group settings of the pivot field. If this field is not grouped, Null will be returned. |
| [getInsertBlankRow()](#getinsertblankrow) | Indicates whether inserting blank line after each item. |
| [getItemCount()](#getitemcount) | Gets the count of the base items in this pivot field. |
| [getItems()](#getitems) | Get all labels of pivot items in this field. |
| [getMaxValue()](#getmaxvalue) |  |
| [getMinValue()](#getminvalue) |  |
| [getName()](#getname) | Represents the name of PivotField. |
| [getNonAutoSortDefault()](#getnonautosortdefault) | Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data so |
| [getNumber()](#getnumber) | Represents the built-in display format of numbers and dates. |
| [getNumberFormat()](#getnumberformat) | Represents the custom display format of numbers and dates. |
| [getOriginalItems()](#getoriginalitems) | Get the original base items; |
| [getPivotFilterByType()](#getpivotfilterbytype) | Gets the pivot filter of the pivot field by type |
| [getPivotFilters()](#getpivotfilters) | Gets the pivot filters of the pivot field NOTE: This method is now obsolete. Instead, please use PivotField.GetFilters() |
| [getPivotItems()](#getpivotitems) | Gets the pivot items of the pivot field |
| [getPosition()](#getposition) | Represents the index of PivotField in the region. |
| [getRegionType()](#getregiontype) | The value of the property is PivotFieldType integer constant. |
| [getShowAllItems()](#getshowallitems) | Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with  |
| [getShowCompact()](#getshowcompact) | Indicates whether display labels from the next field in the same column on the Pivot Table view |
| [getShowInOutlineForm()](#getshowinoutlineform) | Indicates whether layout this field in outline form on the Pivot Table view |
| [getShowSubtotalAtTop()](#getshowsubtotalattop) | when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom Only wor |
| [getShowValuesSetting()](#getshowvaluessetting) | Gets the settings of showing values as when the ShowDataAs calculation is in use. |
| [getSortSetting()](#getsortsetting) |  |
| [getSubtotals(subtotalType)](#getsubtotals) | Indicates whether showing specified subtotal. |
| [groupBy(interval, newField)](#groupby) | Automatically group the field with internal |
| [groupBy()](#groupby-1) |  |
| [groupBy(start, end, groups, interval, firstAsNewField)](#groupby-2) | Group the file by the date group types. |
| [groupBy()](#groupby-3) |  |
| [groupBy(start, end, interval, newField)](#groupby-4) | Group the file by number. |
| [groupBy()](#groupby-5) |  |
| [groupBy(customGroupItems, newField)](#groupby-6) | Custom group the field. |
| [hideDetail(isHiddenDetail)](#hidedetail) | Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field. |
| [hideItem(itemValue, isHidden)](#hideitem) | Sets whether the specific PivotItem in a data field is hidden. |
| [hideItem(index, isHidden)](#hideitem-1) | Sets whether the specific PivotItem in a data field is hidden. |
| [hideItemDetail(index, isHiddenDetail)](#hideitemdetail) | Sets whether the specific PivotItem in a pivot field is hidden detail. |
| [initPivotItems()](#initpivotitems) | Init the pivot items of the pivot field |
| [isAscendShow()](#isascendshow) | Indicates whether the specified PivotTable field is autoshown ascending. |
| [isAscendSort()](#isascendsort) | Indicates whether the specified PivotTable field is autosorted ascending. |
| [isAutoShow()](#isautoshow) | Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003. |
| [isAutoSort()](#isautosort) | Indicates whether the specified PivotTable field is automatically sorted. |
| [isAutoSubtotals()](#isautosubtotals) | Indicates whether the specified field shows automatic subtotals. Default is true. |
| [isCalculatedField()](#iscalculatedfield) | Indicates whether the specified PivotTable field is calculated field. |
| [isHiddenItem(index)](#ishiddenitem) | Gets whether the specific PivotItem is hidden. |
| [isHiddenItemDetail(index)](#ishiddenitemdetail) | Gets whether hidding the detail of the specific PivotItem.. |
| [isIncludeNewItemsInFilter()](#isincludenewitemsinfilter) | Indicates whether including new items to the field in manual filter. The default value is false. |
| [isInsertPageBreaksBetweenItems()](#isinsertpagebreaksbetweenitems) | Indicates whether inserting page breaks after each item. The default value is false. |
| [isMultipleItemSelectionAllowed()](#ismultipleitemselectionallowed) | indicates whether the field can have multiple items selected in the page field The default value is false. |
| [isRepeatItemLabels()](#isrepeatitemlabels) | Indicates whether repeating labels of the field in the region. The default value is false. |
| [isValueFields()](#isvaluefields) |  |
| [isValuesField()](#isvaluesfield) |  |
| [setAscendShow()](#setascendshow) | Indicates whether the specified PivotTable field is autoshown ascending. |
| [setAscendSort()](#setascendsort) | Indicates whether the specified PivotTable field is autosorted ascending. |
| [setAutoShow()](#setautoshow) | Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003. |
| [setAutoShowCount()](#setautoshowcount) | Represent the number of top or bottom items that are automatically shown in the specified PivotTable field. |
| [setAutoShowField()](#setautoshowfield) | Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields. |
| [setAutoSort()](#setautosort) | Indicates whether the specified PivotTable field is automatically sorted. |
| [setAutoSortField()](#setautosortfield) | Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fie |
| [setAutoSubtotals()](#setautosubtotals) | Indicates whether the specified field shows automatic subtotals. Default is true. |
| [setBaseFieldIndex()](#setbasefieldindex) | Represents the base field for a custom calculation when the ShowDataAs calculation is in use. NOTE: This property is now |
| [setBaseIndex()](#setbaseindex) | Represents the PivotField index in the base PivotFields. |
| [setBaseItemIndex()](#setbaseitemindex) | Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for |
| [setBaseItemPosition()](#setbaseitemposition) | Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for |
| [setCurrentPageItem()](#setcurrentpageitem) | Represents the current page item showing for the page field (valid only for page fields). |
| [setDataDisplayFormat()](#setdatadisplayformat) | Represents how to display the values in a data field of the pivot report. The value of the property is PivotFieldDataDis |
| [setDisplayName()](#setdisplayname) | Represents the PivotField display name. |
| [setDragToColumn()](#setdragtocolumn) | Indicates whether the specified field can be dragged to the column position. The default value is true. |
| [setDragToData()](#setdragtodata) | Indicates whether the specified field can be dragged to the data position. The default value is true. |
| [setDragToHide()](#setdragtohide) | Indicates whether the specified field can be dragged to the hide position. The default value is true. |
| [setDragToPage()](#setdragtopage) | Indicates whether the specified field can be dragged to the page position. The default value is true. |
| [setDragToRow()](#setdragtorow) | Indicates whether the specified field can be dragged to the row position. The default value is true. |
| [setFunction()](#setfunction) | Represents the function used to summarize the PivotTable data field. The value of the property is ConsolidationFunction  |
| [setIncludeNewItemsInFilter()](#setincludenewitemsinfilter) | Indicates whether including new items to the field in manual filter. The default value is false. |
| [setInsertBlankRow()](#setinsertblankrow) | Indicates whether inserting blank line after each item. |
| [setInsertPageBreaksBetweenItems()](#setinsertpagebreaksbetweenitems) | Indicates whether inserting page breaks after each item. The default value is false. |
| [setMultipleItemSelectionAllowed()](#setmultipleitemselectionallowed) | indicates whether the field can have multiple items selected in the page field The default value is false. |
| [setName()](#setname) | Represents the name of PivotField. |
| [setNonAutoSortDefault()](#setnonautosortdefault) | Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data so |
| [setNumber()](#setnumber) | Represents the built-in display format of numbers and dates. |
| [setNumberFormat()](#setnumberformat) | Represents the custom display format of numbers and dates. |
| [setRepeatItemLabels()](#setrepeatitemlabels) | Indicates whether repeating labels of the field in the region. The default value is false. |
| [setShowAllItems()](#setshowallitems) | Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with  |
| [setShowCompact()](#setshowcompact) | Indicates whether display labels from the next field in the same column on the Pivot Table view |
| [setShowInOutlineForm()](#setshowinoutlineform) | Indicates whether layout this field in outline form on the Pivot Table view |
| [setShowSubtotalAtTop()](#setshowsubtotalattop) | when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom Only wor |
| [setSubtotals(subtotalType, shown)](#setsubtotals) | Sets whether the specified field shows that subtotals. PivotFieldSubtotalType |
| [showValuesAs(displayFormat, baseField, baseItemPositionType, baseItem)](#showvaluesas) | Show value of data field as different display format when the ShowDataAs calculation is in use. Only for data field. |
| [sortBy()](#sortby) |  |
| [sortBy()](#sortby-1) |  |
| [ungroup()](#ungroup) | Ungroup the pivot field. |

### addCalculatedItem(name, formula) {#addcalculateditem}

Add a calculated formula item to the pivot field. Only supports to add calculated item to Row/Column field.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The item's name. |
| formula | String | The formula of pivot item. |

### clearFilter() {#clearfilter}

### filterByDate() {#filterbydate}

### filterByLabel() {#filterbylabel}

### filterByValue() {#filterbyvalue}

### filterTop10() {#filtertop10}

### getAutoShowCount() {#getautoshowcount}

Represent the number of top or bottom items that are automatically shown in the specified PivotTable field.

### getAutoShowField() {#getautoshowfield}

Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields.

### getAutoSortField() {#getautosortfield}

Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fields.

### getBaseFieldIndex() {#getbasefieldindex}

Represents the base field for a custom calculation when the ShowDataAs calculation is in use. NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.BaseFieldIndex property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### getBaseIndex() {#getbaseindex}

Represents the PivotField index in the base PivotFields.

### getBaseItemIndex() {#getbaseitemindex}

Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.BaseItemIndex property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### getBaseItemPosition() {#getbaseitemposition}

Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. The value of the property is PivotItemPosition integer constant.PivotItemPosition NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.BaseItemType property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### getCalculatedFieldFormula() {#getcalculatedfieldformula}

Get the formula string of the specified calculated field .

### getCurrentPageItem() {#getcurrentpageitem}

Represents the current page item showing for the page field (valid only for page fields).

### getDataDisplayFormat() {#getdatadisplayformat}

Represents how to display the values in a data field of the pivot report. The value of the property is PivotFieldDataDisplayFormat integer constant.PivotFieldDataDisplayFormat NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.CalculationType property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### getDisplayName() {#getdisplayname}

Represents the PivotField display name.

### getDragToColumn() {#getdragtocolumn}

Indicates whether the specified field can be dragged to the column position. The default value is true.

### getDragToData() {#getdragtodata}

Indicates whether the specified field can be dragged to the data position. The default value is true.

### getDragToHide() {#getdragtohide}

Indicates whether the specified field can be dragged to the hide position. The default value is true.

### getDragToPage() {#getdragtopage}

Indicates whether the specified field can be dragged to the page position. The default value is true.

### getDragToRow() {#getdragtorow}

Indicates whether the specified field can be dragged to the row position. The default value is true.

### getFilters() {#getfilters}

Gets all pivot filters of this pivot field.

### getFormula() {#getformula}

### getFunction() {#getfunction}

Represents the function used to summarize the PivotTable data field. The value of the property is ConsolidationFunction integer constant.

### getGroupSettings() {#getgroupsettings}

Gets the group settings of the pivot field. If this field is not grouped, Null will be returned.

### getInsertBlankRow() {#getinsertblankrow}

Indicates whether inserting blank line after each item.

### getItemCount() {#getitemcount}

Gets the count of the base items in this pivot field.

### getItems() {#getitems}

Get all labels of pivot items in this field.

### getMaxValue() {#getmaxvalue}

### getMinValue() {#getminvalue}

### getName() {#getname}

Represents the name of PivotField.

### getNonAutoSortDefault() {#getnonautosortdefault}

Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort.

### getNumber() {#getnumber}

Represents the built-in display format of numbers and dates.

### getNumberFormat() {#getnumberformat}

Represents the custom display format of numbers and dates.

### getOriginalItems() {#getoriginalitems}

Get the original base items;

### getPivotFilterByType() {#getpivotfilterbytype}

Gets the pivot filter of the pivot field by type

### getPivotFilters() {#getpivotfilters}

Gets the pivot filters of the pivot field NOTE: This method is now obsolete. Instead, please use PivotField.GetFilters() method. This method will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.

### getPivotItems() {#getpivotitems}

Gets the pivot items of the pivot field

### getPosition() {#getposition}

Represents the index of PivotField in the region.

### getRegionType() {#getregiontype}

The value of the property is PivotFieldType integer constant.

### getShowAllItems() {#getshowallitems}

Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with no data The default value is false.

### getShowCompact() {#getshowcompact}

Indicates whether display labels from the next field in the same column on the Pivot Table view

### getShowInOutlineForm() {#getshowinoutlineform}

Indicates whether layout this field in outline form on the Pivot Table view

### getShowSubtotalAtTop() {#getshowsubtotalattop}

when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom Only works when ShowInOutlineForm is true.

### getShowValuesSetting() {#getshowvaluessetting}

Gets the settings of showing values as when the ShowDataAs calculation is in use.

### getSortSetting() {#getsortsetting}

### getSubtotals(subtotalType) {#getsubtotals}

Indicates whether showing specified subtotal.

| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | Number | PivotFieldSubtotalType |

**Returns:** boolean — `boolean` Returns whether showing specified subtotal.

### groupBy(interval, newField) {#groupby}

Automatically group the field with internal

| Parameter | Type | Description |
| --- | --- | --- |
| interval | Number | The internal of group. Automatic value will be assigned if it's zero, |
| newField | boolean | Indicates whether adding a new field to the pivottable. |

### groupBy() {#groupby-1}

### groupBy(start, end, groups, interval, firstAsNewField) {#groupby-2}

Group the file by the date group types.

| Parameter | Type | Description |
| --- | --- | --- |
| start | DateTime | The start datetime |
| end | DateTime | The end of datetime |
| groups | Array of Number | Group types |
| interval | Number | The interval |
| firstAsNewField | boolean | Indicates whether adding a new field to the pivottable. Only for the first group item. |

### groupBy() {#groupby-3}

### groupBy(start, end, interval, newField) {#groupby-4}

Group the file by number.

| Parameter | Type | Description |
| --- | --- | --- |
| start | Number | The start value |
| end | Number | The end of value |
| interval | Number | The interval |
| newField | boolean | Indicates whether adding a new field to the pivottable |

### groupBy() {#groupby-5}

### groupBy(customGroupItems, newField) {#groupby-6}

Custom group the field.

| Parameter | Type | Description |
| --- | --- | --- |
| customGroupItems | Array ofCustomPiovtFieldGroupItem | The custom group items. |
| newField | boolean | Indicates whether adding a new field to the pivottable |

### hideDetail(isHiddenDetail) {#hidedetail}

Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field.

| Parameter | Type | Description |
| --- | --- | --- |
| isHiddenDetail | boolean | Whether hide the detail of the pivot field. |

### hideItem(itemValue, isHidden) {#hideitem}

Sets whether the specific PivotItem in a data field is hidden.

| Parameter | Type | Description |
| --- | --- | --- |
| itemValue | String | the value of the pivotItem in the pivotField. |
| isHidden | boolean | whether the specific PivotItem is hidden |

### hideItem(index, isHidden) {#hideitem-1}

Sets whether the specific PivotItem in a data field is hidden.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | the index of the pivotItem in the pivotField. |
| isHidden | boolean | whether the specific PivotItem is hidden |

### hideItemDetail(index, isHiddenDetail) {#hideitemdetail}

Sets whether the specific PivotItem in a pivot field is hidden detail.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | the index of the pivotItem in the pivotField. |
| isHiddenDetail | boolean | whether the specific PivotItem is hidden |

### initPivotItems() {#initpivotitems}

Init the pivot items of the pivot field

### isAscendShow() {#isascendshow}

Indicates whether the specified PivotTable field is autoshown ascending.

### isAscendSort() {#isascendsort}

Indicates whether the specified PivotTable field is autosorted ascending.

### isAutoShow() {#isautoshow}

Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003.

### isAutoSort() {#isautosort}

Indicates whether the specified PivotTable field is automatically sorted.

### isAutoSubtotals() {#isautosubtotals}

Indicates whether the specified field shows automatic subtotals. Default is true.

### isCalculatedField() {#iscalculatedfield}

Indicates whether the specified PivotTable field is calculated field.

### isHiddenItem(index) {#ishiddenitem}

Gets whether the specific PivotItem is hidden.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index of the pivotItem in the pivotField. |

**Returns:** boolean — `boolean` whether the specific PivotItem is hidden

### isHiddenItemDetail(index) {#ishiddenitemdetail}

Gets whether hidding the detail of the specific PivotItem..

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index of the pivotItem in the pivotField. |

**Returns:** boolean — `boolean` whether the specific PivotItem is hidden detail

### isIncludeNewItemsInFilter() {#isincludenewitemsinfilter}

Indicates whether including new items to the field in manual filter. The default value is false.

### isInsertPageBreaksBetweenItems() {#isinsertpagebreaksbetweenitems}

Indicates whether inserting page breaks after each item. The default value is false.

### isMultipleItemSelectionAllowed() {#ismultipleitemselectionallowed}

indicates whether the field can have multiple items selected in the page field The default value is false.

### isRepeatItemLabels() {#isrepeatitemlabels}

Indicates whether repeating labels of the field in the region. The default value is false.

### isValueFields() {#isvaluefields}

### isValuesField() {#isvaluesfield}

### setAscendShow() {#setascendshow}

Indicates whether the specified PivotTable field is autoshown ascending.

### setAscendSort() {#setascendsort}

Indicates whether the specified PivotTable field is autosorted ascending.

### setAutoShow() {#setautoshow}

Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003.

### setAutoShowCount() {#setautoshowcount}

Represent the number of top or bottom items that are automatically shown in the specified PivotTable field.

### setAutoShowField() {#setautoshowfield}

Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields.

### setAutoSort() {#setautosort}

Indicates whether the specified PivotTable field is automatically sorted.

### setAutoSortField() {#setautosortfield}

Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fields.

### setAutoSubtotals() {#setautosubtotals}

Indicates whether the specified field shows automatic subtotals. Default is true.

### setBaseFieldIndex() {#setbasefieldindex}

Represents the base field for a custom calculation when the ShowDataAs calculation is in use. NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.BaseFieldIndex property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### setBaseIndex() {#setbaseindex}

Represents the PivotField index in the base PivotFields.

### setBaseItemIndex() {#setbaseitemindex}

Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.BaseItemIndex property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### setBaseItemPosition() {#setbaseitemposition}

Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. The value of the property is PivotItemPosition integer constant.PivotItemPosition NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.BaseItemType property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### setCurrentPageItem() {#setcurrentpageitem}

Represents the current page item showing for the page field (valid only for page fields).

### setDataDisplayFormat() {#setdatadisplayformat}

Represents how to display the values in a data field of the pivot report. The value of the property is PivotFieldDataDisplayFormat integer constant.PivotFieldDataDisplayFormat NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.CalculationType property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### setDisplayName() {#setdisplayname}

Represents the PivotField display name.

### setDragToColumn() {#setdragtocolumn}

Indicates whether the specified field can be dragged to the column position. The default value is true.

### setDragToData() {#setdragtodata}

Indicates whether the specified field can be dragged to the data position. The default value is true.

### setDragToHide() {#setdragtohide}

Indicates whether the specified field can be dragged to the hide position. The default value is true.

### setDragToPage() {#setdragtopage}

Indicates whether the specified field can be dragged to the page position. The default value is true.

### setDragToRow() {#setdragtorow}

Indicates whether the specified field can be dragged to the row position. The default value is true.

### setFunction() {#setfunction}

Represents the function used to summarize the PivotTable data field. The value of the property is ConsolidationFunction integer constant.

### setIncludeNewItemsInFilter() {#setincludenewitemsinfilter}

Indicates whether including new items to the field in manual filter. The default value is false.

### setInsertBlankRow() {#setinsertblankrow}

Indicates whether inserting blank line after each item.

### setInsertPageBreaksBetweenItems() {#setinsertpagebreaksbetweenitems}

Indicates whether inserting page breaks after each item. The default value is false.

### setMultipleItemSelectionAllowed() {#setmultipleitemselectionallowed}

indicates whether the field can have multiple items selected in the page field The default value is false.

### setName() {#setname}

Represents the name of PivotField.

### setNonAutoSortDefault() {#setnonautosortdefault}

Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort.

### setNumber() {#setnumber}

Represents the built-in display format of numbers and dates.

### setNumberFormat() {#setnumberformat}

Represents the custom display format of numbers and dates.

### setRepeatItemLabels() {#setrepeatitemlabels}

Indicates whether repeating labels of the field in the region. The default value is false.

### setShowAllItems() {#setshowallitems}

Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with no data The default value is false.

### setShowCompact() {#setshowcompact}

Indicates whether display labels from the next field in the same column on the Pivot Table view

### setShowInOutlineForm() {#setshowinoutlineform}

Indicates whether layout this field in outline form on the Pivot Table view

### setShowSubtotalAtTop() {#setshowsubtotalattop}

when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom Only works when ShowInOutlineForm is true.

### setSubtotals(subtotalType, shown) {#setsubtotals}

Sets whether the specified field shows that subtotals. PivotFieldSubtotalType

| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | Number | PivotFieldSubtotalType |
| shown | boolean | whether the specified field shows that subtotals. |

### showValuesAs(displayFormat, baseField, baseItemPositionType, baseItem) {#showvaluesas}

Show value of data field as different display format when the ShowDataAs calculation is in use. Only for data field.

| Parameter | Type | Description |
| --- | --- | --- |
| displayFormat | Number | PivotFieldDataDisplayFormat |
| baseField | Number | The index to the field which ShowDataAs calculation bases on. |
| baseItemPositionType | Number | PivotItemPositionType |
| baseItem | Number | The index to the base item which ShowDataAs calculation bases on. Only works when baseItemPositionType is custom. |

### sortBy() {#sortby}

### sortBy() {#sortby-1}

### ungroup() {#ungroup}

Ungroup the pivot field.
