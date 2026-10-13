---
title: PivotFieldGroupOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Options for pivot field grouping settings.
type: docs
url: /nodejs-cpp/pivotfieldgroupoptions/
---

## PivotFieldGroupOptions class

Options for pivot field grouping settings.

```javascript
class PivotFieldGroupOptions;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [isAutoStart](#isAutoStart--)| boolean | Gets or sets a value indicating whether the start value is automatically determined. |
| [isAutoEnd](#isAutoEnd--)| boolean | Gets or sets a value indicating whether the end value is automatically determined. |
| [startNumber](#startNumber--)| number | Gets or sets the start value of the grouping range. |
| [endNumber](#endNumber--)| number | Gets or sets the end value of the grouping range. |
| [startDate](#startDate--)| Date | Gets or sets the start value of the grouping range. |
| [endDate](#endDate--)| Date | Gets or sets the end value of the grouping range. |
| [interval](#interval--)| number | Gets or sets the interval size for each group. |
| [groupType](#groupType--)| PivotGroupByType | Gets or sets the grouping type for pivot field. Only for grouping date time pivot field. |
| [groupTypes](#groupTypes--)| PivotGroupByType[] | Gets or sets the grouping type for pivot field. |
| [newPivotField](#newPivotField--)| boolean | Gets or sets a value indicating whether new pivot fields should be created after grouping. |

## Methods

| Method | Description |
| --- | --- |
| [isAutoStart()](#isAutoStart--)| <b>@deprecated.</b> Please use the 'isAutoStart' property instead. Gets or sets a value indicating whether the start value is automatically determined. |
| [setIsAutoStart(boolean)](#setIsAutoStart-boolean-)| <b>@deprecated.</b> Please use the 'isAutoStart' property instead. Gets or sets a value indicating whether the start value is automatically determined. |
| [isAutoEnd()](#isAutoEnd--)| <b>@deprecated.</b> Please use the 'isAutoEnd' property instead. Gets or sets a value indicating whether the end value is automatically determined. |
| [setIsAutoEnd(boolean)](#setIsAutoEnd-boolean-)| <b>@deprecated.</b> Please use the 'isAutoEnd' property instead. Gets or sets a value indicating whether the end value is automatically determined. |
| [getStartNumber()](#getStartNumber--)| <b>@deprecated.</b> Please use the 'startNumber' property instead. Gets or sets the start value of the grouping range. |
| [setStartNumber(number)](#setStartNumber-number-)| <b>@deprecated.</b> Please use the 'startNumber' property instead. Gets or sets the start value of the grouping range. |
| [getEndNumber()](#getEndNumber--)| <b>@deprecated.</b> Please use the 'endNumber' property instead. Gets or sets the end value of the grouping range. |
| [setEndNumber(number)](#setEndNumber-number-)| <b>@deprecated.</b> Please use the 'endNumber' property instead. Gets or sets the end value of the grouping range. |
| [getStartDate()](#getStartDate--)| <b>@deprecated.</b> Please use the 'startDate' property instead. Gets or sets the start value of the grouping range. |
| [setStartDate(Date)](#setStartDate-date-)| <b>@deprecated.</b> Please use the 'startDate' property instead. Gets or sets the start value of the grouping range. |
| [getEndDate()](#getEndDate--)| <b>@deprecated.</b> Please use the 'endDate' property instead. Gets or sets the end value of the grouping range. |
| [setEndDate(Date)](#setEndDate-date-)| <b>@deprecated.</b> Please use the 'endDate' property instead. Gets or sets the end value of the grouping range. |
| [getInterval()](#getInterval--)| <b>@deprecated.</b> Please use the 'interval' property instead. Gets or sets the interval size for each group. |
| [setInterval(number)](#setInterval-number-)| <b>@deprecated.</b> Please use the 'interval' property instead. Gets or sets the interval size for each group. |
| [getGroupType()](#getGroupType--)| <b>@deprecated.</b> Please use the 'groupType' property instead. Gets or sets the grouping type for pivot field. Only for grouping date time pivot field. |
| [setGroupType(PivotGroupByType)](#setGroupType-pivotgroupbytype-)| <b>@deprecated.</b> Please use the 'groupType' property instead. Gets or sets the grouping type for pivot field. Only for grouping date time pivot field. |
| [getGroupTypes()](#getGroupTypes--)| <b>@deprecated.</b> Please use the 'groupTypes' property instead. Gets or sets the grouping type for pivot field. |
| [setGroupTypes(PivotGroupByType[])](#setGroupTypes-pivotgroupbytypearray-)| <b>@deprecated.</b> Please use the 'groupTypes' property instead. Gets or sets the grouping type for pivot field. |
| [getNewPivotField()](#getNewPivotField--)| <b>@deprecated.</b> Please use the 'newPivotField' property instead. Gets or sets a value indicating whether new pivot fields should be created after grouping. |
| [setNewPivotField(boolean)](#setNewPivotField-boolean-)| <b>@deprecated.</b> Please use the 'newPivotField' property instead. Gets or sets a value indicating whether new pivot fields should be created after grouping. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### isAutoStart {#isAutoStart--}

Gets or sets a value indicating whether the start value is automatically determined.

```javascript
isAutoStart : boolean;
```


**Remarks**

If [StartNumber](../startnumber/) or [StartDate](../startdate/) is set, this property will be false.

### isAutoEnd {#isAutoEnd--}

Gets or sets a value indicating whether the end value is automatically determined.

```javascript
isAutoEnd : boolean;
```


**Remarks**

If [EndNumber](../endnumber/) or [EndDate](../enddate/) is set, this property will be false.

### startNumber {#startNumber--}

Gets or sets the start value of the grouping range.

```javascript
startNumber : number;
```


### endNumber {#endNumber--}

Gets or sets the end value of the grouping range.

```javascript
endNumber : number;
```


### startDate {#startDate--}

Gets or sets the start value of the grouping range.

```javascript
startDate : Date;
```


### endDate {#endDate--}

Gets or sets the end value of the grouping range.

```javascript
endDate : Date;
```


### interval {#interval--}

Gets or sets the interval size for each group.

```javascript
interval : number;
```


**Remarks**

Only for number and days group.

### groupType {#groupType--}

Gets or sets the grouping type for pivot field. Only for grouping date time pivot field.

```javascript
groupType : PivotGroupByType;
```


### groupTypes {#groupTypes--}

Gets or sets the grouping type for pivot field.

```javascript
groupTypes : PivotGroupByType[];
```


**Remarks**

The order in this property will be ignored. When specifying multiple group types, base group fields will be inserted in ascending order and show group field to row/column region in descending order (Years → Quarters → Months → Days → Hours → Minutes → Seconds).

### newPivotField {#newPivotField--}

Gets or sets a value indicating whether new pivot fields should be created after grouping.

```javascript
newPivotField : boolean;
```


**Remarks**

If not explicitly set, the default value is false for numeric grouping and true for date-time grouping. Only works for the first new group pivot field of the base field.

### isAutoStart() {#isAutoStart--}

<b>@deprecated.</b> Please use the 'isAutoStart' property instead. Gets or sets a value indicating whether the start value is automatically determined.

```javascript
isAutoStart() : boolean;
```


**Remarks**

If [StartNumber](../startnumber/) or [StartDate](../startdate/) is set, this property will be false.

### setIsAutoStart(boolean) {#setIsAutoStart-boolean-}

<b>@deprecated.</b> Please use the 'isAutoStart' property instead. Gets or sets a value indicating whether the start value is automatically determined.

```javascript
setIsAutoStart(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

If [StartNumber](../startnumber/) or [StartDate](../startdate/) is set, this property will be false.

### isAutoEnd() {#isAutoEnd--}

<b>@deprecated.</b> Please use the 'isAutoEnd' property instead. Gets or sets a value indicating whether the end value is automatically determined.

```javascript
isAutoEnd() : boolean;
```


**Remarks**

If [EndNumber](../endnumber/) or [EndDate](../enddate/) is set, this property will be false.

### setIsAutoEnd(boolean) {#setIsAutoEnd-boolean-}

<b>@deprecated.</b> Please use the 'isAutoEnd' property instead. Gets or sets a value indicating whether the end value is automatically determined.

```javascript
setIsAutoEnd(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

If [EndNumber](../endnumber/) or [EndDate](../enddate/) is set, this property will be false.

### getStartNumber() {#getStartNumber--}

<b>@deprecated.</b> Please use the 'startNumber' property instead. Gets or sets the start value of the grouping range.

```javascript
getStartNumber() : number;
```


### setStartNumber(number) {#setStartNumber-number-}

<b>@deprecated.</b> Please use the 'startNumber' property instead. Gets or sets the start value of the grouping range.

```javascript
setStartNumber(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getEndNumber() {#getEndNumber--}

<b>@deprecated.</b> Please use the 'endNumber' property instead. Gets or sets the end value of the grouping range.

```javascript
getEndNumber() : number;
```


### setEndNumber(number) {#setEndNumber-number-}

<b>@deprecated.</b> Please use the 'endNumber' property instead. Gets or sets the end value of the grouping range.

```javascript
setEndNumber(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getStartDate() {#getStartDate--}

<b>@deprecated.</b> Please use the 'startDate' property instead. Gets or sets the start value of the grouping range.

```javascript
getStartDate() : Date;
```


### setStartDate(Date) {#setStartDate-date-}

<b>@deprecated.</b> Please use the 'startDate' property instead. Gets or sets the start value of the grouping range.

```javascript
setStartDate(value: Date) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |

### getEndDate() {#getEndDate--}

<b>@deprecated.</b> Please use the 'endDate' property instead. Gets or sets the end value of the grouping range.

```javascript
getEndDate() : Date;
```


### setEndDate(Date) {#setEndDate-date-}

<b>@deprecated.</b> Please use the 'endDate' property instead. Gets or sets the end value of the grouping range.

```javascript
setEndDate(value: Date) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |

### getInterval() {#getInterval--}

<b>@deprecated.</b> Please use the 'interval' property instead. Gets or sets the interval size for each group.

```javascript
getInterval() : number;
```


**Remarks**

Only for number and days group.

### setInterval(number) {#setInterval-number-}

<b>@deprecated.</b> Please use the 'interval' property instead. Gets or sets the interval size for each group.

```javascript
setInterval(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Only for number and days group.

### getGroupType() {#getGroupType--}

<b>@deprecated.</b> Please use the 'groupType' property instead. Gets or sets the grouping type for pivot field. Only for grouping date time pivot field.

```javascript
getGroupType() : PivotGroupByType;
```


**Returns**

[PivotGroupByType](../pivotgroupbytype/)

### setGroupType(PivotGroupByType) {#setGroupType-pivotgroupbytype-}

<b>@deprecated.</b> Please use the 'groupType' property instead. Gets or sets the grouping type for pivot field. Only for grouping date time pivot field.

```javascript
setGroupType(value: PivotGroupByType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotGroupByType](../pivotgroupbytype/) | The value to set. |

### getGroupTypes() {#getGroupTypes--}

<b>@deprecated.</b> Please use the 'groupTypes' property instead. Gets or sets the grouping type for pivot field.

```javascript
getGroupTypes() : PivotGroupByType[];
```


**Returns**

[PivotGroupByType](../pivotgroupbytype/)[]

**Remarks**

The order in this property will be ignored. When specifying multiple group types, base group fields will be inserted in ascending order and show group field to row/column region in descending order (Years → Quarters → Months → Days → Hours → Minutes → Seconds).

### setGroupTypes(PivotGroupByType[]) {#setGroupTypes-pivotgroupbytypearray-}

<b>@deprecated.</b> Please use the 'groupTypes' property instead. Gets or sets the grouping type for pivot field.

```javascript
setGroupTypes(value: PivotGroupByType[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotGroupByType](../pivotgroupbytype/)[] | The value to set. |

**Remarks**

The order in this property will be ignored. When specifying multiple group types, base group fields will be inserted in ascending order and show group field to row/column region in descending order (Years → Quarters → Months → Days → Hours → Minutes → Seconds).

### getNewPivotField() {#getNewPivotField--}

<b>@deprecated.</b> Please use the 'newPivotField' property instead. Gets or sets a value indicating whether new pivot fields should be created after grouping.

```javascript
getNewPivotField() : boolean;
```


**Remarks**

If not explicitly set, the default value is false for numeric grouping and true for date-time grouping. Only works for the first new group pivot field of the base field.

### setNewPivotField(boolean) {#setNewPivotField-boolean-}

<b>@deprecated.</b> Please use the 'newPivotField' property instead. Gets or sets a value indicating whether new pivot fields should be created after grouping.

```javascript
setNewPivotField(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

If not explicitly set, the default value is false for numeric grouping and true for date-time grouping. Only works for the first new group pivot field of the base field.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



