---
title: PivotFilter
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a PivotFilter in PivotFilter Collection.
type: docs
url: /nodejs-cpp/pivotfilter/
---

## PivotFilter class

Represents a PivotFilter in PivotFilter Collection.

```javascript
class PivotFilter;
```


## Methods

| Method | Description |
| --- | --- |
| [getUseWholeDay()](#getUseWholeDay--)| Indicates whether uses whole days in its filtering criteria. |
| [setUseWholeDay(boolean)](#setUseWholeDay-boolean-)| Indicates whether uses whole days in its filtering criteria. |
| [getAutoFilter()](#getAutoFilter--)| Gets the autofilter of the pivot filter. |
| [getFilterType()](#getFilterType--)| Gets the autofilter type of the pivot filter. |
| [getFieldIndex()](#getFieldIndex--)| Gets the index of source field which this pivot filter is applied to. |
| [getFilterCategory()](#getFilterCategory--)| Gets the category of this filter. |
| [getValue1()](#getValue1--)| Gets the string value1 of the label pivot filter. |
| [setValue1(string)](#setValue1-string-)| Gets the string value1 of the label pivot filter. |
| [getValue2()](#getValue2--)| Gets the string value2 of the label pivot filter. |
| [setValue2(string)](#setValue2-string-)| Gets the string value2 of the label pivot filter. |
| [getMeasureFldIndex()](#getMeasureFldIndex--)| Gets the measure field index of the pivot filter. |
| [setMeasureFldIndex(number)](#setMeasureFldIndex-number-)| Gets the measure field index of the pivot filter. |
| [getValueFieldIndex()](#getValueFieldIndex--)| Gets the index of value field in the value region. |
| [setValueFieldIndex(number)](#setValueFieldIndex-number-)| Gets the index of value field in the value region. |
| [getMeasureCubeFieldIndex()](#getMeasureCubeFieldIndex--)| Specifies the index of the measure cube field. this property is used only by filters in OLAP pivots and specifies on which measure a value filter should apply. |
| [getMemberPropertyFieldIndex()](#getMemberPropertyFieldIndex--)| Gets the member property field index of the pivot filter. |
| [setMemberPropertyFieldIndex(number)](#setMemberPropertyFieldIndex-number-)| Gets the member property field index of the pivot filter. |
| [getName()](#getName--)| Gets the name of the pivot filter. |
| [setName(string)](#setName-string-)| Gets the name of the pivot filter. |
| [getEvaluationOrder()](#getEvaluationOrder--)| Gets the Evaluation Order of the pivot filter. |
| [setEvaluationOrder(number)](#setEvaluationOrder-number-)| Gets the Evaluation Order of the pivot filter. |
| [getTop10Value()](#getTop10Value--)| Gets top 10 setting of the filter. |
| [getLabels()](#getLabels--)| Gets labels of the caption filter. |
| [getNumberValues()](#getNumberValues--)| Gets values of the number filter. |
| [getDateTimeValues()](#getDateTimeValues--)| Gets values of the number filter. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getUseWholeDay() {#getUseWholeDay--}

Indicates whether uses whole days in its filtering criteria.

```javascript
getUseWholeDay() : boolean;
```


### setUseWholeDay(boolean) {#setUseWholeDay-boolean-}

Indicates whether uses whole days in its filtering criteria.

```javascript
setUseWholeDay(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAutoFilter() {#getAutoFilter--}

Gets the autofilter of the pivot filter.

```javascript
getAutoFilter() : AutoFilter;
```


**Returns**

[AutoFilter](../autofilter/)

**Remarks**

NOTE: This method is now obsolete. Instead, please use FilterLabel, FilterValue,FilterDate or FilterTop10 method. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.

### getFilterType() {#getFilterType--}

Gets the autofilter type of the pivot filter.

```javascript
getFilterType() : PivotFilterType;
```


**Returns**

[PivotFilterType](../pivotfiltertype/)

### getFieldIndex() {#getFieldIndex--}

Gets the index of source field which this pivot filter is applied to.

```javascript
getFieldIndex() : number;
```


### getFilterCategory() {#getFilterCategory--}

Gets the category of this filter.

```javascript
getFilterCategory() : FilterCategory;
```


**Returns**

[FilterCategory](../filtercategory/)

### getValue1() {#getValue1--}

Gets the string value1 of the label pivot filter.

```javascript
getValue1() : string;
```


### setValue1(string) {#setValue1-string-}

Gets the string value1 of the label pivot filter.

```javascript
setValue1(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getValue2() {#getValue2--}

Gets the string value2 of the label pivot filter.

```javascript
getValue2() : string;
```


### setValue2(string) {#setValue2-string-}

Gets the string value2 of the label pivot filter.

```javascript
setValue2(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getMeasureFldIndex() {#getMeasureFldIndex--}

Gets the measure field index of the pivot filter.

```javascript
getMeasureFldIndex() : number;
```


**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotFilter.ValueFieldIndex property. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.

### setMeasureFldIndex(number) {#setMeasureFldIndex-number-}

Gets the measure field index of the pivot filter.

```javascript
setMeasureFldIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotFilter.ValueFieldIndex property. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.

### getValueFieldIndex() {#getValueFieldIndex--}

Gets the index of value field in the value region.

```javascript
getValueFieldIndex() : number;
```


### setValueFieldIndex(number) {#setValueFieldIndex-number-}

Gets the index of value field in the value region.

```javascript
setValueFieldIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getMeasureCubeFieldIndex() {#getMeasureCubeFieldIndex--}

Specifies the index of the measure cube field. this property is used only by filters in OLAP pivots and specifies on which measure a value filter should apply.

```javascript
getMeasureCubeFieldIndex() : number;
```


### getMemberPropertyFieldIndex() {#getMemberPropertyFieldIndex--}

Gets the member property field index of the pivot filter.

```javascript
getMemberPropertyFieldIndex() : number;
```


### setMemberPropertyFieldIndex(number) {#setMemberPropertyFieldIndex-number-}

Gets the member property field index of the pivot filter.

```javascript
setMemberPropertyFieldIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getName() {#getName--}

Gets the name of the pivot filter.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

Gets the name of the pivot filter.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getEvaluationOrder() {#getEvaluationOrder--}

Gets the Evaluation Order of the pivot filter.

```javascript
getEvaluationOrder() : number;
```


### setEvaluationOrder(number) {#setEvaluationOrder-number-}

Gets the Evaluation Order of the pivot filter.

```javascript
setEvaluationOrder(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

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

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



