---
title: "PivotField Class"
linktitle: "PivotField"
articleTitle: "PivotField"
second_title: "Aspose.Cells for Python via Java"
description: "Represents a field in a PivotTable report."
type: docs
weight: 4560
url: /python-java/asposecells.api/pivotfield/
---

## PivotField class

Represents a field in a PivotTable report.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [PivotItems](#pivotitems) | PivotItemCollection | Gets the pivot items of the pivot field |
| [GroupSettings](#groupsettings) | PivotFieldGroupSettings | Gets the group settings of the pivot field. If this field is not grouped, Null will be returned. |
| [IsCalculatedField](#iscalculatedfield) | boolean | Indicates whether the specified PivotTable field is calculated field. |
| [IsValueFields](#isvaluefields) | boolean |  |
| [IsValuesField](#isvaluesfield) | boolean |  |
| [BaseIndex](#baseindex) | int | Represents the PivotField index in the base PivotFields. |
| [Position](#position) | int | Represents the index of PivotField in the region. |
| [RegionType](#regiontype) | int | The value of the property is PivotFieldType integer constant. |
| [Name](#name) | String | Represents the name of PivotField. |
| [DisplayName](#displayname) | String | Represents the PivotField display name. |
| [IsAutoSubtotals](#isautosubtotals) | boolean | Indicates whether the specified field shows automatic subtotals. Default is true. |
| [DragToColumn](#dragtocolumn) | boolean | Indicates whether the specified field can be dragged to the column position. The default value is true. |
| [DragToHide](#dragtohide) | boolean | Indicates whether the specified field can be dragged to the hide position. The default value is true. |
| [DragToRow](#dragtorow) | boolean | Indicates whether the specified field can be dragged to the row position. The default value is true. |
| [DragToPage](#dragtopage) | boolean | Indicates whether the specified field can be dragged to the page position. The default value is true. |
| [DragToData](#dragtodata) | boolean | Indicates whether the specified field can be dragged to the data position. The default value is true. |
| [IsMultipleItemSelectionAllowed](#ismultipleitemselectionallowed) | boolean | indicates whether the field can have multiple items selected in the page field The default value is false. |
| [IsRepeatItemLabels](#isrepeatitemlabels) | boolean | Indicates whether repeating labels of the field in the region. The default value is false. |
| [IsIncludeNewItemsInFilter](#isincludenewitemsinfilter) | boolean | Indicates whether including new items to the field in manual filter. The default value is false. |
| [IsInsertPageBreaksBetweenItems](#isinsertpagebreaksbetweenitems) | boolean | Indicates whether inserting page breaks after each item. The default value is false. |
| [ShowAllItems](#showallitems) | boolean | Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with  |
| [NonAutoSortDefault](#nonautosortdefault) | boolean | Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data so |
| [IsAutoSort](#isautosort) | boolean | Indicates whether the specified PivotTable field is automatically sorted. |
| [IsAscendSort](#isascendsort) | boolean | Indicates whether the specified PivotTable field is autosorted ascending. |
| [SortSetting](#sortsetting) | PivotFieldSortSetting |  |
| [AutoSortField](#autosortfield) | int | Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fie |
| [IsAutoShow](#isautoshow) | boolean | Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003. |
| [IsAscendShow](#isascendshow) | boolean | Indicates whether the specified PivotTable field is autoshown ascending. |
| [AutoShowCount](#autoshowcount) | int | Represent the number of top or bottom items that are automatically shown in the specified PivotTable field. |
| [AutoShowField](#autoshowfield) | int | Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields. |
| [Function](#function) | int | Represents the function used to summarize the PivotTable data field. The value of the property is ConsolidationFunction  |
| [ShowValuesSetting](#showvaluessetting) | PivotShowValuesSetting | Gets the settings of showing values as when the ShowDataAs calculation is in use. |
| [DataDisplayFormat](#datadisplayformat) | int | Represents how to display the values in a data field of the pivot report. The value of the property is PivotFieldDataDis |
| [BaseFieldIndex](#basefieldindex) | int | Represents the base field for a custom calculation when the ShowDataAs calculation is in use. NOTE: This property is now |
| [BaseItemPosition](#baseitemposition) | int | Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for |
| [BaseItemIndex](#baseitemindex) | int | Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for |
| [CurrentPageItem](#currentpageitem) | int | Represents the current page item showing for the page field (valid only for page fields). |
| [InsertBlankRow](#insertblankrow) | boolean | Indicates whether inserting blank line after each item. |
| [ShowSubtotalAtTop](#showsubtotalattop) | boolean | when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom Only wor |
| [ShowInOutlineForm](#showinoutlineform) | boolean | Indicates whether layout this field in outline form on the Pivot Table view |
| [Number](#number) | int | Represents the built-in display format of numbers and dates. |
| [NumberFormat](#numberformat) | String | Represents the custom display format of numbers and dates. |
| [Items](#items) | String[] | Get all labels of pivot items in this field. |
| [OriginalItems](#originalitems) | String[] | Get the original base items; |
| [ItemCount](#itemcount) | int | Gets the count of the base items in this pivot field. |
| [ShowCompact](#showcompact) | boolean | Indicates whether display labels from the next field in the same column on the Pivot Table view |

## Methods

| Name | Description |
| --- | --- |
| [isHiddenItemDetail](#ishiddenitemdetail) | Gets whether hidding the detail of the specific PivotItem.. |
| [hideItemDetail](#hideitemdetail) | Sets whether the specific PivotItem in a pivot field is hidden detail. |
| [hideDetail](#hidedetail) | Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field. |
| [hideItem](#hideitem) | Sets whether the specific PivotItem in a data field is hidden. |
| [addCalculatedItem](#addcalculateditem) | Add a calculated formula item to the pivot field.

Only supports to add calculated item to Row/Column field. |
| [getMaxValue](#getmaxvalue) |  |
| [getMinValue](#getminvalue) |  |
| [initPivotItems](#initpivotitems) | Init the pivot items of the pivot field |
| [groupBy](#groupby) | Automatically group the field with internal |
| [ungroup](#ungroup) | Ungroup the pivot field. |
| [getPivotFilterByType](#getpivotfilterbytype) | Gets the pivot filter of the pivot field by type |
| [getPivotFilters](#getpivotfilters) | Gets the pivot filters of the pivot field

NOTE: This method is now obsolete. Instead, please use PivotField.GetFilters( |
| [getFilters](#getfilters) | Gets all pivot filters of this pivot field. |
| [clearFilter](#clearfilter) |  |
| [filterTop10](#filtertop10) |  |
| [filterByValue](#filterbyvalue) |  |
| [filterByLabel](#filterbylabel) |  |
| [filterByDate](#filterbydate) |  |
| [getCalculatedFieldFormula](#getcalculatedfieldformula) | Get the formula string of the specified calculated field . |
| [getFormula](#getformula) |  |
| [setSubtotals](#setsubtotals) | Sets whether the specified field shows that subtotals. |
| [getSubtotals](#getsubtotals) | Indicates whether showing specified subtotal. |
| [sortBy](#sortby) |  |
| [showValuesAs](#showvaluesas) | Shows values of data field as different display format when the ShowDataAs calculation is in use.

Only for data field. |
| [isHiddenItem](#ishiddenitem) | Gets whether the specific PivotItem is hidden. |

### PivotField.PivotItems property {#pivotitems}

Gets the pivot items of the pivot field

**Type:** PivotItemCollection

### PivotField.GroupSettings property {#groupsettings}

Gets the group settings of the pivot field. If this field is not grouped, Null will be returned.

**Type:** PivotFieldGroupSettings

### PivotField.IsCalculatedField property {#iscalculatedfield}

Indicates whether the specified PivotTable field is calculated field.

**Type:** boolean

### PivotField.IsValueFields property {#isvaluefields}

**Type:** boolean

### PivotField.IsValuesField property {#isvaluesfield}

**Type:** boolean

### PivotField.BaseIndex property {#baseindex}

Represents the PivotField index in the base PivotFields.

**Type:** int

### PivotField.Position property {#position}

Represents the index of PivotField in the region.

**Type:** int

### PivotField.RegionType property {#regiontype}

The value of the property is PivotFieldType integer constant.

**Type:** int

### PivotField.Name property {#name}

Represents the name of PivotField.

**Type:** String

### PivotField.DisplayName property {#displayname}

Represents the PivotField display name.

**Type:** String

### PivotField.IsAutoSubtotals property {#isautosubtotals}

Indicates whether the specified field shows automatic subtotals. Default is true.

**Type:** boolean

### PivotField.DragToColumn property {#dragtocolumn}

Indicates whether the specified field can be dragged to the column position. The default value is true.

**Type:** boolean

### PivotField.DragToHide property {#dragtohide}

Indicates whether the specified field can be dragged to the hide position. The default value is true.

**Type:** boolean

### PivotField.DragToRow property {#dragtorow}

Indicates whether the specified field can be dragged to the row position. The default value is true.

**Type:** boolean

### PivotField.DragToPage property {#dragtopage}

Indicates whether the specified field can be dragged to the page position. The default value is true.

**Type:** boolean

### PivotField.DragToData property {#dragtodata}

Indicates whether the specified field can be dragged to the data position. The default value is true.

**Type:** boolean

### PivotField.IsMultipleItemSelectionAllowed property {#ismultipleitemselectionallowed}

indicates whether the field can have multiple items selected in the page field The default value is false.

**Type:** boolean

### PivotField.IsRepeatItemLabels property {#isrepeatitemlabels}

Indicates whether repeating labels of the field in the region. The default value is false.

**Type:** boolean

### PivotField.IsIncludeNewItemsInFilter property {#isincludenewitemsinfilter}

Indicates whether including new items to the field in manual filter. The default value is false.

**Type:** boolean

### PivotField.IsInsertPageBreaksBetweenItems property {#isinsertpagebreaksbetweenitems}

Indicates whether inserting page breaks after each item. The default value is false.

**Type:** boolean

### PivotField.ShowAllItems property {#showallitems}

Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with no data The default value is false.

**Type:** boolean

### PivotField.NonAutoSortDefault property {#nonautosortdefault}

Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort.

**Type:** boolean

### PivotField.IsAutoSort property {#isautosort}

Indicates whether the specified PivotTable field is automatically sorted.

**Type:** boolean

### PivotField.IsAscendSort property {#isascendsort}

Indicates whether the specified PivotTable field is autosorted ascending.

**Type:** boolean

### PivotField.SortSetting property {#sortsetting}

**Type:** PivotFieldSortSetting

### PivotField.AutoSortField property {#autosortfield}

Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fields.

**Type:** int

### PivotField.IsAutoShow property {#isautoshow}

Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003.

**Type:** boolean

### PivotField.IsAscendShow property {#isascendshow}

Indicates whether the specified PivotTable field is autoshown ascending.

**Type:** boolean

### PivotField.AutoShowCount property {#autoshowcount}

Represent the number of top or bottom items that are automatically shown in the specified PivotTable field.

**Type:** int

### PivotField.AutoShowField property {#autoshowfield}

Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields.

**Type:** int

### PivotField.Function property {#function}

Represents the function used to summarize the PivotTable data field. The value of the property is ConsolidationFunction integer constant.

**Type:** int

### PivotField.ShowValuesSetting property {#showvaluessetting}

Gets the settings of showing values as when the ShowDataAs calculation is in use.

**Type:** PivotShowValuesSetting

### PivotField.DataDisplayFormat property {#datadisplayformat}

Represents how to display the values in a data field of the pivot report. The value of the property is PivotFieldDataDisplayFormat integer constant. NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.CalculationType property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

**Type:** int

### PivotField.BaseFieldIndex property {#basefieldindex}

Represents the base field for a custom calculation when the ShowDataAs calculation is in use. NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.BaseFieldIndex property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

**Type:** int

### PivotField.BaseItemPosition property {#baseitemposition}

Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. The value of the property is PivotItemPosition integer constant. NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.BaseItemType property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

**Type:** int

### PivotField.BaseItemIndex property {#baseitemindex}

Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.BaseItemIndex property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

**Type:** int

### PivotField.CurrentPageItem property {#currentpageitem}

Represents the current page item showing for the page field (valid only for page fields).

**Type:** int

### PivotField.InsertBlankRow property {#insertblankrow}

Indicates whether inserting blank line after each item.

**Type:** boolean

### PivotField.ShowSubtotalAtTop property {#showsubtotalattop}

when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom Only works when ShowInOutlineForm is true.

**Type:** boolean

### PivotField.ShowInOutlineForm property {#showinoutlineform}

Indicates whether layout this field in outline form on the Pivot Table view

**Type:** boolean

### PivotField.Number property {#number}

Represents the built-in display format of numbers and dates.

**Type:** int

### PivotField.NumberFormat property {#numberformat}

Represents the custom display format of numbers and dates.

**Type:** String

### PivotField.Items property {#items}

Get all labels of pivot items in this field.

**Type:** String[]

### PivotField.OriginalItems property {#originalitems}

Get the original base items;

**Type:** String[]

### PivotField.ItemCount property {#itemcount}

Gets the count of the base items in this pivot field.

**Type:** int

### PivotField.ShowCompact property {#showcompact}

Indicates whether display labels from the next field in the same column on the Pivot Table view

**Type:** boolean

### isHiddenItemDetail(index) {#ishiddenitemdetail}

Gets whether hidding the detail of the specific PivotItem..

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index of the pivotItem in the pivotField. |

**Returns:** whether the specific PivotItem is hidden detail

### hideItemDetail(index, isHiddenDetail) {#hideitemdetail}

Sets whether the specific PivotItem in a pivot field is hidden detail.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the index of the pivotItem in the pivotField. |
| isHiddenDetail | boolean | whether the specific PivotItem is hidden |

### hideDetail(isHiddenDetail) {#hidedetail}

Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field.

| Parameter | Type | Description |
| --- | --- | --- |
| isHiddenDetail | boolean | Whether hide the detail of the pivot field. |

### hideItem(itemValue, isHidden) (1 of 2) {#hideitem}

Sets whether the specific PivotItem in a data field is hidden.

| Parameter | Type | Description |
| --- | --- | --- |
| itemValue | String | the value of the pivotItem in the pivotField. |
| isHidden | boolean | whether the specific PivotItem is hidden |

---

### hideItem(index, isHidden) (2 of 2) {#hideitem-1}

Sets whether the specific PivotItem in a data field is hidden.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the index of the pivotItem in the pivotField. |
| isHidden | boolean | whether the specific PivotItem is hidden |

### addCalculatedItem(name, formula) {#addcalculateditem}

Add a calculated formula item to the pivot field.

Only supports to add calculated item to Row/Column field.

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The item's name. |
| formula | String | The formula of pivot item. |

### getMaxValue() {#getmaxvalue}

### getMinValue() {#getminvalue}

### initPivotItems() {#initpivotitems}

Init the pivot items of the pivot field

### groupBy(interval, newField) (1 of 7) {#groupby}

Automatically group the field with internal

| Parameter | Type | Description |
| --- | --- | --- |
| interval | float | The internal of group. Automatic value will be assigned if it's zero, |
| newField | boolean | Indicates whether adding a new field to the pivottable. |

---

### groupBy(groups, interval, newField) (2 of 7) {#groupby-1}

---

### groupBy(start, end, groups, interval, firstAsNewField) (3 of 7) {#groupby-2}

Group the file by the date group types.

| Parameter | Type | Description |
| --- | --- | --- |
| start | DateTime | The start datetime |
| end | DateTime | The end of datetime |
| groups | Number Array | Group types |
| interval | float | The interval |
| firstAsNewField | boolean | Indicates whether adding a new field to the pivottable. Only for the first group item. |

---

### groupBy(isAutoStart, start, isAutoEnd, end, groups, interval, firstAsNewField) (4 of 7) {#groupby-3}

---

### groupBy(start, end, interval, newField) (5 of 7) {#groupby-4}

Group the file by number.

| Parameter | Type | Description |
| --- | --- | --- |
| start | float | The start value |
| end | float | The end of value |
| interval | float | The interval |
| newField | boolean | Indicates whether adding a new field to the pivottable |

---

### groupBy(isAutoStart, start, isAutoEnd, end, interval, newField) (6 of 7) {#groupby-5}

---

### groupBy(customGroupItems, newField) (7 of 7) {#groupby-6}

Custom group the field.

| Parameter | Type | Description |
| --- | --- | --- |
| customGroupItems | CustomPiovtFieldGroupItem[] | The custom group items. |
| newField | boolean | Indicates whether adding a new field to the pivottable |

### ungroup() {#ungroup}

Ungroup the pivot field.

### getPivotFilterByType(type) {#getpivotfilterbytype}

Gets the pivot filter of the pivot field by type

### getPivotFilters() {#getpivotfilters}

Gets the pivot filters of the pivot field

NOTE: This method is now obsolete. Instead, please use PivotField.GetFilters() method. This method will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.

### getFilters() {#getfilters}

Gets all pivot filters of this pivot field.

### clearFilter() {#clearfilter}

### filterTop10(valueFieldIndex, type, isTop, itemCount) {#filtertop10}

### filterByValue(valueFieldIndex, type, value1, value2) {#filterbyvalue}

### filterByLabel(type, label1, label2) {#filterbylabel}

### filterByDate(type, dateTime1, dateTime2) {#filterbydate}

### getCalculatedFieldFormula() {#getcalculatedfieldformula}

Get the formula string of the specified calculated field .

### getFormula() {#getformula}

### setSubtotals(subtotalType, shown) {#setsubtotals}

Sets whether the specified field shows that subtotals.

| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | int | A PivotFieldSubtotalType value. subtotals type. |
| shown | boolean | whether the specified field shows that subtotals. |

### getSubtotals(subtotalType) {#getsubtotals}

Indicates whether showing specified subtotal.

| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | int | A PivotFieldSubtotalType value. subtotal type. |

**Returns:** Returns whether showing specified subtotal.

### sortBy(sortType, fieldSortedBy) (1 of 2) {#sortby}

---

### sortBy(sortType, fieldSortedBy, dataType, cellName) (2 of 2) {#sortby-1}

### showValuesAs(displayFormat, baseField, baseItemPositionType, baseItem) {#showvaluesas}

Shows values of data field as different display format when the ShowDataAs calculation is in use.

Only for data field.

| Parameter | Type | Description |
| --- | --- | --- |
| displayFormat | int | A PivotFieldDataDisplayFormat value. The data display format type. |
| baseField | int | The index to the field which ShowDataAs calculation bases on. |
| baseItemPositionType | int | A PivotItemPositionType value. The position type of base iteam. |
| baseItem | int | The index to the base item which ShowDataAs calculation bases on. Only works when baseItemPositionType is custom. |

### isHiddenItem(index) {#ishiddenitem}

Gets whether the specific PivotItem is hidden.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index of the pivotItem in the pivotField. |

**Returns:** whether the specific PivotItem is hidden
