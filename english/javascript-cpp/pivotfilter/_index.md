---
title: PivotFilter
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents a PivotFilter in PivotFilter Collection.
type: docs
url: /javascript-cpp/pivotfilter/
---

## PivotFilter class

Represents a PivotFilter in PivotFilter Collection.

```javascript
class PivotFilter;
```


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [useWholeDay](#useWholeDay--)| boolean | Indicates whether to use whole days in its date filtering criteria. |
| [autoFilter](#autoFilter--)| AutoFilter | Readonly. Gets the autofilter of the pivot filter. |
| [filterType](#filterType--)| PivotFilterType | Readonly. Gets the filter type of the pivot filter. |
| [fieldIndex](#fieldIndex--)| number | Readonly. Gets the index of source field which this pivot filter is applied to. |
| [filterCategory](#filterCategory--)| FilterCategory | Readonly. Gets the category of this filter. |
| [value1](#value1--)| string | Gets the string value1 of the label pivot filter. |
| [value2](#value2--)| string | Gets the string value2 of the label pivot filter. |
| [measureFldIndex](#measureFldIndex--)| number | Gets the measure field index of the pivot filter. |
| [valueFieldIndex](#valueFieldIndex--)| number | Gets the index of value field in the value region. |
| [measureCubeFieldIndex](#measureCubeFieldIndex--)| number | Readonly. Specifies the index of the measure cube field. this property is used only by filters in OLAP pivots and specifies on which measure a value filter should apply. |
| [memberPropertyFieldIndex](#memberPropertyFieldIndex--)| number | Gets the member property field index of the pivot filter. |
| [name](#name--)| string | Gets the name of the pivot filter. |
| [evaluationOrder](#evaluationOrder--)| number | Gets the Evaluation Order of the pivot filter. |

## Methods

| Method | Description |
| --- | --- |
| [getTop10Value()](#getTop10Value--)| Gets top 10 setting of the filter. |
| [getLabels()](#getLabels--)| Gets labels of the caption filter. |
| [getNumberValues()](#getNumberValues--)| Gets values of the number filter. |
| [getDateTimeValues()](#getDateTimeValues--)| Gets values of the number filter. |


### useWholeDay {#useWholeDay--}

Indicates whether to use whole days in its date filtering criteria.

```javascript
useWholeDay : boolean;
```


### autoFilter {#autoFilter--}

Readonly. Gets the autofilter of the pivot filter.

```javascript
autoFilter : AutoFilter;
```


**Remarks**

NOTE: This method is now obsolete. Instead, please use FilterLabel, FilterValue,FilterDate or FilterTop10 method. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.

### filterType {#filterType--}

Readonly. Gets the filter type of the pivot filter.

```javascript
filterType : PivotFilterType;
```


### fieldIndex {#fieldIndex--}

Readonly. Gets the index of source field which this pivot filter is applied to.

```javascript
fieldIndex : number;
```


### filterCategory {#filterCategory--}

Readonly. Gets the category of this filter.

```javascript
filterCategory : FilterCategory;
```


### value1 {#value1--}

Gets the string value1 of the label pivot filter.

```javascript
value1 : string;
```


### value2 {#value2--}

Gets the string value2 of the label pivot filter.

```javascript
value2 : string;
```


### measureFldIndex {#measureFldIndex--}

Gets the measure field index of the pivot filter.

```javascript
measureFldIndex : number;
```


**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotFilter.ValueFieldIndex property. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.

### valueFieldIndex {#valueFieldIndex--}

Gets the index of value field in the value region.

```javascript
valueFieldIndex : number;
```


### measureCubeFieldIndex {#measureCubeFieldIndex--}

Readonly. Specifies the index of the measure cube field. this property is used only by filters in OLAP pivots and specifies on which measure a value filter should apply.

```javascript
measureCubeFieldIndex : number;
```


### memberPropertyFieldIndex {#memberPropertyFieldIndex--}

Gets the member property field index of the pivot filter.

```javascript
memberPropertyFieldIndex : number;
```


### name {#name--}

Gets the name of the pivot filter.

```javascript
name : string;
```


### evaluationOrder {#evaluationOrder--}

Gets the Evaluation Order of the pivot filter.

```javascript
evaluationOrder : number;
```


### getTop10Value() {#getTop10Value--}

Gets top 10 setting of the filter.

```javascript
getTop10Value() : Top10Filter;
```


**Returns**

[Top10Filter](../top10filter/)

### getLabels() {#getLabels--}

Gets labels of the caption filter.

```javascript
getLabels() : string[];
```


**Returns**

string[]

### getNumberValues() {#getNumberValues--}

Gets values of the number filter.

```javascript
getNumberValues() : number[];
```


**Returns**

number[]

### getDateTimeValues() {#getDateTimeValues--}

Gets values of the number filter.

```javascript
getDateTimeValues() : Date[];
```


**Returns**

Date[]


