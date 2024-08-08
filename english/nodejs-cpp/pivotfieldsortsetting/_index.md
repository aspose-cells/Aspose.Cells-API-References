---
title: PivotFieldSortSetting
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the setting of sorting pivot fields.
type: docs
url: /nodejs-cpp/pivotfieldsortsetting/
---

## PivotFieldSortSetting class

Represents the setting of sorting pivot fields.

```javascript
class PivotFieldSortSetting;
```


## Methods

| Method | Description |
| --- | --- |
| [getSortType()](#getSortType--)| Represents the [SortOrder](../sortorder/). |
| [isSortByLabels()](#isSortByLabels--)| Indicates whether sorting the field by itself or data field. |
| [getFieldIndex()](#getFieldIndex--)| Represents the index of the field sorted by. -1 means sorting the PivotField by the labels,others means sorting by the data field. |
| [getLineTypeSortedBy()](#getLineTypeSortedBy--)| The pivot line type sorted by. |
| [isSimpleSort()](#isSimpleSort--)| Indicates whether a simple data sort operation will be applied. |
| [getCell()](#getCell--)| Sorts by the values in which row or column. |


### getSortType() {#getSortType--}

Represents the [SortOrder](../sortorder/).

```javascript
getSortType() : SortOrder;
```


**Returns**

[SortOrder](../sortorder/)

### isSortByLabels() {#isSortByLabels--}

Indicates whether sorting the field by itself or data field.

```javascript
isSortByLabels() : boolean;
```


### getFieldIndex() {#getFieldIndex--}

Represents the index of the field sorted by. -1 means sorting the PivotField by the labels,others means sorting by the data field.

```javascript
getFieldIndex() : number;
```


### getLineTypeSortedBy() {#getLineTypeSortedBy--}

The pivot line type sorted by.

```javascript
getLineTypeSortedBy() : PivotLineType;
```


**Returns**

[PivotLineType](../pivotlinetype/)

**Remarks**

Only works when not sorting this field by labels.

### isSimpleSort() {#isSimpleSort--}

Indicates whether a simple data sort operation will be applied.

```javascript
isSimpleSort() : boolean;
```


**Remarks**

The default value is true.

### getCell() {#getCell--}

Sorts by the values in which row or column.

```javascript
getCell() : string;
```



