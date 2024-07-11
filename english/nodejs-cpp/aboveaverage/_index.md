---
title: AboveAverage
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Describe the AboveAverage conditional formatting rule. This conditional formatting rule highlights cells that are above or below the average for all values in the range.
type: docs
url: /nodejs-cpp/aboveaverage/
---

## AboveAverage class

Describe the AboveAverage conditional formatting rule. This conditional formatting rule highlights cells that are above or below the average for all values in the range.

```javascript
class AboveAverage;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [isAboveAverage()](#isAboveAverage--)| Get or set the flag indicating whether the rule is an "above average" rule. 'true' indicates 'above average'. Default value is true. |
| [setIsAboveAverage(boolean)](#setIsAboveAverage-boolean-)| Get or set the flag indicating whether the rule is an "above average" rule. 'true' indicates 'above average'. Default value is true. |
| [isEqualAverage()](#isEqualAverage--)| Get or set the flag indicating whether the 'aboveAverage' and 'belowAverage' criteria is inclusive of the average itself, or exclusive of that value. 'true' indicates to include the average value in the criteria. Default value is false. |
| [setIsEqualAverage(boolean)](#setIsEqualAverage-boolean-)| Get or set the flag indicating whether the 'aboveAverage' and 'belowAverage' criteria is inclusive of the average itself, or exclusive of that value. 'true' indicates to include the average value in the criteria. Default value is false. |
| [getStdDev()](#getStdDev--)| Get or set the number of standard deviations to include above or below the average in the conditional formatting rule. The input value must between 0 and 3 (include 0 and 3). Setting this value to 0 means stdDev is not set. The default value is 0. |
| [setStdDev(number)](#setStdDev-number-)| Get or set the number of standard deviations to include above or below the average in the conditional formatting rule. The input value must between 0 and 3 (include 0 and 3). Setting this value to 0 means stdDev is not set. The default value is 0. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### isAboveAverage() {#isAboveAverage--}

Get or set the flag indicating whether the rule is an "above average" rule. 'true' indicates 'above average'. Default value is true.

```javascript
isAboveAverage() : boolean;
```


### setIsAboveAverage(boolean) {#setIsAboveAverage-boolean-}

Get or set the flag indicating whether the rule is an "above average" rule. 'true' indicates 'above average'. Default value is true.

```javascript
setIsAboveAverage(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isEqualAverage() {#isEqualAverage--}

Get or set the flag indicating whether the 'aboveAverage' and 'belowAverage' criteria is inclusive of the average itself, or exclusive of that value. 'true' indicates to include the average value in the criteria. Default value is false.

```javascript
isEqualAverage() : boolean;
```


### setIsEqualAverage(boolean) {#setIsEqualAverage-boolean-}

Get or set the flag indicating whether the 'aboveAverage' and 'belowAverage' criteria is inclusive of the average itself, or exclusive of that value. 'true' indicates to include the average value in the criteria. Default value is false.

```javascript
setIsEqualAverage(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getStdDev() {#getStdDev--}

Get or set the number of standard deviations to include above or below the average in the conditional formatting rule. The input value must between 0 and 3 (include 0 and 3). Setting this value to 0 means stdDev is not set. The default value is 0.

```javascript
getStdDev() : number;
```


### setStdDev(number) {#setStdDev-number-}

Get or set the number of standard deviations to include above or below the average in the conditional formatting rule. The input value must between 0 and 3 (include 0 and 3). Setting this value to 0 means stdDev is not set. The default value is 0.

```javascript
setStdDev(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |


