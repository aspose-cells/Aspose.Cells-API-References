---
title: SubtotalSetting
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the setting of the subtotal .
type: docs
url: /nodejs-cpp/subtotalsetting/
---

## SubtotalSetting class

Represents the setting of the subtotal .

```javascript
class SubtotalSetting;
```


## Methods

| Method | Description |
| --- | --- |
| [getGroupBy()](#getGroupBy--)| The field to group by, as a zero-based integer offset |
| [getSubtotalFunction()](#getSubtotalFunction--)| The subtotal function. |
| [getTotalList()](#getTotalList--)| An array of zero-based field offsets, indicating the fields to which the subtotals are added. |
| [getSummaryBelowData()](#getSummaryBelowData--)| Indicates whether add summary below data. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getGroupBy() {#getGroupBy--}

The field to group by, as a zero-based integer offset

```javascript
getGroupBy() : number;
```


### getSubtotalFunction() {#getSubtotalFunction--}

The subtotal function.

```javascript
getSubtotalFunction() : ConsolidationFunction;
```


**Returns**

[ConsolidationFunction](../consolidationfunction/)

### getTotalList() {#getTotalList--}

An array of zero-based field offsets, indicating the fields to which the subtotals are added.

```javascript
getTotalList() : number[];
```


**Returns**

number[]

### getSummaryBelowData() {#getSummaryBelowData--}

Indicates whether add summary below data.

```javascript
getSummaryBelowData() : boolean;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



