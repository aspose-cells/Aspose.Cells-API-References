---
title: PivotFieldGroupOptions
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Options for pivot field grouping settings.
type: docs
url: /javascript-cpp/pivotfieldgroupoptions/
---

## PivotFieldGroupOptions class

Options for pivot field grouping settings.

```javascript
class PivotFieldGroupOptions;
```


## Constructors

| Name | Description |
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


