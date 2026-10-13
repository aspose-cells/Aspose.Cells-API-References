---
title: PivotFieldSortSetting
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the setting for sorting pivot fields.
type: docs
url: /javascript-cpp/pivotfieldsortsetting/
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



