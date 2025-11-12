---
title: PivotFilterCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a collection of all the PivotFilters.
type: docs
url: /nodejs-cpp/pivotfiltercollection/
---

## PivotFilterCollection class

Represents a collection of all the PivotFilters.

```javascript
class PivotFilterCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the pivotfilter object at the specific index. |
| [add(number, PivotFilterType)](#add-number-pivotfiltertype-)| Adds a PivotFilter Object to the specific type |
| [addTop10Filter(number, number, PivotFilterType, boolean, number)](#addTop10Filter-number-number-pivotfiltertype-boolean-number-)| Filters by values of data pivot field. |
| [addValueFilter(number, number, PivotFilterType, number, number)](#addValueFilter-number-number-pivotfiltertype-number-number-)| Filters by values of data pivot field. |
| [addLabelFilter(number, PivotFilterType, string, string)](#addLabelFilter-number-pivotfiltertype-string-string-)| Filters by captions of row or column pivot field. |
| [addDateFilter(number, PivotFilterType, Date, Date)](#addDateFilter-number-pivotfiltertype-date-date-)| Filters by date setting of row or column pivot field. |
| [clearFilter(number)](#clearFilter-number-)| Clear PivotFilter from the specific PivotField |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### get(number) {#get-number-}

Gets the pivotfilter object at the specific index.

```javascript
get(index: number) : PivotFilter;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

**Returns**

[PivotFilter](../pivotfilter/)

### add(number, PivotFilterType) {#add-number-pivotfiltertype-}

Adds a PivotFilter Object to the specific type

```javascript
add(fieldIndex: number, type: PivotFilterType) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | the PivotField index |
| type | [PivotFilterType](../pivotfiltertype/) | the PivotFilter type |

**Returns**

the index of  the PivotFilter Object in this PivotFilterCollection.

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() and AddDateFilter() methods. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.

### addTop10Filter(number, number, PivotFilterType, boolean, number) {#addTop10Filter-number-number-pivotfiltertype-boolean-number-}

Filters by values of data pivot field.

```javascript
addTop10Filter(baseFieldIndex: number, valueFieldIndex: number, type: PivotFilterType, isTop: boolean, itemCount: number) : PivotFilter;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | number | The index of field in the source. |
| valueFieldIndex | number | The index of data field  in the data region. |
| type | [PivotFilterType](../pivotfiltertype/) | The type of filtering data. Only can be Count,Sum and Percent. |
| isTop | boolean | Indicates whether filter from top or bottom |
| itemCount | number | The item count |

**Returns**

[PivotFilter](../pivotfilter/)

### addValueFilter(number, number, PivotFilterType, number, number) {#addValueFilter-number-number-pivotfiltertype-number-number-}

Filters by values of data pivot field.

```javascript
addValueFilter(baseFieldIndex: number, valueFieldIndex: number, type: PivotFilterType, value1: number, value2: number) : PivotFilter;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | number | The index of field in the source. |
| valueFieldIndex | number | The index of value field in the value region. |
| type | [PivotFilterType](../pivotfiltertype/) | The type of filtering data. |
| value1 | number | The value of filter condition |
| value2 | number | The upper-bound value of between filter condition |

**Returns**

[PivotFilter](../pivotfilter/)

### addLabelFilter(number, PivotFilterType, string, string) {#addLabelFilter-number-pivotfiltertype-string-string-}

Filters by captions of row or column pivot field.

```javascript
addLabelFilter(baseFieldIndex: number, type: PivotFilterType, label1: string, label2: string) : PivotFilter;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | number | The index of field in the source. |
| type | [PivotFilterType](../pivotfiltertype/) | The type of filtering data. |
| label1 | string | The label of filter condition |
| label2 | string | The upper-bound label of between filter condition |

**Returns**

[PivotFilter](../pivotfilter/)

### addDateFilter(number, PivotFilterType, Date, Date) {#addDateFilter-number-pivotfiltertype-date-date-}

Filters by date setting of row or column pivot field.

```javascript
addDateFilter(baseFieldIndex: number, type: PivotFilterType, dateTime1: Date, dateTime2: Date) : PivotFilter;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | number | The index of field in the source. |
| type | [PivotFilterType](../pivotfiltertype/) | The type of filtering data. |
| dateTime1 | Date | The date label of filter condition |
| dateTime2 | Date | The upper-bound date label of between filter condition |

**Returns**

[PivotFilter](../pivotfilter/)

### clearFilter(number) {#clearFilter-number-}

Clear PivotFilter from the specific PivotField

```javascript
clearFilter(fieldIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | the PivotField index |

### getCount() {#getCount--}

<b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in.

```javascript
getCount() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



