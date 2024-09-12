---
title: FormatCondition
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents conditional formatting condition.
type: docs
url: /nodejs-cpp/formatcondition/
---

## FormatCondition class

Represents conditional formatting condition.

```javascript
class FormatCondition;
```


## Methods

| Method | Description |
| --- | --- |
| [getOperator()](#getOperator--)| Gets and sets the conditional format operator type. |
| [setOperator(OperatorType)](#setOperator-operatortype-)| Gets and sets the conditional format operator type. |
| [getStopIfTrue()](#getStopIfTrue--)| True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Excel 2007; |
| [setStopIfTrue(boolean)](#setStopIfTrue-boolean-)| True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Excel 2007; |
| [getPriority()](#getPriority--)| The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority. |
| [setPriority(number)](#setPriority-number-)| The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority. |
| [getStyle()](#getStyle--)| Gets or setts style of conditional formatted cell ranges. |
| [setStyle(Style)](#setStyle-style-)| Gets or setts style of conditional formatted cell ranges. |
| [getType()](#getType--)| Gets and sets whether the conditional format Type. |
| [setType(FormatConditionType)](#setType-formatconditiontype-)| Gets and sets whether the conditional format Type. |
| [getIconSet()](#getIconSet--)| Get the conditional formatting's "IconSet" instance. The default instance's IconSetType is TrafficLights31. Valid only for type = IconSet. |
| [getDataBar()](#getDataBar--)| Get the conditional formatting's "DataBar" instance. The default instance's color is blue. Valid only for type is DataBar. |
| [getColorScale()](#getColorScale--)| Get the conditional formatting's "ColorScale" instance. The default instance is a "green-yellow-red" 3ColorScale . Valid only for type = ColorScale. |
| [getTop10()](#getTop10--)| Get the conditional formatting's "Top10" instance. The default instance's rule highlights cells whose values fall in the top 10 bracket. Valid only for type is Top10. |
| [getAboveAverage()](#getAboveAverage--)| Get the conditional formatting's "AboveAverage" instance. The default instance's rule highlights cells that are above the average for all values in the range. Valid only for type = AboveAverage. |
| [getText()](#getText--)| The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null. |
| [setText(string)](#setText-string-)| The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null. |
| [getTimePeriod()](#getTimePeriod--)| The applicable time period in a "date occurring…" conditional formatting rule. Valid only for type = timePeriod. The default value is TimePeriodType.Today. |
| [setTimePeriod(TimePeriodType)](#setTimePeriod-timeperiodtype-)| The applicable time period in a "date occurring…" conditional formatting rule. Valid only for type = timePeriod. The default value is TimePeriodType.Today. |
| [getFormula1(boolean, boolean)](#getFormula1-boolean-boolean-)| Gets the value or expression associated with this format condition. |
| [getFormula1(boolean, boolean, number, number)](#getFormula1-boolean-boolean-number-number-)| Gets the value or expression of the conditional formatting of the cell. |
| [getFormula1(number, number)](#getFormula1-number-number-)| Gets the formula of the conditional formatting of the cell. |
| [getFormula2(boolean, boolean)](#getFormula2-boolean-boolean-)| Gets the value or expression associated with this format condition. |
| [getFormula2(boolean, boolean, number, number)](#getFormula2-boolean-boolean-number-number-)| Gets the value or expression of the conditional formatting of the cell. |
| [getFormula2(number, number)](#getFormula2-number-number-)| Gets the formula of the conditional formatting of the cell. |
| [setFormulas(string, string, boolean, boolean)](#setFormulas-string-string-boolean-boolean-)| Sets the value or expression associated with this format condition. |
| [setFormula1(string, boolean, boolean)](#setFormula1-string-boolean-boolean-)| Sets the value or expression associated with this format condition. |
| [setFormula2(string, boolean, boolean)](#setFormula2-string-boolean-boolean-)| Sets the value or expression associated with this format condition. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getOperator() {#getOperator--}

Gets and sets the conditional format operator type.

```javascript
getOperator() : OperatorType;
```


**Returns**

[OperatorType](../operatortype/)

### setOperator(OperatorType) {#setOperator-operatortype-}

Gets and sets the conditional format operator type.

```javascript
setOperator(value: OperatorType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [OperatorType](../operatortype/) | The value to set. |

### getStopIfTrue() {#getStopIfTrue--}

True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Excel 2007;

```javascript
getStopIfTrue() : boolean;
```


### setStopIfTrue(boolean) {#setStopIfTrue-boolean-}

True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Excel 2007;

```javascript
setStopIfTrue(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPriority() {#getPriority--}

The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority.

```javascript
getPriority() : number;
```


### setPriority(number) {#setPriority-number-}

The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority.

```javascript
setPriority(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getStyle() {#getStyle--}

Gets or setts style of conditional formatted cell ranges.

```javascript
getStyle() : Style;
```


**Returns**

[Style](../style/)

### setStyle(Style) {#setStyle-style-}

Gets or setts style of conditional formatted cell ranges.

```javascript
setStyle(value: Style) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Style](../style/) | The value to set. |

### getType() {#getType--}

Gets and sets whether the conditional format Type.

```javascript
getType() : FormatConditionType;
```


**Returns**

[FormatConditionType](../formatconditiontype/)

### setType(FormatConditionType) {#setType-formatconditiontype-}

Gets and sets whether the conditional format Type.

```javascript
setType(value: FormatConditionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FormatConditionType](../formatconditiontype/) | The value to set. |

### getIconSet() {#getIconSet--}

Get the conditional formatting's "IconSet" instance. The default instance's IconSetType is TrafficLights31. Valid only for type = IconSet.

```javascript
getIconSet() : IconSet;
```


**Returns**

[IconSet](../iconset/)

### getDataBar() {#getDataBar--}

Get the conditional formatting's "DataBar" instance. The default instance's color is blue. Valid only for type is DataBar.

```javascript
getDataBar() : DataBar;
```


**Returns**

[DataBar](../databar/)

### getColorScale() {#getColorScale--}

Get the conditional formatting's "ColorScale" instance. The default instance is a "green-yellow-red" 3ColorScale . Valid only for type = ColorScale.

```javascript
getColorScale() : ColorScale;
```


**Returns**

[ColorScale](../colorscale/)

### getTop10() {#getTop10--}

Get the conditional formatting's "Top10" instance. The default instance's rule highlights cells whose values fall in the top 10 bracket. Valid only for type is Top10.

```javascript
getTop10() : Top10;
```


**Returns**

[Top10](../top10/)

### getAboveAverage() {#getAboveAverage--}

Get the conditional formatting's "AboveAverage" instance. The default instance's rule highlights cells that are above the average for all values in the range. Valid only for type = AboveAverage.

```javascript
getAboveAverage() : AboveAverage;
```


**Returns**

[AboveAverage](../aboveaverage/)

### getText() {#getText--}

The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null.

```javascript
getText() : string;
```


### setText(string) {#setText-string-}

The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null.

```javascript
setText(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTimePeriod() {#getTimePeriod--}

The applicable time period in a "date occurring…" conditional formatting rule. Valid only for type = timePeriod. The default value is TimePeriodType.Today.

```javascript
getTimePeriod() : TimePeriodType;
```


**Returns**

[TimePeriodType](../timeperiodtype/)

### setTimePeriod(TimePeriodType) {#setTimePeriod-timeperiodtype-}

The applicable time period in a "date occurring…" conditional formatting rule. Valid only for type = timePeriod. The default value is TimePeriodType.Today.

```javascript
setTimePeriod(value: TimePeriodType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TimePeriodType](../timeperiodtype/) | The value to set. |

### getFormula1(boolean, boolean) {#getFormula1-boolean-boolean-}

Gets the value or expression associated with this format condition.

```javascript
getFormula1(isR1C1: boolean, isLocal: boolean) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns**

The value or expression associated with this format condition.

### getFormula1(boolean, boolean, number, number) {#getFormula1-boolean-boolean-number-number-}

Gets the value or expression of the conditional formatting of the cell.

```javascript
getFormula1(isR1C1: boolean, isLocal: boolean, row: number, column: number) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
| row | number | The row index. |
| column | number | The column index. |

**Returns**

The value or expression associated with the conditional formatting of the cell.

**Remarks**

The given cell must be contained by this conditional formatting, otherwise null will be returned.

### getFormula1(number, number) {#getFormula1-number-number-}

Gets the formula of the conditional formatting of the cell.

```javascript
getFormula1(row: number, column: number) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| column | number | The column index. |

**Returns**

The formula.

### getFormula2(boolean, boolean) {#getFormula2-boolean-boolean-}

Gets the value or expression associated with this format condition.

```javascript
getFormula2(isR1C1: boolean, isLocal: boolean) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns**

The value or expression associated with this format condition.

### getFormula2(boolean, boolean, number, number) {#getFormula2-boolean-boolean-number-number-}

Gets the value or expression of the conditional formatting of the cell.

```javascript
getFormula2(isR1C1: boolean, isLocal: boolean, row: number, column: number) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
| row | number | The row index. |
| column | number | The column index. |

**Returns**

The value or expression associated with the conditional formatting of the cell.

**Remarks**

The given cell must be contained by this conditional formatting, otherwise null will be returned.

### getFormula2(number, number) {#getFormula2-number-number-}

Gets the formula of the conditional formatting of the cell.

```javascript
getFormula2(row: number, column: number) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| column | number | The column index. |

**Returns**

The formula.

### setFormulas(string, string, boolean, boolean) {#setFormulas-string-string-boolean-boolean-}

Sets the value or expression associated with this format condition.

```javascript
setFormulas(formula1: string, formula2: string, isR1C1: boolean, isLocal: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula1 | string | The value or expression associated with this format condition.         /// If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool).         /// For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| formula2 | string | The value or expression associated with this format condition. The input format is same with formula1 |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |

### setFormula1(string, boolean, boolean) {#setFormula1-string-boolean-boolean-}

Sets the value or expression associated with this format condition.

```javascript
setFormula1(formula: string, isR1C1: boolean, isLocal: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | The value or expression associated with this format condition.         /// If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool).         /// For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |

### setFormula2(string, boolean, boolean) {#setFormula2-string-boolean-boolean-}

Sets the value or expression associated with this format condition.

```javascript
setFormula2(formula: string, isR1C1: boolean, isLocal: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | The value or expression associated with this format condition.         /// If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool).         /// For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



