##AboveAverage
Describe the AboveAverage conditional formatting rule. This conditional formatting rule highlights cells that are above or below the average for all values in the range.
## AboveAverage class
Describe the AboveAverage conditional formatting rule. This conditional formatting rule highlights cells that are above or below the average for all values in the range.
```javascript
class AboveAverage;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isAboveAverage](#isAboveAverage--)| boolean | Get or set the flag indicating whether the rule is an "above average" rule. 'true' indicates 'above average'. Default value is true. |
| [isEqualAverage](#isEqualAverage--)| boolean | Get or set the flag indicating whether the 'aboveAverage' and 'belowAverage' criteria is inclusive of the average itself, or exclusive of that value. 'true' indicates to include the average value in the criteria. Default value is false. |
| [stdDev](#stdDev--)| number | Get or set the number of standard deviations to include above or below the average in the conditional formatting rule. The input value must between 0 and 3 (include 0 and 3). Setting this value to 0 means stdDev is not set. The default value is 0. |
## Methods
| Method | Description |
| --- | --- |
| [isAboveAverage()](#isAboveAverage--)| <b>@deprecated.</b> Please use the 'isAboveAverage' property instead. Get or set the flag indicating whether the rule is an "above average" rule. 'true' indicates 'above average'. Default value is true. |
| [setIsAboveAverage(boolean)](#setIsAboveAverage-boolean-)| <b>@deprecated.</b> Please use the 'isAboveAverage' property instead. Get or set the flag indicating whether the rule is an "above average" rule. 'true' indicates 'above average'. Default value is true. |
| [isEqualAverage()](#isEqualAverage--)| <b>@deprecated.</b> Please use the 'isEqualAverage' property instead. Get or set the flag indicating whether the 'aboveAverage' and 'belowAverage' criteria is inclusive of the average itself, or exclusive of that value. 'true' indicates to include the average value in the criteria. Default value is false. |
| [setIsEqualAverage(boolean)](#setIsEqualAverage-boolean-)| <b>@deprecated.</b> Please use the 'isEqualAverage' property instead. Get or set the flag indicating whether the 'aboveAverage' and 'belowAverage' criteria is inclusive of the average itself, or exclusive of that value. 'true' indicates to include the average value in the criteria. Default value is false. |
| [getStdDev()](#getStdDev--)| <b>@deprecated.</b> Please use the 'stdDev' property instead. Get or set the number of standard deviations to include above or below the average in the conditional formatting rule. The input value must between 0 and 3 (include 0 and 3). Setting this value to 0 means stdDev is not set. The default value is 0. |
| [setStdDev(number)](#setStdDev-number-)| <b>@deprecated.</b> Please use the 'stdDev' property instead. Get or set the number of standard deviations to include above or below the average in the conditional formatting rule. The input value must between 0 and 3 (include 0 and 3). Setting this value to 0 means stdDev is not set. The default value is 0. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### isAboveAverage() {#isAboveAverage--}
```javascript
isAboveAverage() : boolean;
```
### setIsAboveAverage(boolean) {#setIsAboveAverage-boolean-}
```javascript
setIsAboveAverage(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isEqualAverage() {#isEqualAverage--}
```javascript
isEqualAverage() : boolean;
```
### setIsEqualAverage(boolean) {#setIsEqualAverage-boolean-}
```javascript
setIsEqualAverage(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getStdDev() {#getStdDev--}
```javascript
getStdDev() : number;
```
### setStdDev(number) {#setStdDev-number-}
```javascript
setStdDev(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
