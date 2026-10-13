---
title: PivotFieldSortSetting
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the setting for sorting pivot fields.
type: docs
url: /nodejs-cpp/pivotfieldsortsetting/
---

## PivotFieldSortSetting class

Represents the setting for sorting pivot fields.

```javascript
class PivotFieldSortSetting;
```


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [sortType](#sortType--)| SortOrder | Represents the [SortOrder](../sortorder/). |
| [isSortByLabels](#isSortByLabels--)| boolean | Readonly. Indicates whether to sort the field by itself or data field. |
| [fieldIndex](#fieldIndex--)| number | Represents the index of the field sorted by. -1 means sorting the PivotField by the labels,others means sorting by the data field. |
| [sortBy](#sortBy--)| number | Represents the index of the field sorted by. A value of -1 indicates sorting by the pivot item's own values. When greater than or equal to zero, it represents the index of data field in the data region. |
| [lineTypeSortedBy](#lineTypeSortedBy--)| PivotLineType | Readonly. The pivot line type sorted by. |
| [isSimpleSort](#isSimpleSort--)| boolean | Indicates whether a simple data sort operation will be applied. |
| [cell](#cell--)| string | Readonly. Sorts by the values in which row or column. |

## Methods

| Method | Description |
| --- | --- |
| [getSortType()](#getSortType--)| <b>@deprecated.</b> Please use the 'sortType' property instead. Represents the [SortOrder](../sortorder/). |
| [setSortType(SortOrder)](#setSortType-sortorder-)| <b>@deprecated.</b> Please use the 'sortType' property instead. Represents the [SortOrder](../sortorder/). |
| [isSortByLabels()](#isSortByLabels--)| <b>@deprecated.</b> Please use the 'isSortByLabels' property instead. Indicates whether to sort the field by itself or data field. |
| [getFieldIndex()](#getFieldIndex--)| <b>@deprecated.</b> Please use the 'fieldIndex' property instead. Represents the index of the field sorted by. -1 means sorting the PivotField by the labels,others means sorting by the data field. |
| [setFieldIndex(number)](#setFieldIndex-number-)| <b>@deprecated.</b> Please use the 'fieldIndex' property instead. Represents the index of the field sorted by. -1 means sorting the PivotField by the labels,others means sorting by the data field. |
| [getSortBy()](#getSortBy--)| <b>@deprecated.</b> Please use the 'sortBy' property instead. Represents the index of the field sorted by. A value of -1 indicates sorting by the pivot item's own values. When greater than or equal to zero, it represents the index of data field in the data region. |
| [setSortBy(number)](#setSortBy-number-)| <b>@deprecated.</b> Please use the 'sortBy' property instead. Represents the index of the field sorted by. A value of -1 indicates sorting by the pivot item's own values. When greater than or equal to zero, it represents the index of data field in the data region. |
| [getLineTypeSortedBy()](#getLineTypeSortedBy--)| <b>@deprecated.</b> Please use the 'lineTypeSortedBy' property instead. The pivot line type sorted by. |
| [isSimpleSort()](#isSimpleSort--)| <b>@deprecated.</b> Please use the 'isSimpleSort' property instead. Indicates whether a simple data sort operation will be applied. |
| [setIsSimpleSort(boolean)](#setIsSimpleSort-boolean-)| <b>@deprecated.</b> Please use the 'isSimpleSort' property instead. Indicates whether a simple data sort operation will be applied. |
| [getCell()](#getCell--)| <b>@deprecated.</b> Please use the 'cell' property instead. Sorts by the values in which row or column. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### sortType {#sortType--}

Represents the [SortOrder](../sortorder/).

```javascript
sortType : SortOrder;
```


### isSortByLabels {#isSortByLabels--}

Readonly. Indicates whether to sort the field by itself or data field.

```javascript
isSortByLabels : boolean;
```


### fieldIndex {#fieldIndex--}

Represents the index of the field sorted by. -1 means sorting the PivotField by the labels,others means sorting by the data field.

```javascript
fieldIndex : number;
```


**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotFieldSortSetting.SortBy property  instead. This method will be removed 12 months later since September 2026. Aspose apologizes for any inconvenience you may have experienced.

### sortBy {#sortBy--}

Represents the index of the field sorted by. A value of -1 indicates sorting by the pivot item's own values. When greater than or equal to zero, it represents the index of data field in the data region.

```javascript
sortBy : number;
```


### lineTypeSortedBy {#lineTypeSortedBy--}

Readonly. The pivot line type sorted by.

```javascript
lineTypeSortedBy : PivotLineType;
```


**Remarks**

Only works when not sorting this field by labels.

### isSimpleSort {#isSimpleSort--}

Indicates whether a simple data sort operation will be applied.

```javascript
isSimpleSort : boolean;
```


**Remarks**

The default value is true.

### cell {#cell--}

Readonly. Sorts by the values in which row or column.

```javascript
cell : string;
```


### getSortType() {#getSortType--}

<b>@deprecated.</b> Please use the 'sortType' property instead. Represents the [SortOrder](../sortorder/).

```javascript
getSortType() : SortOrder;
```


**Returns**

[SortOrder](../sortorder/)

### setSortType(SortOrder) {#setSortType-sortorder-}

<b>@deprecated.</b> Please use the 'sortType' property instead. Represents the [SortOrder](../sortorder/).

```javascript
setSortType(value: SortOrder) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SortOrder](../sortorder/) | The value to set. |

### isSortByLabels() {#isSortByLabels--}

<b>@deprecated.</b> Please use the 'isSortByLabels' property instead. Indicates whether to sort the field by itself or data field.

```javascript
isSortByLabels() : boolean;
```


### getFieldIndex() {#getFieldIndex--}

<b>@deprecated.</b> Please use the 'fieldIndex' property instead. Represents the index of the field sorted by. -1 means sorting the PivotField by the labels,others means sorting by the data field.

```javascript
getFieldIndex() : number;
```


**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotFieldSortSetting.SortBy property  instead. This method will be removed 12 months later since September 2026. Aspose apologizes for any inconvenience you may have experienced.

### setFieldIndex(number) {#setFieldIndex-number-}

<b>@deprecated.</b> Please use the 'fieldIndex' property instead. Represents the index of the field sorted by. -1 means sorting the PivotField by the labels,others means sorting by the data field.

```javascript
setFieldIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

NOTE: This property is now obsolete. Instead, please use PivotFieldSortSetting.SortBy property  instead. This method will be removed 12 months later since September 2026. Aspose apologizes for any inconvenience you may have experienced.

### getSortBy() {#getSortBy--}

<b>@deprecated.</b> Please use the 'sortBy' property instead. Represents the index of the field sorted by. A value of -1 indicates sorting by the pivot item's own values. When greater than or equal to zero, it represents the index of data field in the data region.

```javascript
getSortBy() : number;
```


### setSortBy(number) {#setSortBy-number-}

<b>@deprecated.</b> Please use the 'sortBy' property instead. Represents the index of the field sorted by. A value of -1 indicates sorting by the pivot item's own values. When greater than or equal to zero, it represents the index of data field in the data region.

```javascript
setSortBy(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLineTypeSortedBy() {#getLineTypeSortedBy--}

<b>@deprecated.</b> Please use the 'lineTypeSortedBy' property instead. The pivot line type sorted by.

```javascript
getLineTypeSortedBy() : PivotLineType;
```


**Returns**

[PivotLineType](../pivotlinetype/)

**Remarks**

Only works when not sorting this field by labels.

### isSimpleSort() {#isSimpleSort--}

<b>@deprecated.</b> Please use the 'isSimpleSort' property instead. Indicates whether a simple data sort operation will be applied.

```javascript
isSimpleSort() : boolean;
```


**Remarks**

The default value is true.

### setIsSimpleSort(boolean) {#setIsSimpleSort-boolean-}

<b>@deprecated.</b> Please use the 'isSimpleSort' property instead. Indicates whether a simple data sort operation will be applied.

```javascript
setIsSimpleSort(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is true.

### getCell() {#getCell--}

<b>@deprecated.</b> Please use the 'cell' property instead. Sorts by the values in which row or column.

```javascript
getCell() : string;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



