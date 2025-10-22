##PivotField
Represents a field in a PivotTable report.
## PivotField class
Represents a field in a PivotTable report.
```javascript
class PivotField;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [pivotItems](#pivotItems--)| PivotItemCollection | Readonly. Gets the pivot items of the pivot field |
| [groupSettings](#groupSettings--)| PivotFieldGroupSettings | Readonly. Gets the group settings of the pivot field. |
| [isCalculatedField](#isCalculatedField--)| boolean | Readonly. Indicates whether the specified PivotTable field is calculated field. |
| [isValueFields](#isValueFields--)| boolean | Readonly. Indicates whether this field represents values fields. |
| [baseIndex](#baseIndex--)| number | Represents the PivotField index in the base PivotFields. |
| [position](#position--)| number | Readonly. Represents the index of [PivotField](../pivotfield/) in the region. |
| [regionType](#regionType--)| PivotFieldType | Readonly. Specifies the region of the PivotTable that this field is displayed. |
| [name](#name--)| string | Represents the name of PivotField. |
| [displayName](#displayName--)| string | Represents the PivotField display name. |
| [isAutoSubtotals](#isAutoSubtotals--)| boolean | Indicates whether the specified field shows automatic subtotals. Default is true. |
| [dragToColumn](#dragToColumn--)| boolean | Indicates whether the specified field can be dragged to the column position. The default value is true. |
| [dragToHide](#dragToHide--)| boolean | Indicates whether the specified field can be dragged to the hide position. The default value is true. |
| [dragToRow](#dragToRow--)| boolean | Indicates whether the specified field can be dragged to the row position. The default value is true. |
| [dragToPage](#dragToPage--)| boolean | Indicates whether the specified field can be dragged to the page position. The default value is true. |
| [dragToData](#dragToData--)| boolean | Indicates whether the specified field can be dragged to the data position. The default value is true. |
| [isMultipleItemSelectionAllowed](#isMultipleItemSelectionAllowed--)| boolean | indicates whether the field can have multiple items selected in the page field The default value is false. |
| [isRepeatItemLabels](#isRepeatItemLabels--)| boolean | Indicates whether repeating labels of the field in the region. The default value is false. |
| [isIncludeNewItemsInFilter](#isIncludeNewItemsInFilter--)| boolean | Indicates whether including new items to the field in manual filter. The default value is false. |
| [isInsertPageBreaksBetweenItems](#isInsertPageBreaksBetweenItems--)| boolean | Indicates whether inserting page breaks after each item. The default value is false. |
| [showAllItems](#showAllItems--)| boolean | Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with no data The default value is false. |
| [nonAutoSortDefault](#nonAutoSortDefault--)| boolean | Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort. |
| [isAutoSort](#isAutoSort--)| boolean | Indicates whether the specified PivotTable field is automatically sorted. |
| [isAscendSort](#isAscendSort--)| boolean | Indicates whether the specified PivotTable field is autosorted ascending. |
| [sortSetting](#sortSetting--)| PivotFieldSortSetting | Readonly. Gets all settings of auto sorting |
| [autoSortField](#autoSortField--)| number | Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fields. |
| [isAutoShow](#isAutoShow--)| boolean | Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003. |
| [isAscendShow](#isAscendShow--)| boolean | Indicates whether the specified PivotTable field is autoshown ascending. |
| [autoShowCount](#autoShowCount--)| number | Represent the number of top or bottom items that are automatically shown in the specified PivotTable field. |
| [autoShowField](#autoShowField--)| number | Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields. |
| [function](#function--)| ConsolidationFunction | Represents the function used to summarize the PivotTable data field. |
| [showValuesSetting](#showValuesSetting--)| PivotShowValuesSetting | Readonly. Gets the settings of showing values as when the ShowDataAs calculation is in use. |
| [currentPageItem](#currentPageItem--)| number | Represents the current page item showing for the page field (valid only for page fields). |
| [number](#number--)| number | Represents the built-in display format of numbers and dates. |
| [insertBlankRow](#insertBlankRow--)| boolean | Indicates whether inserting blank line after each item. |
| [showSubtotalAtTop](#showSubtotalAtTop--)| boolean | when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom |
| [showInOutlineForm](#showInOutlineForm--)| boolean | Indicates whether layout this field in outline form on the Pivot Table view |
| [numberFormat](#numberFormat--)| string | Represents the custom display format of numbers and dates. |
| [items](#items--)| string[] | Readonly. Get all labels of pivot items in this field. |
| [originalItems](#originalItems--)| string[] | Readonly. Get the original base items; |
| [itemCount](#itemCount--)| number | Readonly. Gets the count of the base items in this pivot field. |
| [showCompact](#showCompact--)| boolean | Indicates whether display labels from the next field in the same column on the Pivot Table view |
## Methods
| Method | Description |
| --- | --- |
| [getPivotItems()](#getPivotItems--)| <b>@deprecated.</b> Please use the 'pivotItems' property instead. Gets the pivot items of the pivot field |
| [getGroupSettings()](#getGroupSettings--)| <b>@deprecated.</b> Please use the 'groupSettings' property instead. Gets the group settings of the pivot field. |
| [isCalculatedField()](#isCalculatedField--)| <b>@deprecated.</b> Please use the 'isCalculatedField' property instead. Indicates whether the specified PivotTable field is calculated field. |
| [isValueFields()](#isValueFields--)| <b>@deprecated.</b> Please use the 'isValueFields' property instead. Indicates whether this field represents values fields. |
| [getBaseIndex()](#getBaseIndex--)| <b>@deprecated.</b> Please use the 'baseIndex' property instead. Represents the PivotField index in the base PivotFields. |
| [setBaseIndex(number)](#setBaseIndex-number-)| <b>@deprecated.</b> Please use the 'baseIndex' property instead. Represents the PivotField index in the base PivotFields. |
| [getPosition()](#getPosition--)| <b>@deprecated.</b> Please use the 'position' property instead. Represents the index of [PivotField](../pivotfield/) in the region. |
| [getRegionType()](#getRegionType--)| <b>@deprecated.</b> Please use the 'regionType' property instead. Specifies the region of the PivotTable that this field is displayed. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Represents the name of PivotField. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Represents the name of PivotField. |
| [getDisplayName()](#getDisplayName--)| <b>@deprecated.</b> Please use the 'displayName' property instead. Represents the PivotField display name. |
| [setDisplayName(string)](#setDisplayName-string-)| <b>@deprecated.</b> Please use the 'displayName' property instead. Represents the PivotField display name. |
| [isAutoSubtotals()](#isAutoSubtotals--)| <b>@deprecated.</b> Please use the 'isAutoSubtotals' property instead. Indicates whether the specified field shows automatic subtotals. Default is true. |
| [setIsAutoSubtotals(boolean)](#setIsAutoSubtotals-boolean-)| <b>@deprecated.</b> Please use the 'isAutoSubtotals' property instead. Indicates whether the specified field shows automatic subtotals. Default is true. |
| [getDragToColumn()](#getDragToColumn--)| <b>@deprecated.</b> Please use the 'dragToColumn' property instead. Indicates whether the specified field can be dragged to the column position. The default value is true. |
| [setDragToColumn(boolean)](#setDragToColumn-boolean-)| <b>@deprecated.</b> Please use the 'dragToColumn' property instead. Indicates whether the specified field can be dragged to the column position. The default value is true. |
| [getDragToHide()](#getDragToHide--)| <b>@deprecated.</b> Please use the 'dragToHide' property instead. Indicates whether the specified field can be dragged to the hide position. The default value is true. |
| [setDragToHide(boolean)](#setDragToHide-boolean-)| <b>@deprecated.</b> Please use the 'dragToHide' property instead. Indicates whether the specified field can be dragged to the hide position. The default value is true. |
| [getDragToRow()](#getDragToRow--)| <b>@deprecated.</b> Please use the 'dragToRow' property instead. Indicates whether the specified field can be dragged to the row position. The default value is true. |
| [setDragToRow(boolean)](#setDragToRow-boolean-)| <b>@deprecated.</b> Please use the 'dragToRow' property instead. Indicates whether the specified field can be dragged to the row position. The default value is true. |
| [getDragToPage()](#getDragToPage--)| <b>@deprecated.</b> Please use the 'dragToPage' property instead. Indicates whether the specified field can be dragged to the page position. The default value is true. |
| [setDragToPage(boolean)](#setDragToPage-boolean-)| <b>@deprecated.</b> Please use the 'dragToPage' property instead. Indicates whether the specified field can be dragged to the page position. The default value is true. |
| [getDragToData()](#getDragToData--)| <b>@deprecated.</b> Please use the 'dragToData' property instead. Indicates whether the specified field can be dragged to the data position. The default value is true. |
| [setDragToData(boolean)](#setDragToData-boolean-)| <b>@deprecated.</b> Please use the 'dragToData' property instead. Indicates whether the specified field can be dragged to the data position. The default value is true. |
| [isMultipleItemSelectionAllowed()](#isMultipleItemSelectionAllowed--)| <b>@deprecated.</b> Please use the 'isMultipleItemSelectionAllowed' property instead. indicates whether the field can have multiple items selected in the page field The default value is false. |
| [setIsMultipleItemSelectionAllowed(boolean)](#setIsMultipleItemSelectionAllowed-boolean-)| <b>@deprecated.</b> Please use the 'isMultipleItemSelectionAllowed' property instead. indicates whether the field can have multiple items selected in the page field The default value is false. |
| [isRepeatItemLabels()](#isRepeatItemLabels--)| <b>@deprecated.</b> Please use the 'isRepeatItemLabels' property instead. Indicates whether repeating labels of the field in the region. The default value is false. |
| [setIsRepeatItemLabels(boolean)](#setIsRepeatItemLabels-boolean-)| <b>@deprecated.</b> Please use the 'isRepeatItemLabels' property instead. Indicates whether repeating labels of the field in the region. The default value is false. |
| [isIncludeNewItemsInFilter()](#isIncludeNewItemsInFilter--)| <b>@deprecated.</b> Please use the 'isIncludeNewItemsInFilter' property instead. Indicates whether including new items to the field in manual filter. The default value is false. |
| [setIsIncludeNewItemsInFilter(boolean)](#setIsIncludeNewItemsInFilter-boolean-)| <b>@deprecated.</b> Please use the 'isIncludeNewItemsInFilter' property instead. Indicates whether including new items to the field in manual filter. The default value is false. |
| [isInsertPageBreaksBetweenItems()](#isInsertPageBreaksBetweenItems--)| <b>@deprecated.</b> Please use the 'isInsertPageBreaksBetweenItems' property instead. Indicates whether inserting page breaks after each item. The default value is false. |
| [setIsInsertPageBreaksBetweenItems(boolean)](#setIsInsertPageBreaksBetweenItems-boolean-)| <b>@deprecated.</b> Please use the 'isInsertPageBreaksBetweenItems' property instead. Indicates whether inserting page breaks after each item. The default value is false. |
| [getShowAllItems()](#getShowAllItems--)| <b>@deprecated.</b> Please use the 'showAllItems' property instead. Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with no data The default value is false. |
| [setShowAllItems(boolean)](#setShowAllItems-boolean-)| <b>@deprecated.</b> Please use the 'showAllItems' property instead. Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with no data The default value is false. |
| [getNonAutoSortDefault()](#getNonAutoSortDefault--)| <b>@deprecated.</b> Please use the 'nonAutoSortDefault' property instead. Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort. |
| [setNonAutoSortDefault(boolean)](#setNonAutoSortDefault-boolean-)| <b>@deprecated.</b> Please use the 'nonAutoSortDefault' property instead. Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort. |
| [isAutoSort()](#isAutoSort--)| <b>@deprecated.</b> Please use the 'isAutoSort' property instead. Indicates whether the specified PivotTable field is automatically sorted. |
| [setIsAutoSort(boolean)](#setIsAutoSort-boolean-)| <b>@deprecated.</b> Please use the 'isAutoSort' property instead. Indicates whether the specified PivotTable field is automatically sorted. |
| [isAscendSort()](#isAscendSort--)| <b>@deprecated.</b> Please use the 'isAscendSort' property instead. Indicates whether the specified PivotTable field is autosorted ascending. |
| [setIsAscendSort(boolean)](#setIsAscendSort-boolean-)| <b>@deprecated.</b> Please use the 'isAscendSort' property instead. Indicates whether the specified PivotTable field is autosorted ascending. |
| [getSortSetting()](#getSortSetting--)| <b>@deprecated.</b> Please use the 'sortSetting' property instead. Gets all settings of auto sorting |
| [getAutoSortField()](#getAutoSortField--)| <b>@deprecated.</b> Please use the 'autoSortField' property instead. Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fields. |
| [setAutoSortField(number)](#setAutoSortField-number-)| <b>@deprecated.</b> Please use the 'autoSortField' property instead. Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fields. |
| [isAutoShow()](#isAutoShow--)| <b>@deprecated.</b> Please use the 'isAutoShow' property instead. Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003. |
| [setIsAutoShow(boolean)](#setIsAutoShow-boolean-)| <b>@deprecated.</b> Please use the 'isAutoShow' property instead. Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003. |
| [isAscendShow()](#isAscendShow--)| <b>@deprecated.</b> Please use the 'isAscendShow' property instead. Indicates whether the specified PivotTable field is autoshown ascending. |
| [setIsAscendShow(boolean)](#setIsAscendShow-boolean-)| <b>@deprecated.</b> Please use the 'isAscendShow' property instead. Indicates whether the specified PivotTable field is autoshown ascending. |
| [getAutoShowCount()](#getAutoShowCount--)| <b>@deprecated.</b> Please use the 'autoShowCount' property instead. Represent the number of top or bottom items that are automatically shown in the specified PivotTable field. |
| [setAutoShowCount(number)](#setAutoShowCount-number-)| <b>@deprecated.</b> Please use the 'autoShowCount' property instead. Represent the number of top or bottom items that are automatically shown in the specified PivotTable field. |
| [getAutoShowField()](#getAutoShowField--)| <b>@deprecated.</b> Please use the 'autoShowField' property instead. Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields. |
| [setAutoShowField(number)](#setAutoShowField-number-)| <b>@deprecated.</b> Please use the 'autoShowField' property instead. Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields. |
| [getFunction()](#getFunction--)| <b>@deprecated.</b> Please use the 'function' property instead. Represents the function used to summarize the PivotTable data field. |
| [setFunction(ConsolidationFunction)](#setFunction-consolidationfunction-)| <b>@deprecated.</b> Please use the 'function' property instead. Represents the function used to summarize the PivotTable data field. |
| [getShowValuesSetting()](#getShowValuesSetting--)| <b>@deprecated.</b> Please use the 'showValuesSetting' property instead. Gets the settings of showing values as when the ShowDataAs calculation is in use. |
| [getCurrentPageItem()](#getCurrentPageItem--)| <b>@deprecated.</b> Please use the 'currentPageItem' property instead. Represents the current page item showing for the page field (valid only for page fields). |
| [setCurrentPageItem(number)](#setCurrentPageItem-number-)| <b>@deprecated.</b> Please use the 'currentPageItem' property instead. Represents the current page item showing for the page field (valid only for page fields). |
| [getNumber()](#getNumber--)| <b>@deprecated.</b> Please use the 'number' property instead. Represents the built-in display format of numbers and dates. |
| [setNumber(number)](#setNumber-number-)| <b>@deprecated.</b> Please use the 'number' property instead. Represents the built-in display format of numbers and dates. |
| [getInsertBlankRow()](#getInsertBlankRow--)| <b>@deprecated.</b> Please use the 'insertBlankRow' property instead. Indicates whether inserting blank line after each item. |
| [setInsertBlankRow(boolean)](#setInsertBlankRow-boolean-)| <b>@deprecated.</b> Please use the 'insertBlankRow' property instead. Indicates whether inserting blank line after each item. |
| [getShowSubtotalAtTop()](#getShowSubtotalAtTop--)| <b>@deprecated.</b> Please use the 'showSubtotalAtTop' property instead. when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom |
| [setShowSubtotalAtTop(boolean)](#setShowSubtotalAtTop-boolean-)| <b>@deprecated.</b> Please use the 'showSubtotalAtTop' property instead. when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom |
| [getShowInOutlineForm()](#getShowInOutlineForm--)| <b>@deprecated.</b> Please use the 'showInOutlineForm' property instead. Indicates whether layout this field in outline form on the Pivot Table view |
| [setShowInOutlineForm(boolean)](#setShowInOutlineForm-boolean-)| <b>@deprecated.</b> Please use the 'showInOutlineForm' property instead. Indicates whether layout this field in outline form on the Pivot Table view |
| [get_NumberFormat()](#get_NumberFormat--)| <b>@deprecated.</b> Please use the 'numberFormat' property instead. Represents the custom display format of numbers and dates. |
| [setNumberFormat(string)](#setNumberFormat-string-)| <b>@deprecated.</b> Please use the 'numberFormat' property instead. Represents the custom display format of numbers and dates. |
| [getItems()](#getItems--)| <b>@deprecated.</b> Please use the 'items' property instead. Get all labels of pivot items in this field. |
| [getOriginalItems()](#getOriginalItems--)| <b>@deprecated.</b> Please use the 'originalItems' property instead. Get the original base items; |
| [getItemCount()](#getItemCount--)| <b>@deprecated.</b> Please use the 'itemCount' property instead. Gets the count of the base items in this pivot field. |
| [getShowCompact()](#getShowCompact--)| <b>@deprecated.</b> Please use the 'showCompact' property instead. Indicates whether display labels from the next field in the same column on the Pivot Table view |
| [setShowCompact(boolean)](#setShowCompact-boolean-)| <b>@deprecated.</b> Please use the 'showCompact' property instead. Indicates whether display labels from the next field in the same column on the Pivot Table view |
| [initPivotItems()](#initPivotItems--)| Init the pivot items of the pivot field |
| [groupBy(number, boolean)](#groupBy-number-boolean-)| Automatically group the field with internal |
| [groupBy(Date, Date, PivotGroupByType[], number, boolean)](#groupBy-date-date-pivotgroupbytypearray-number-boolean-)| Group the file by the date group types. |
| [groupBy(number, number, number, boolean)](#groupBy-number-number-number-boolean-)| Group the file by number. |
| [groupBy(CustomPiovtFieldGroupItem[], boolean)](#groupBy-custompiovtfieldgroupitemarray-boolean-)| Custom group the field. |
| [ungroup()](#ungroup--)| Ungroup the pivot field. |
| [getPivotFilterByType(PivotFilterType)](#getPivotFilterByType-pivotfiltertype-)| Gets the pivot filter of the pivot field by type |
| [getFilters()](#getFilters--)| Gets all pivot filters of this pivot field. |
| [clearFilter()](#clearFilter--)| Clears filter setting on this pivot field. |
| [filterTop10(number, PivotFilterType, boolean, number)](#filterTop10-number-pivotfiltertype-boolean-number-)| Filters by values of data pivot field. |
| [filterByValue(number, PivotFilterType, number, number)](#filterByValue-number-pivotfiltertype-number-number-)| Filters by values of data pivot field. |
| [filterByLabel(PivotFilterType, string, string)](#filterByLabel-pivotfiltertype-string-string-)| Filters by captions of row or column pivot field. |
| [filterByDate(PivotFilterType, Date, Date)](#filterByDate-pivotfiltertype-date-date-)| Filters by date setting of row or column pivot field. |
| [getFormula()](#getFormula--)| Gets formula of the calculated field . |
| [setSubtotals(PivotFieldSubtotalType, boolean)](#setSubtotals-pivotfieldsubtotaltype-boolean-)| Sets whether the specified field shows that subtotals. |
| [getSubtotals(PivotFieldSubtotalType)](#getSubtotals-pivotfieldsubtotaltype-)| Indicates whether showing specified subtotal. |
| [sortBy(SortOrder, number)](#sortBy-sortorder-number-)| Sorts this pivot field. |
| [sortBy(SortOrder, number, PivotLineType, string)](#sortBy-sortorder-number-pivotlinetype-string-)| Sorts this pivot field. |
| [showValuesAs(PivotFieldDataDisplayFormat, number, PivotItemPositionType, number)](#showValuesAs-pivotfielddatadisplayformat-number-pivotitempositiontype-number-)| Shows values of data field as different display format when the ShowDataAs calculation is in use. |
| [isHiddenItem(number)](#isHiddenItem-number-)| Gets whether the specific PivotItem is hidden. |
| [hideItem(number, boolean)](#hideItem-number-boolean-)| Sets whether the specific PivotItem in a data field is hidden. |
| [hideItem(string, boolean)](#hideItem-string-boolean-)| Sets whether the specific PivotItem in a data field is hidden. |
| [isHiddenItemDetail(number)](#isHiddenItemDetail-number-)| Gets whether hidding the detail of  the specific PivotItem.. |
| [hideItemDetail(number, boolean)](#hideItemDetail-number-boolean-)| Sets whether the specific PivotItem in a pivot field is hidden detail. |
| [hideDetail(boolean)](#hideDetail-boolean-)| Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field. |
| [addCalculatedItem(string, string)](#addCalculatedItem-string-string-)| Add a calculated formula item to the pivot field. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### pivotItems {#pivotItems--}
Readonly. Gets the pivot items of the pivot field
```javascript
pivotItems : PivotItemCollection;
```
### groupSettings {#groupSettings--}
Readonly. Gets the group settings of the pivot field.
```javascript
groupSettings : PivotFieldGroupSettings;
```
**Remarks**
If this field is not grouped, Null will be returned.
### isCalculatedField {#isCalculatedField--}
Readonly. Indicates whether the specified PivotTable field is calculated field.
```javascript
isCalculatedField : boolean;
```
### isValueFields {#isValueFields--}
Readonly. Indicates whether this field represents values fields.
```javascript
isValueFields : boolean;
```
### baseIndex {#baseIndex--}
Represents the PivotField index in the base PivotFields.
```javascript
baseIndex : number;
```
### position {#position--}
Readonly. Represents the index of [PivotField](../pivotfield/) in the region.
```javascript
position : number;
```
### regionType {#regionType--}
Readonly. Specifies the region of the PivotTable that this field is displayed.
```javascript
regionType : PivotFieldType;
```
### name {#name--}
Represents the name of PivotField.
```javascript
name : string;
```
### displayName {#displayName--}
Represents the PivotField display name.
```javascript
displayName : string;
```
### isAutoSubtotals {#isAutoSubtotals--}
Indicates whether the specified field shows automatic subtotals. Default is true.
```javascript
isAutoSubtotals : boolean;
```
### dragToColumn {#dragToColumn--}
Indicates whether the specified field can be dragged to the column position. The default value is true.
```javascript
dragToColumn : boolean;
```
### dragToHide {#dragToHide--}
Indicates whether the specified field can be dragged to the hide position. The default value is true.
```javascript
dragToHide : boolean;
```
### dragToRow {#dragToRow--}
Indicates whether the specified field can be dragged to the row position. The default value is true.
```javascript
dragToRow : boolean;
```
### dragToPage {#dragToPage--}
Indicates whether the specified field can be dragged to the page position. The default value is true.
```javascript
dragToPage : boolean;
```
### dragToData {#dragToData--}
Indicates whether the specified field can be dragged to the data position. The default value is true.
```javascript
dragToData : boolean;
```
### isMultipleItemSelectionAllowed {#isMultipleItemSelectionAllowed--}
indicates whether the field can have multiple items selected in the page field The default value is false.
```javascript
isMultipleItemSelectionAllowed : boolean;
```
### isRepeatItemLabels {#isRepeatItemLabels--}
Indicates whether repeating labels of the field in the region. The default value is false.
```javascript
isRepeatItemLabels : boolean;
```
### isIncludeNewItemsInFilter {#isIncludeNewItemsInFilter--}
Indicates whether including new items to the field in manual filter. The default value is false.
```javascript
isIncludeNewItemsInFilter : boolean;
```
### isInsertPageBreaksBetweenItems {#isInsertPageBreaksBetweenItems--}
Indicates whether inserting page breaks after each item. The default value is false.
```javascript
isInsertPageBreaksBetweenItems : boolean;
```
### showAllItems {#showAllItems--}
Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with no data The default value is false.
```javascript
showAllItems : boolean;
```
### nonAutoSortDefault {#nonAutoSortDefault--}
Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort.
```javascript
nonAutoSortDefault : boolean;
```
### isAutoSort {#isAutoSort--}
Indicates whether the specified PivotTable field is automatically sorted.
```javascript
isAutoSort : boolean;
```
### isAscendSort {#isAscendSort--}
Indicates whether the specified PivotTable field is autosorted ascending.
```javascript
isAscendSort : boolean;
```
### sortSetting {#sortSetting--}
Readonly. Gets all settings of auto sorting
```javascript
sortSetting : PivotFieldSortSetting;
```
### autoSortField {#autoSortField--}
Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fields.
```javascript
autoSortField : number;
```
### isAutoShow {#isAutoShow--}
Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003.
```javascript
isAutoShow : boolean;
```
### isAscendShow {#isAscendShow--}
Indicates whether the specified PivotTable field is autoshown ascending.
```javascript
isAscendShow : boolean;
```
### autoShowCount {#autoShowCount--}
Represent the number of top or bottom items that are automatically shown in the specified PivotTable field.
```javascript
autoShowCount : number;
```
### autoShowField {#autoShowField--}
Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields.
```javascript
autoShowField : number;
```
### function {#function--}
Represents the function used to summarize the PivotTable data field.
```javascript
function : ConsolidationFunction;
```
### showValuesSetting {#showValuesSetting--}
Readonly. Gets the settings of showing values as when the ShowDataAs calculation is in use.
```javascript
showValuesSetting : PivotShowValuesSetting;
```
### currentPageItem {#currentPageItem--}
Represents the current page item showing for the page field (valid only for page fields).
```javascript
currentPageItem : number;
```
### number {#number--}
Represents the built-in display format of numbers and dates.
```javascript
number : number;
```
### insertBlankRow {#insertBlankRow--}
Indicates whether inserting blank line after each item.
```javascript
insertBlankRow : boolean;
```
### showSubtotalAtTop {#showSubtotalAtTop--}
when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom
```javascript
showSubtotalAtTop : boolean;
```
**Remarks**
Only works when ShowInOutlineForm is true.
### showInOutlineForm {#showInOutlineForm--}
Indicates whether layout this field in outline form on the Pivot Table view
```javascript
showInOutlineForm : boolean;
```
### numberFormat {#numberFormat--}
Represents the custom display format of numbers and dates.
```javascript
numberFormat : string;
```
### items {#items--}
Readonly. Get all labels of pivot items in this field.
```javascript
items : string[];
```
### originalItems {#originalItems--}
Readonly. Get the original base items;
```javascript
originalItems : string[];
```
### itemCount {#itemCount--}
Readonly. Gets the count of the base items in this pivot field.
```javascript
itemCount : number;
```
### showCompact {#showCompact--}
Indicates whether display labels from the next field in the same column on the Pivot Table view
```javascript
showCompact : boolean;
```
### getPivotItems() {#getPivotItems--}
```javascript
getPivotItems() : PivotItemCollection;
```
**Returns**
[PivotItemCollection](../pivotitemcollection/)
### getGroupSettings() {#getGroupSettings--}
```javascript
getGroupSettings() : PivotFieldGroupSettings;
```
**Returns**
[PivotFieldGroupSettings](../pivotfieldgroupsettings/)
**Remarks**
If this field is not grouped, Null will be returned.
### isCalculatedField() {#isCalculatedField--}
```javascript
isCalculatedField() : boolean;
```
### isValueFields() {#isValueFields--}
```javascript
isValueFields() : boolean;
```
### getBaseIndex() {#getBaseIndex--}
```javascript
getBaseIndex() : number;
```
### setBaseIndex(number) {#setBaseIndex-number-}
```javascript
setBaseIndex(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getPosition() {#getPosition--}
```javascript
getPosition() : number;
```
### getRegionType() {#getRegionType--}
```javascript
getRegionType() : PivotFieldType;
```
**Returns**
[PivotFieldType](../pivotfieldtype/)
### getName() {#getName--}
```javascript
getName() : string;
```
### setName(string) {#setName-string-}
```javascript
setName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getDisplayName() {#getDisplayName--}
```javascript
getDisplayName() : string;
```
### setDisplayName(string) {#setDisplayName-string-}
```javascript
setDisplayName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### isAutoSubtotals() {#isAutoSubtotals--}
```javascript
isAutoSubtotals() : boolean;
```
### setIsAutoSubtotals(boolean) {#setIsAutoSubtotals-boolean-}
```javascript
setIsAutoSubtotals(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getDragToColumn() {#getDragToColumn--}
```javascript
getDragToColumn() : boolean;
```
### setDragToColumn(boolean) {#setDragToColumn-boolean-}
```javascript
setDragToColumn(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getDragToHide() {#getDragToHide--}
```javascript
getDragToHide() : boolean;
```
### setDragToHide(boolean) {#setDragToHide-boolean-}
```javascript
setDragToHide(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getDragToRow() {#getDragToRow--}
```javascript
getDragToRow() : boolean;
```
### setDragToRow(boolean) {#setDragToRow-boolean-}
```javascript
setDragToRow(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getDragToPage() {#getDragToPage--}
```javascript
getDragToPage() : boolean;
```
### setDragToPage(boolean) {#setDragToPage-boolean-}
```javascript
setDragToPage(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getDragToData() {#getDragToData--}
```javascript
getDragToData() : boolean;
```
### setDragToData(boolean) {#setDragToData-boolean-}
```javascript
setDragToData(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isMultipleItemSelectionAllowed() {#isMultipleItemSelectionAllowed--}
```javascript
isMultipleItemSelectionAllowed() : boolean;
```
### setIsMultipleItemSelectionAllowed(boolean) {#setIsMultipleItemSelectionAllowed-boolean-}
```javascript
setIsMultipleItemSelectionAllowed(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isRepeatItemLabels() {#isRepeatItemLabels--}
```javascript
isRepeatItemLabels() : boolean;
```
### setIsRepeatItemLabels(boolean) {#setIsRepeatItemLabels-boolean-}
```javascript
setIsRepeatItemLabels(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isIncludeNewItemsInFilter() {#isIncludeNewItemsInFilter--}
```javascript
isIncludeNewItemsInFilter() : boolean;
```
### setIsIncludeNewItemsInFilter(boolean) {#setIsIncludeNewItemsInFilter-boolean-}
```javascript
setIsIncludeNewItemsInFilter(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isInsertPageBreaksBetweenItems() {#isInsertPageBreaksBetweenItems--}
```javascript
isInsertPageBreaksBetweenItems() : boolean;
```
### setIsInsertPageBreaksBetweenItems(boolean) {#setIsInsertPageBreaksBetweenItems-boolean-}
```javascript
setIsInsertPageBreaksBetweenItems(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowAllItems() {#getShowAllItems--}
```javascript
getShowAllItems() : boolean;
```
### setShowAllItems(boolean) {#setShowAllItems-boolean-}
```javascript
setShowAllItems(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getNonAutoSortDefault() {#getNonAutoSortDefault--}
```javascript
getNonAutoSortDefault() : boolean;
```
### setNonAutoSortDefault(boolean) {#setNonAutoSortDefault-boolean-}
```javascript
setNonAutoSortDefault(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isAutoSort() {#isAutoSort--}
```javascript
isAutoSort() : boolean;
```
### setIsAutoSort(boolean) {#setIsAutoSort-boolean-}
```javascript
setIsAutoSort(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isAscendSort() {#isAscendSort--}
```javascript
isAscendSort() : boolean;
```
### setIsAscendSort(boolean) {#setIsAscendSort-boolean-}
```javascript
setIsAscendSort(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getSortSetting() {#getSortSetting--}
```javascript
getSortSetting() : PivotFieldSortSetting;
```
**Returns**
[PivotFieldSortSetting](../pivotfieldsortsetting/)
### getAutoSortField() {#getAutoSortField--}
```javascript
getAutoSortField() : number;
```
### setAutoSortField(number) {#setAutoSortField-number-}
```javascript
setAutoSortField(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isAutoShow() {#isAutoShow--}
```javascript
isAutoShow() : boolean;
```
### setIsAutoShow(boolean) {#setIsAutoShow-boolean-}
```javascript
setIsAutoShow(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isAscendShow() {#isAscendShow--}
```javascript
isAscendShow() : boolean;
```
### setIsAscendShow(boolean) {#setIsAscendShow-boolean-}
```javascript
setIsAscendShow(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAutoShowCount() {#getAutoShowCount--}
```javascript
getAutoShowCount() : number;
```
### setAutoShowCount(number) {#setAutoShowCount-number-}
```javascript
setAutoShowCount(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getAutoShowField() {#getAutoShowField--}
```javascript
getAutoShowField() : number;
```
### setAutoShowField(number) {#setAutoShowField-number-}
```javascript
setAutoShowField(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getFunction() {#getFunction--}
```javascript
getFunction() : ConsolidationFunction;
```
**Returns**
[ConsolidationFunction](../consolidationfunction/)
### setFunction(ConsolidationFunction) {#setFunction-consolidationfunction-}
```javascript
setFunction(value: ConsolidationFunction) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ConsolidationFunction](../consolidationfunction/) | The value to set. |
### getShowValuesSetting() {#getShowValuesSetting--}
```javascript
getShowValuesSetting() : PivotShowValuesSetting;
```
**Returns**
[PivotShowValuesSetting](../pivotshowvaluessetting/)
### getCurrentPageItem() {#getCurrentPageItem--}
```javascript
getCurrentPageItem() : number;
```
### setCurrentPageItem(number) {#setCurrentPageItem-number-}
```javascript
setCurrentPageItem(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getNumber() {#getNumber--}
```javascript
getNumber() : number;
```
### setNumber(number) {#setNumber-number-}
```javascript
setNumber(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getInsertBlankRow() {#getInsertBlankRow--}
```javascript
getInsertBlankRow() : boolean;
```
### setInsertBlankRow(boolean) {#setInsertBlankRow-boolean-}
```javascript
setInsertBlankRow(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowSubtotalAtTop() {#getShowSubtotalAtTop--}
```javascript
getShowSubtotalAtTop() : boolean;
```
**Remarks**
Only works when ShowInOutlineForm is true.
### setShowSubtotalAtTop(boolean) {#setShowSubtotalAtTop-boolean-}
```javascript
setShowSubtotalAtTop(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Only works when ShowInOutlineForm is true.
### getShowInOutlineForm() {#getShowInOutlineForm--}
```javascript
getShowInOutlineForm() : boolean;
```
### setShowInOutlineForm(boolean) {#setShowInOutlineForm-boolean-}
```javascript
setShowInOutlineForm(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### get_NumberFormat() {#get_NumberFormat--}
```javascript
get_NumberFormat() : string;
```
### setNumberFormat(string) {#setNumberFormat-string-}
```javascript
setNumberFormat(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getItems() {#getItems--}
```javascript
getItems() : string[];
```
**Returns**
string[]
### getOriginalItems() {#getOriginalItems--}
```javascript
getOriginalItems() : string[];
```
**Returns**
string[]
### getItemCount() {#getItemCount--}
```javascript
getItemCount() : number;
```
### getShowCompact() {#getShowCompact--}
```javascript
getShowCompact() : boolean;
```
### setShowCompact(boolean) {#setShowCompact-boolean-}
```javascript
setShowCompact(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### initPivotItems() {#initPivotItems--}
Init the pivot items of the pivot field
```javascript
initPivotItems() : void;
```
### groupBy(number, boolean) {#groupBy-number-boolean-}
Automatically group the field with internal
```javascript
groupBy(interval: number, newField: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| interval | number | The internal of group.         /// Automatic value will be assigned if it's zero, |
| newField | boolean | Indicates whether adding a new field to the pivottable. |
### groupBy(Date, Date, PivotGroupByType[], number, boolean) {#groupBy-date-date-pivotgroupbytypearray-number-boolean-}
Group the file by the date group types.
```javascript
groupBy(start: Date, end: Date, groups: PivotGroupByType[], interval: number, firstAsNewField: boolean) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | Date | The start datetime |
| end | Date | The end of datetime |
| groups | [PivotGroupByType](../pivotgroupbytype/)[] | Group types |
| interval | number | The interval |
| firstAsNewField | boolean | Indicates whether adding a new field to the pivottable.         /// Only for the first group item. |
**Returns**
False means this field could not be grouped by date time.
### groupBy(number, number, number, boolean) {#groupBy-number-number-number-boolean-}
Group the file by number.
```javascript
groupBy(start: number, end: number, interval: number, newField: boolean) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | number | The start value |
| end | number | The end of value |
| interval | number | The interval |
| newField | boolean | Indicates whether adding a new field to the pivottable |
**Returns**
False means this field could not be grouped by date time.
### groupBy(CustomPiovtFieldGroupItem[], boolean) {#groupBy-custompiovtfieldgroupitemarray-boolean-}
Custom group the field.
```javascript
groupBy(customGroupItems: CustomPiovtFieldGroupItem[], newField: boolean) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customGroupItems | [CustomPiovtFieldGroupItem](../custompiovtfieldgroupitem/)[] | The custom group items. |
| newField | boolean | Indicates whether adding a new field to the pivottable |
**Returns**
False means this field could not be grouped by date time.
### ungroup() {#ungroup--}
Ungroup the pivot field.
```javascript
ungroup() : void;
```
### getPivotFilterByType(PivotFilterType) {#getPivotFilterByType-pivotfiltertype-}
Gets the pivot filter of the pivot field by type
```javascript
getPivotFilterByType(type: PivotFilterType) : PivotFilter;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [PivotFilterType](../pivotfiltertype/) |  |
**Returns**
[PivotFilter](../pivotfilter/)
### getFilters() {#getFilters--}
Gets all pivot filters of this pivot field.
```javascript
getFilters() : PivotFilter[];
```
**Returns**
[PivotFilter](../pivotfilter/)[]
### clearFilter() {#clearFilter--}
Clears filter setting on this pivot field.
```javascript
clearFilter() : void;
```
### filterTop10(number, PivotFilterType, boolean, number) {#filterTop10-number-pivotfiltertype-boolean-number-}
Filters by values of data pivot field.
```javascript
filterTop10(valueFieldIndex: number, type: PivotFilterType, isTop: boolean, itemCount: number) : PivotFilter;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| valueFieldIndex | number | The index of data field  in the data region. |
| type | [PivotFilterType](../pivotfiltertype/) | The type of filtering data. Only can be Count,Sum and Percent. |
| isTop | boolean | Indicates whether filter from top or bottom |
| itemCount | number | The item count |
**Returns**
[PivotFilter](../pivotfilter/)
### filterByValue(number, PivotFilterType, number, number) {#filterByValue-number-pivotfiltertype-number-number-}
Filters by values of data pivot field.
```javascript
filterByValue(valueFieldIndex: number, type: PivotFilterType, value1: number, value2: number) : PivotFilter;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| valueFieldIndex | number | The index of value field in the value region. |
| type | [PivotFilterType](../pivotfiltertype/) | The type of filtering data. |
| value1 | number | The value of filter condition |
| value2 | number | The upper-bound value of between filter condition |
**Returns**
[PivotFilter](../pivotfilter/)
### filterByLabel(PivotFilterType, string, string) {#filterByLabel-pivotfiltertype-string-string-}
Filters by captions of row or column pivot field.
```javascript
filterByLabel(type: PivotFilterType, label1: string, label2: string) : PivotFilter;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [PivotFilterType](../pivotfiltertype/) | The type of filtering data. |
| label1 | string | The label of filter condition |
| label2 | string | The upper-bound label of between filter condition |
**Returns**
[PivotFilter](../pivotfilter/)
### filterByDate(PivotFilterType, Date, Date) {#filterByDate-pivotfiltertype-date-date-}
Filters by date setting of row or column pivot field.
```javascript
filterByDate(type: PivotFilterType, dateTime1: Date, dateTime2: Date) : PivotFilter;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [PivotFilterType](../pivotfiltertype/) | The type of filtering data. |
| dateTime1 | Date | The date label of filter condition |
| dateTime2 | Date | The upper-bound date label of between filter condition |
**Returns**
[PivotFilter](../pivotfilter/)
### getFormula() {#getFormula--}
Gets formula of the calculated field .
```javascript
getFormula() : string;
```
### setSubtotals(PivotFieldSubtotalType, boolean) {#setSubtotals-pivotfieldsubtotaltype-boolean-}
Sets whether the specified field shows that subtotals.
```javascript
setSubtotals(subtotalType: PivotFieldSubtotalType, shown: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) | subtotals type. |
| shown | boolean | whether the specified field shows that subtotals. |
### getSubtotals(PivotFieldSubtotalType) {#getSubtotals-pivotfieldsubtotaltype-}
Indicates whether showing specified subtotal.
```javascript
getSubtotals(subtotalType: PivotFieldSubtotalType) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) | subtotal type. |
**Returns**
Returns whether showing specified subtotal.
### sortBy(SortOrder, number) {#sortBy-sortorder-number-}
Sorts this pivot field.
```javascript
sortBy(sortType: SortOrder, fieldSortedBy: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sortType | [SortOrder](../sortorder/) | The type of sorting this field. |
| fieldSortedBy | number | The index of pivot field sorted by.         /// -1 means sorting by data labels of this field, others mean the index of data field sorted by. |
### sortBy(SortOrder, number, PivotLineType, string) {#sortBy-sortorder-number-pivotlinetype-string-}
Sorts this pivot field.
```javascript
sortBy(sortType: SortOrder, fieldSortedBy: number, dataType: PivotLineType, cellName: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sortType | [SortOrder](../sortorder/) | The type of sorting this field. |
| fieldSortedBy | number | The index of pivot field sorted by.         /// -1 means sorting by data labels of this field, others mean the index of data field sorted by. |
| dataType | [PivotLineType](../pivotlinetype/) | The type of data sorted by. |
| cellName | string | Sort by values in the row or column |
### showValuesAs(PivotFieldDataDisplayFormat, number, PivotItemPositionType, number) {#showValuesAs-pivotfielddatadisplayformat-number-pivotitempositiontype-number-}
Shows values of data field as different display format when the ShowDataAs calculation is in use.
```javascript
showValuesAs(displayFormat: PivotFieldDataDisplayFormat, baseField: number, baseItemPositionType: PivotItemPositionType, baseItem: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| displayFormat | [PivotFieldDataDisplayFormat](../pivotfielddatadisplayformat/) | The data display format type. |
| baseField | number | The index to the field which ShowDataAs calculation bases on. |
| baseItemPositionType | [PivotItemPositionType](../pivotitempositiontype/) | The position type of base iteam. |
| baseItem | number | The index to the base item which ShowDataAs calculation bases on.         /// Only works when baseItemPositionType is custom. |
**Remarks**
Only for data field.
### isHiddenItem(number) {#isHiddenItem-number-}
Gets whether the specific PivotItem is hidden.
```javascript
isHiddenItem(index: number) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index of the pivotItem in the pivotField. |
**Returns**
whether the specific PivotItem is hidden
### hideItem(number, boolean) {#hideItem-number-boolean-}
Sets whether the specific PivotItem in a data field is hidden.
```javascript
hideItem(index: number, isHidden: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | the index of the pivotItem in the pivotField. |
| isHidden | boolean | whether the specific PivotItem is hidden |
### hideItem(string, boolean) {#hideItem-string-boolean-}
Sets whether the specific PivotItem in a data field is hidden.
```javascript
hideItem(itemValue: string, isHidden: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| itemValue | string | the value of the pivotItem in the pivotField. |
| isHidden | boolean | whether the specific PivotItem is hidden |
### isHiddenItemDetail(number) {#isHiddenItemDetail-number-}
Gets whether hidding the detail of  the specific PivotItem..
```javascript
isHiddenItemDetail(index: number) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index of the pivotItem in the pivotField. |
**Returns**
whether the specific PivotItem is hidden detail
### hideItemDetail(number, boolean) {#hideItemDetail-number-boolean-}
Sets whether the specific PivotItem in a pivot field is hidden detail.
```javascript
hideItemDetail(index: number, isHiddenDetail: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | the index of the pivotItem in the pivotField. |
| isHiddenDetail | boolean | whether the specific PivotItem is hidden |
### hideDetail(boolean) {#hideDetail-boolean-}
Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field.
```javascript
hideDetail(isHiddenDetail: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isHiddenDetail | boolean | Whether hide the detail of the pivot field. |
### addCalculatedItem(string, string) {#addCalculatedItem-string-string-}
Add a calculated formula item to the pivot field.
```javascript
addCalculatedItem(name: string, formula: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The item's name. |
| formula | string | The formula of pivot item. |
**Remarks**
Only supports to add calculated item to Row/Column field.
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
