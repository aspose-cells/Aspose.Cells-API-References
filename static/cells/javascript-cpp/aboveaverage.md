##AboveAverage
Describe the AboveAverage conditional formatting rule. This conditional formatting rule highlights cells that are above or below the average for all values in the range.
## AboveAverage class
Describe the AboveAverage conditional formatting rule. This conditional formatting rule highlights cells that are above or below the average for all values in the range.
```javascript
class AboveAverage;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isAboveAverage](#isAboveAverage--)| boolean | Get or set the flag indicating whether the rule is an "above average" rule. 'true' indicates 'above average'. Default value is true. |
| [isEqualAverage](#isEqualAverage--)| boolean | Get or set the flag indicating whether the 'aboveAverage' and 'belowAverage' criteria is inclusive of the average itself, or exclusive of that value. 'true' indicates to include the average value in the criteria. Default value is false. |
| [stdDev](#stdDev--)| number | Get or set the number of standard deviations to include above or below the average in the conditional formatting rule. The input value must between 0 and 3 (include 0 and 3). Setting this value to 0 means stdDev is not set. The default value is 0. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### isAboveAverage {#isAboveAverage--}
Get or set the flag indicating whether the rule is an "above average" rule. 'true' indicates 'above average'. Default value is true.
```javascript
isAboveAverage : boolean;
```
### isEqualAverage {#isEqualAverage--}
Get or set the flag indicating whether the 'aboveAverage' and 'belowAverage' criteria is inclusive of the average itself, or exclusive of that value. 'true' indicates to include the average value in the criteria. Default value is false.
```javascript
isEqualAverage : boolean;
```
### stdDev {#stdDev--}
Get or set the number of standard deviations to include above or below the average in the conditional formatting rule. The input value must between 0 and 3 (include 0 and 3). Setting this value to 0 means stdDev is not set. The default value is 0.
```javascript
stdDev : number;
```
