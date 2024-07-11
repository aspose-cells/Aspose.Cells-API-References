---
title: PivotField
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a field in a PivotTable report.
type: docs
url: /nodejs-cpp/pivotfield/
---

## PivotField class

Represents a field in a PivotTable report.

```javascript
class PivotField;
```


## Methods

| Method | Description |
| --- | --- |
| [getPivotItems()](#getPivotItems--)| Gets the pivot items of the pivot field |
| [getGroupSettings()](#getGroupSettings--)| Gets the group settings of the pivot field. |
| [isCalculatedField()](#isCalculatedField--)| Indicates whether the specified PivotTable field is calculated field. |
| [getBaseIndex()](#getBaseIndex--)| Represents the PivotField index in the base PivotFields. |
| [setBaseIndex(number)](#setBaseIndex-number-)| Represents the PivotField index in the base PivotFields. |
| [getPosition()](#getPosition--)| Represents the index of [PivotField](./pivotfield/) in the region. |
| [getName()](#getName--)| Represents the name of PivotField. |
| [setName(string)](#setName-string-)| Represents the name of PivotField. |
| [getDisplayName()](#getDisplayName--)| Represents the PivotField display name. |
| [setDisplayName(string)](#setDisplayName-string-)| Represents the PivotField display name. |
| [isAutoSubtotals()](#isAutoSubtotals--)| Indicates whether the specified field shows automatic subtotals. Default is true. |
| [setIsAutoSubtotals(boolean)](#setIsAutoSubtotals-boolean-)| Indicates whether the specified field shows automatic subtotals. Default is true. |
| [getDragToColumn()](#getDragToColumn--)| Indicates whether the specified field can be dragged to the column position. The default value is true. |
| [setDragToColumn(boolean)](#setDragToColumn-boolean-)| Indicates whether the specified field can be dragged to the column position. The default value is true. |
| [getDragToHide()](#getDragToHide--)| Indicates whether the specified field can be dragged to the hide position. The default value is true. |
| [setDragToHide(boolean)](#setDragToHide-boolean-)| Indicates whether the specified field can be dragged to the hide position. The default value is true. |
| [getDragToRow()](#getDragToRow--)| Indicates whether the specified field can be dragged to the row position. The default value is true. |
| [setDragToRow(boolean)](#setDragToRow-boolean-)| Indicates whether the specified field can be dragged to the row position. The default value is true. |
| [getDragToPage()](#getDragToPage--)| Indicates whether the specified field can be dragged to the page position. The default value is true. |
| [setDragToPage(boolean)](#setDragToPage-boolean-)| Indicates whether the specified field can be dragged to the page position. The default value is true. |
| [getDragToData()](#getDragToData--)| Indicates whether the specified field can be dragged to the data position. The default value is true. |
| [setDragToData(boolean)](#setDragToData-boolean-)| Indicates whether the specified field can be dragged to the data position. The default value is true. |
| [isMultipleItemSelectionAllowed()](#isMultipleItemSelectionAllowed--)| indicates whether the field can have multiple items selected in the page field The default value is false. |
| [setIsMultipleItemSelectionAllowed(boolean)](#setIsMultipleItemSelectionAllowed-boolean-)| indicates whether the field can have multiple items selected in the page field The default value is false. |
| [isRepeatItemLabels()](#isRepeatItemLabels--)| Indicates whether repeating labels of the field in the region. The default value is false. |
| [setIsRepeatItemLabels(boolean)](#setIsRepeatItemLabels-boolean-)| Indicates whether repeating labels of the field in the region. The default value is false. |
| [isIncludeNewItemsInFilter()](#isIncludeNewItemsInFilter--)| Indicates whether including new items to the field in manual filter. The default value is false. |
| [setIsIncludeNewItemsInFilter(boolean)](#setIsIncludeNewItemsInFilter-boolean-)| Indicates whether including new items to the field in manual filter. The default value is false. |
| [isInsertPageBreaksBetweenItems()](#isInsertPageBreaksBetweenItems--)| Indicates whether inserting page breaks after each item. The default value is false. |
| [setIsInsertPageBreaksBetweenItems(boolean)](#setIsInsertPageBreaksBetweenItems-boolean-)| Indicates whether inserting page breaks after each item. The default value is false. |
| [getShowAllItems()](#getShowAllItems--)| Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with no data The default value is false. |
| [setShowAllItems(boolean)](#setShowAllItems-boolean-)| Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with no data The default value is false. |
| [getNonAutoSortDefault()](#getNonAutoSortDefault--)| Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort. |
| [setNonAutoSortDefault(boolean)](#setNonAutoSortDefault-boolean-)| Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort. |
| [isAutoSort()](#isAutoSort--)| Indicates whether the specified PivotTable field is automatically sorted. |
| [setIsAutoSort(boolean)](#setIsAutoSort-boolean-)| Indicates whether the specified PivotTable field is automatically sorted. |
| [isAscendSort()](#isAscendSort--)| Indicates whether the specified PivotTable field is autosorted ascending. |
| [setIsAscendSort(boolean)](#setIsAscendSort-boolean-)| Indicates whether the specified PivotTable field is autosorted ascending. |
| [getAutoSortField()](#getAutoSortField--)| Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fields. |
| [setAutoSortField(number)](#setAutoSortField-number-)| Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fields. |
| [isAutoShow()](#isAutoShow--)| Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003. |
| [setIsAutoShow(boolean)](#setIsAutoShow-boolean-)| Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003. |
| [isAscendShow()](#isAscendShow--)| Indicates whether the specified PivotTable field is autoshown ascending. |
| [setIsAscendShow(boolean)](#setIsAscendShow-boolean-)| Indicates whether the specified PivotTable field is autoshown ascending. |
| [getAutoShowCount()](#getAutoShowCount--)| Represent the number of top or bottom items that are automatically shown in the specified PivotTable field. |
| [setAutoShowCount(number)](#setAutoShowCount-number-)| Represent the number of top or bottom items that are automatically shown in the specified PivotTable field. |
| [getAutoShowField()](#getAutoShowField--)| Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields. |
| [setAutoShowField(number)](#setAutoShowField-number-)| Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields. |
| [getFunction()](#getFunction--)| Represents the function used to summarize the PivotTable data field. |
| [setFunction(ConsolidationFunction)](#setFunction-consolidationfunction-)| Represents the function used to summarize the PivotTable data field. |
| [getShowValuesSetting()](#getShowValuesSetting--)| Gets the settings of showing values as when the ShowDataAs calculation is in use. |
| [getDataDisplayFormat()](#getDataDisplayFormat--)| Represents how to display the values in a data field of the pivot report. |
| [setDataDisplayFormat(PivotFieldDataDisplayFormat)](#setDataDisplayFormat-pivotfielddatadisplayformat-)| Represents how to display the values in a data field of the pivot report. |
| [getBaseFieldIndex()](#getBaseFieldIndex--)| Represents the base field for a custom calculation when the ShowDataAs calculation is in use. |
| [setBaseFieldIndex(number)](#setBaseFieldIndex-number-)| Represents the base field for a custom calculation when the ShowDataAs calculation is in use. |
| [getBaseItemPosition()](#getBaseItemPosition--)| Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. |
| [setBaseItemPosition(PivotItemPosition)](#setBaseItemPosition-pivotitemposition-)| Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. |
| [getBaseItemIndex()](#getBaseItemIndex--)| Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. |
| [setBaseItemIndex(number)](#setBaseItemIndex-number-)| Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. |
| [getCurrentPageItem()](#getCurrentPageItem--)| Represents the current page item showing for the page field (valid only for page fields). |
| [setCurrentPageItem(number)](#setCurrentPageItem-number-)| Represents the current page item showing for the page field (valid only for page fields). |
| [getNumber()](#getNumber--)| Represents the built-in display format of numbers and dates. |
| [setNumber(number)](#setNumber-number-)| Represents the built-in display format of numbers and dates. |
| [getInsertBlankRow()](#getInsertBlankRow--)| Indicates whether inserting blank line after each item. |
| [setInsertBlankRow(boolean)](#setInsertBlankRow-boolean-)| Indicates whether inserting blank line after each item. |
| [getShowSubtotalAtTop()](#getShowSubtotalAtTop--)| when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom |
| [setShowSubtotalAtTop(boolean)](#setShowSubtotalAtTop-boolean-)| when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom |
| [getShowInOutlineForm()](#getShowInOutlineForm--)| Indicates whether layout this field in outline form on the Pivot Table view |
| [setShowInOutlineForm(boolean)](#setShowInOutlineForm-boolean-)| Indicates whether layout this field in outline form on the Pivot Table view |
| [get_NumberFormat()](#get_NumberFormat--)| Represents the custom display format of numbers and dates. |
| [setNumberFormat(string)](#setNumberFormat-string-)| Represents the custom display format of numbers and dates. |
| [getItems()](#getItems--)| Get all labels of pivot items in this field. |
| [getOriginalItems()](#getOriginalItems--)| Get the original base items; |
| [getItemCount()](#getItemCount--)| Gets the count of the base items in this pivot field. |
| [getShowCompact()](#getShowCompact--)| Indicates whether display labels from the next field in the same column on the Pivot Table view |
| [setShowCompact(boolean)](#setShowCompact-boolean-)| Indicates whether display labels from the next field in the same column on the Pivot Table view |
| [getPivotFilterByType(PivotFilterType)](#getPivotFilterByType-pivotfiltertype-)| Gets the pivot filter of the pivot field by type |
| [getFilters()](#getFilters--)| Gets all pivot filters of this pivot field. |
| [initPivotItems()](#initPivotItems--)| Init the pivot items of the pivot field |
| [groupBy(number, boolean)](#groupBy-number-boolean-)| Automatically group the field with internal |
| [groupBy(Date, Date, PivotGroupByType[], number, boolean)](#groupBy-date-date-pivotgroupbytype[]-number-boolean-)| Group the file by the date group types. |
| [groupBy(number, number, number, boolean)](#groupBy-number-number-number-boolean-)| Group the file by number. |
| [groupBy(CustomPiovtFieldGroupItem[], boolean)](#groupBy-custompiovtfieldgroupitem[]-boolean-)| Custom group the field. |
| [ungroup()](#ungroup--)| Ungroup the pivot field. |
| [getCalculatedFieldFormula()](#getCalculatedFieldFormula--)| Get the formula string of the specified calculated field . |
| [setSubtotals(PivotFieldSubtotalType, boolean)](#setSubtotals-pivotfieldsubtotaltype-boolean-)| Sets whether the specified field shows that subtotals. |
| [getSubtotals(PivotFieldSubtotalType)](#getSubtotals-pivotfieldsubtotaltype-)| Indicates whether showing specified subtotal. |
| [showValuesAs(PivotFieldDataDisplayFormat, number, PivotItemPositionType, number)](#showValuesAs-pivotfielddatadisplayformat-number-pivotitempositiontype-number-)| Shows values of data field as different display format when the ShowDataAs calculation is in use. |
| [isHiddenItem(number)](#isHiddenItem-number-)| Gets whether the specific PivotItem is hidden. |
| [hideItem(number, boolean)](#hideItem-number-boolean-)| Sets whether the specific PivotItem in a data field is hidden. |
| [hideItem(string, boolean)](#hideItem-string-boolean-)| Sets whether the specific PivotItem in a data field is hidden. |
| [isHiddenItemDetail(number)](#isHiddenItemDetail-number-)| Gets whether hidding the detail of  the specific PivotItem.. |
| [hideItemDetail(number, boolean)](#hideItemDetail-number-boolean-)| Sets whether the specific PivotItem in a pivot field is hidden detail. |
| [hideDetail(boolean)](#hideDetail-boolean-)| Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field. |
| [addCalculatedItem(string, string)](#addCalculatedItem-string-string-)| Add a calculated formula item to the pivot field. |


### getPivotItems() {#getPivotItems--}

Gets the pivot items of the pivot field

```javascript
getPivotItems() : PivotItemCollection;
```


**Returns**

[PivotItemCollection](./pivotitemcollection/)

### getGroupSettings() {#getGroupSettings--}

Gets the group settings of the pivot field.

```javascript
getGroupSettings() : PivotFieldGroupSettings;
```


**Returns**

[PivotFieldGroupSettings](./pivotfieldgroupsettings/)

**Remarks**

If this field is not grouped, Null will be returned.

### isCalculatedField() {#isCalculatedField--}

Indicates whether the specified PivotTable field is calculated field.

```javascript
isCalculatedField() : boolean;
```


### getBaseIndex() {#getBaseIndex--}

Represents the PivotField index in the base PivotFields.

```javascript
getBaseIndex() : number;
```


### setBaseIndex(number) {#setBaseIndex-number-}

Represents the PivotField index in the base PivotFields.

```javascript
setBaseIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getPosition() {#getPosition--}

Represents the index of [PivotField](./pivotfield/) in the region.

```javascript
getPosition() : number;
```


### getName() {#getName--}

Represents the name of PivotField.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

Represents the name of PivotField.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getDisplayName() {#getDisplayName--}

Represents the PivotField display name.

```javascript
getDisplayName() : string;
```


### setDisplayName(string) {#setDisplayName-string-}

Represents the PivotField display name.

```javascript
setDisplayName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isAutoSubtotals() {#isAutoSubtotals--}

Indicates whether the specified field shows automatic subtotals. Default is true.

```javascript
isAutoSubtotals() : boolean;
```


### setIsAutoSubtotals(boolean) {#setIsAutoSubtotals-boolean-}

Indicates whether the specified field shows automatic subtotals. Default is true.

```javascript
setIsAutoSubtotals(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDragToColumn() {#getDragToColumn--}

Indicates whether the specified field can be dragged to the column position. The default value is true.

```javascript
getDragToColumn() : boolean;
```


### setDragToColumn(boolean) {#setDragToColumn-boolean-}

Indicates whether the specified field can be dragged to the column position. The default value is true.

```javascript
setDragToColumn(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDragToHide() {#getDragToHide--}

Indicates whether the specified field can be dragged to the hide position. The default value is true.

```javascript
getDragToHide() : boolean;
```


### setDragToHide(boolean) {#setDragToHide-boolean-}

Indicates whether the specified field can be dragged to the hide position. The default value is true.

```javascript
setDragToHide(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDragToRow() {#getDragToRow--}

Indicates whether the specified field can be dragged to the row position. The default value is true.

```javascript
getDragToRow() : boolean;
```


### setDragToRow(boolean) {#setDragToRow-boolean-}

Indicates whether the specified field can be dragged to the row position. The default value is true.

```javascript
setDragToRow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDragToPage() {#getDragToPage--}

Indicates whether the specified field can be dragged to the page position. The default value is true.

```javascript
getDragToPage() : boolean;
```


### setDragToPage(boolean) {#setDragToPage-boolean-}

Indicates whether the specified field can be dragged to the page position. The default value is true.

```javascript
setDragToPage(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDragToData() {#getDragToData--}

Indicates whether the specified field can be dragged to the data position. The default value is true.

```javascript
getDragToData() : boolean;
```


### setDragToData(boolean) {#setDragToData-boolean-}

Indicates whether the specified field can be dragged to the data position. The default value is true.

```javascript
setDragToData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isMultipleItemSelectionAllowed() {#isMultipleItemSelectionAllowed--}

indicates whether the field can have multiple items selected in the page field The default value is false.

```javascript
isMultipleItemSelectionAllowed() : boolean;
```


### setIsMultipleItemSelectionAllowed(boolean) {#setIsMultipleItemSelectionAllowed-boolean-}

indicates whether the field can have multiple items selected in the page field The default value is false.

```javascript
setIsMultipleItemSelectionAllowed(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isRepeatItemLabels() {#isRepeatItemLabels--}

Indicates whether repeating labels of the field in the region. The default value is false.

```javascript
isRepeatItemLabels() : boolean;
```


### setIsRepeatItemLabels(boolean) {#setIsRepeatItemLabels-boolean-}

Indicates whether repeating labels of the field in the region. The default value is false.

```javascript
setIsRepeatItemLabels(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isIncludeNewItemsInFilter() {#isIncludeNewItemsInFilter--}

Indicates whether including new items to the field in manual filter. The default value is false.

```javascript
isIncludeNewItemsInFilter() : boolean;
```


### setIsIncludeNewItemsInFilter(boolean) {#setIsIncludeNewItemsInFilter-boolean-}

Indicates whether including new items to the field in manual filter. The default value is false.

```javascript
setIsIncludeNewItemsInFilter(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isInsertPageBreaksBetweenItems() {#isInsertPageBreaksBetweenItems--}

Indicates whether inserting page breaks after each item. The default value is false.

```javascript
isInsertPageBreaksBetweenItems() : boolean;
```


### setIsInsertPageBreaksBetweenItems(boolean) {#setIsInsertPageBreaksBetweenItems-boolean-}

Indicates whether inserting page breaks after each item. The default value is false.

```javascript
setIsInsertPageBreaksBetweenItems(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowAllItems() {#getShowAllItems--}

Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with no data The default value is false.

```javascript
getShowAllItems() : boolean;
```


### setShowAllItems(boolean) {#setShowAllItems-boolean-}

Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with no data The default value is false.

```javascript
setShowAllItems(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getNonAutoSortDefault() {#getNonAutoSortDefault--}

Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort.

```javascript
getNonAutoSortDefault() : boolean;
```


### setNonAutoSortDefault(boolean) {#setNonAutoSortDefault-boolean-}

Indicates whether a sort operation that will be applied to this pivot field is an autosort operation or a simple data sort.

```javascript
setNonAutoSortDefault(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isAutoSort() {#isAutoSort--}

Indicates whether the specified PivotTable field is automatically sorted.

```javascript
isAutoSort() : boolean;
```


### setIsAutoSort(boolean) {#setIsAutoSort-boolean-}

Indicates whether the specified PivotTable field is automatically sorted.

```javascript
setIsAutoSort(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isAscendSort() {#isAscendSort--}

Indicates whether the specified PivotTable field is autosorted ascending.

```javascript
isAscendSort() : boolean;
```


### setIsAscendSort(boolean) {#setIsAscendSort-boolean-}

Indicates whether the specified PivotTable field is autosorted ascending.

```javascript
setIsAscendSort(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAutoSortField() {#getAutoSortField--}

Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fields.

```javascript
getAutoSortField() : number;
```


### setAutoSortField(number) {#setAutoSortField-number-}

Represents the index of field which is auto sorted. -1 means PivotField itself,others means the position of the data fields.

```javascript
setAutoSortField(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### isAutoShow() {#isAutoShow--}

Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003.

```javascript
isAutoShow() : boolean;
```


### setIsAutoShow(boolean) {#setIsAutoShow-boolean-}

Indicates whether the specified PivotTable field is automatically shown,only valid for excel 2003.

```javascript
setIsAutoShow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isAscendShow() {#isAscendShow--}

Indicates whether the specified PivotTable field is autoshown ascending.

```javascript
isAscendShow() : boolean;
```


### setIsAscendShow(boolean) {#setIsAscendShow-boolean-}

Indicates whether the specified PivotTable field is autoshown ascending.

```javascript
setIsAscendShow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAutoShowCount() {#getAutoShowCount--}

Represent the number of top or bottom items that are automatically shown in the specified PivotTable field.

```javascript
getAutoShowCount() : number;
```


### setAutoShowCount(number) {#setAutoShowCount-number-}

Represent the number of top or bottom items that are automatically shown in the specified PivotTable field.

```javascript
setAutoShowCount(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getAutoShowField() {#getAutoShowField--}

Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields.

```javascript
getAutoShowField() : number;
```


### setAutoShowField(number) {#setAutoShowField-number-}

Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields.

```javascript
setAutoShowField(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getFunction() {#getFunction--}

Represents the function used to summarize the PivotTable data field.

```javascript
getFunction() : ConsolidationFunction;
```


**Returns**

[ConsolidationFunction](./consolidationfunction/)

### setFunction(ConsolidationFunction) {#setFunction-consolidationfunction-}

Represents the function used to summarize the PivotTable data field.

```javascript
setFunction(value: ConsolidationFunction) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ConsolidationFunction](./consolidationfunction/) | The value to set. |

### getShowValuesSetting() {#getShowValuesSetting--}

Gets the settings of showing values as when the ShowDataAs calculation is in use.

```javascript
getShowValuesSetting() : PivotShowValuesSetting;
```


**Returns**

[PivotShowValuesSetting](./pivotshowvaluessetting/)

### getDataDisplayFormat() {#getDataDisplayFormat--}

Represents how to display the values in a data field of the pivot report.

```javascript
getDataDisplayFormat() : PivotFieldDataDisplayFormat;
```


**Returns**

[PivotFieldDataDisplayFormat](./pivotfielddatadisplayformat/)

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.CalculationType property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### setDataDisplayFormat(PivotFieldDataDisplayFormat) {#setDataDisplayFormat-pivotfielddatadisplayformat-}

Represents how to display the values in a data field of the pivot report.

```javascript
setDataDisplayFormat(value: PivotFieldDataDisplayFormat) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotFieldDataDisplayFormat](./pivotfielddatadisplayformat/) | The value to set. |

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.CalculationType property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### getBaseFieldIndex() {#getBaseFieldIndex--}

Represents the base field for a custom calculation when the ShowDataAs calculation is in use.

```javascript
getBaseFieldIndex() : number;
```


**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.BaseFieldIndex property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### setBaseFieldIndex(number) {#setBaseFieldIndex-number-}

Represents the base field for a custom calculation when the ShowDataAs calculation is in use.

```javascript
setBaseFieldIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.BaseFieldIndex property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### getBaseItemPosition() {#getBaseItemPosition--}

Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.

```javascript
getBaseItemPosition() : PivotItemPosition;
```


**Returns**

[PivotItemPosition](./pivotitemposition/)

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.BaseItemType property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### setBaseItemPosition(PivotItemPosition) {#setBaseItemPosition-pivotitemposition-}

Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.

```javascript
setBaseItemPosition(value: PivotItemPosition) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotItemPosition](./pivotitemposition/) | The value to set. |

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.BaseItemType property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### getBaseItemIndex() {#getBaseItemIndex--}

Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields.

```javascript
getBaseItemIndex() : number;
```


**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.BaseItemIndex property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### setBaseItemIndex(number) {#setBaseItemIndex-number-}

Represents the item in the base field for a custom calculation when the ShowDataAs calculation is in use. Valid only for data fields.

```javascript
setBaseItemIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotField.PivotShowValuesSetting.BaseItemIndex property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### getCurrentPageItem() {#getCurrentPageItem--}

Represents the current page item showing for the page field (valid only for page fields).

```javascript
getCurrentPageItem() : number;
```


### setCurrentPageItem(number) {#setCurrentPageItem-number-}

Represents the current page item showing for the page field (valid only for page fields).

```javascript
setCurrentPageItem(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getNumber() {#getNumber--}

Represents the built-in display format of numbers and dates.

```javascript
getNumber() : number;
```


### setNumber(number) {#setNumber-number-}

Represents the built-in display format of numbers and dates.

```javascript
setNumber(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getInsertBlankRow() {#getInsertBlankRow--}

Indicates whether inserting blank line after each item.

```javascript
getInsertBlankRow() : boolean;
```


### setInsertBlankRow(boolean) {#setInsertBlankRow-boolean-}

Indicates whether inserting blank line after each item.

```javascript
setInsertBlankRow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowSubtotalAtTop() {#getShowSubtotalAtTop--}

when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom

```javascript
getShowSubtotalAtTop() : boolean;
```


**Remarks**

Only works when ShowInOutlineForm is true.

### setShowSubtotalAtTop(boolean) {#setShowSubtotalAtTop-boolean-}

when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom

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

Indicates whether layout this field in outline form on the Pivot Table view

```javascript
getShowInOutlineForm() : boolean;
```


### setShowInOutlineForm(boolean) {#setShowInOutlineForm-boolean-}

Indicates whether layout this field in outline form on the Pivot Table view

```javascript
setShowInOutlineForm(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### get_NumberFormat() {#get_NumberFormat--}

Represents the custom display format of numbers and dates.

```javascript
get_NumberFormat() : string;
```


### setNumberFormat(string) {#setNumberFormat-string-}

Represents the custom display format of numbers and dates.

```javascript
setNumberFormat(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getItems() {#getItems--}

Get all labels of pivot items in this field.

```javascript
getItems() : string[];
```


**Returns**

string[]

### getOriginalItems() {#getOriginalItems--}

Get the original base items;

```javascript
getOriginalItems() : string[];
```


**Returns**

string[]

### getItemCount() {#getItemCount--}

Gets the count of the base items in this pivot field.

```javascript
getItemCount() : number;
```


### getShowCompact() {#getShowCompact--}

Indicates whether display labels from the next field in the same column on the Pivot Table view

```javascript
getShowCompact() : boolean;
```


### setShowCompact(boolean) {#setShowCompact-boolean-}

Indicates whether display labels from the next field in the same column on the Pivot Table view

```javascript
setShowCompact(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPivotFilterByType(PivotFilterType) {#getPivotFilterByType-pivotfiltertype-}

Gets the pivot filter of the pivot field by type

```javascript
getPivotFilterByType(type: PivotFilterType) : PivotFilter;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [PivotFilterType](./pivotfiltertype/) |  |

**Returns**

[PivotFilter](./pivotfilter/)

### getFilters() {#getFilters--}

Gets all pivot filters of this pivot field.

```javascript
getFilters() : PivotFilter[];
```


**Returns**

[PivotFilter](./pivotfilter/)[]

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

### groupBy(Date, Date, PivotGroupByType[], number, boolean) {#groupBy-date-date-pivotgroupbytype[]-number-boolean-}

Group the file by the date group types.

```javascript
groupBy(start: Date, end: Date, groups: PivotGroupByType[], interval: number, firstAsNewField: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | Date | The start datetime |
| end | Date | The end of datetime |
| groups | [PivotGroupByType](./pivotgroupbytype/)[] | Group types |
| interval | number | The interval |
| firstAsNewField | boolean | Indicates whether adding a new field to the pivottable.         /// Only for the first group item. |

### groupBy(number, number, number, boolean) {#groupBy-number-number-number-boolean-}

Group the file by number.

```javascript
groupBy(start: number, end: number, interval: number, newField: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | number | The start value |
| end | number | The end of value |
| interval | number | The interval |
| newField | boolean | Indicates whether adding a new field to the pivottable |

### groupBy(CustomPiovtFieldGroupItem[], boolean) {#groupBy-custompiovtfieldgroupitem[]-boolean-}

Custom group the field.

```javascript
groupBy(customGroupItems: CustomPiovtFieldGroupItem[], newField: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| customGroupItems | [CustomPiovtFieldGroupItem](./custompiovtfieldgroupitem/)[] | The custom group items. |
| newField | boolean | Indicates whether adding a new field to the pivottable |

### ungroup() {#ungroup--}

Ungroup the pivot field.

```javascript
ungroup() : void;
```


### getCalculatedFieldFormula() {#getCalculatedFieldFormula--}

Get the formula string of the specified calculated field .

```javascript
getCalculatedFieldFormula() : string;
```


### setSubtotals(PivotFieldSubtotalType, boolean) {#setSubtotals-pivotfieldsubtotaltype-boolean-}

Sets whether the specified field shows that subtotals.

```javascript
setSubtotals(subtotalType: PivotFieldSubtotalType, shown: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | [PivotFieldSubtotalType](./pivotfieldsubtotaltype/) | subtotals type. |
| shown | boolean | whether the specified field shows that subtotals. |

### getSubtotals(PivotFieldSubtotalType) {#getSubtotals-pivotfieldsubtotaltype-}

Indicates whether showing specified subtotal.

```javascript
getSubtotals(subtotalType: PivotFieldSubtotalType) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | [PivotFieldSubtotalType](./pivotfieldsubtotaltype/) | subtotal type. |

**Returns**

Returns whether showing specified subtotal.

### showValuesAs(PivotFieldDataDisplayFormat, number, PivotItemPositionType, number) {#showValuesAs-pivotfielddatadisplayformat-number-pivotitempositiontype-number-}

Shows values of data field as different display format when the ShowDataAs calculation is in use.

```javascript
showValuesAs(displayFormat: PivotFieldDataDisplayFormat, baseField: number, baseItemPositionType: PivotItemPositionType, baseItem: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| displayFormat | [PivotFieldDataDisplayFormat](./pivotfielddatadisplayformat/) | The data display format type. |
| baseField | number | The index to the field which ShowDataAs calculation bases on. |
| baseItemPositionType | [PivotItemPositionType](./pivotitempositiontype/) | The position type of base iteam. |
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


