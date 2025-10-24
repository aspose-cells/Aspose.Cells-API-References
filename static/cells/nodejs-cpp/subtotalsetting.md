##SubtotalSetting
Represents the setting of the subtotal .
## SubtotalSetting class
Represents the setting of the subtotal .
```javascript
class SubtotalSetting;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [groupBy](#groupBy--)| number | Readonly. The field to group by, as a zero-based integer offset |
| [subtotalFunction](#subtotalFunction--)| ConsolidationFunction | Readonly. The subtotal function. |
| [totalList](#totalList--)| number[] | Readonly. An array of zero-based field offsets, indicating the fields to which the subtotals are added. |
| [summaryBelowData](#summaryBelowData--)| boolean | Readonly. Indicates whether add summary below data. |
## Methods
| Method | Description |
| --- | --- |
| [getGroupBy()](#getGroupBy--)| <b>@deprecated.</b> Please use the 'groupBy' property instead. The field to group by, as a zero-based integer offset |
| [getSubtotalFunction()](#getSubtotalFunction--)| <b>@deprecated.</b> Please use the 'subtotalFunction' property instead. The subtotal function. |
| [getTotalList()](#getTotalList--)| <b>@deprecated.</b> Please use the 'totalList' property instead. An array of zero-based field offsets, indicating the fields to which the subtotals are added. |
| [getSummaryBelowData()](#getSummaryBelowData--)| <b>@deprecated.</b> Please use the 'summaryBelowData' property instead. Indicates whether add summary below data. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### groupBy {#groupBy--}
Readonly. The field to group by, as a zero-based integer offset
```javascript
groupBy : number;
```
### subtotalFunction {#subtotalFunction--}
Readonly. The subtotal function.
```javascript
subtotalFunction : ConsolidationFunction;
```
### totalList {#totalList--}
Readonly. An array of zero-based field offsets, indicating the fields to which the subtotals are added.
```javascript
totalList : number[];
```
### summaryBelowData {#summaryBelowData--}
Readonly. Indicates whether add summary below data.
```javascript
summaryBelowData : boolean;
```
### getGroupBy() {#getGroupBy--}
```javascript
getGroupBy() : number;
```
### getSubtotalFunction() {#getSubtotalFunction--}
```javascript
getSubtotalFunction() : ConsolidationFunction;
```
**Returns**
[ConsolidationFunction](../consolidationfunction/)
### getTotalList() {#getTotalList--}
```javascript
getTotalList() : number[];
```
**Returns**
number[]
### getSummaryBelowData() {#getSummaryBelowData--}
```javascript
getSummaryBelowData() : boolean;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
