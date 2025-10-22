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
