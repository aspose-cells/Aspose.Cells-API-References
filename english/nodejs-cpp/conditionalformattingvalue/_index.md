---
title: ConditionalFormattingValue
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Describes the values of the interpolation points in a gradient scale dataBar or iconSet.
type: docs
url: /nodejs-cpp/conditionalformattingvalue/
---

## ConditionalFormattingValue class

Describes the values of the interpolation points in a gradient scale, dataBar or iconSet.

```javascript
class ConditionalFormattingValue;
```


## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set "Value" to null. |
| [setType(FormatConditionValueType)](#setType-formatconditionvaluetype-)| Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set "Value" to null. |
| [isGTE()](#isGTE--)| Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true. |
| [setIsGTE(boolean)](#setIsGTE-boolean-)| Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true. |


### getType() {#getType--}

Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set "Value" to null.

```javascript
getType() : FormatConditionValueType;
```


**Returns**

[FormatConditionValueType](/nodejs-cpp/formatconditionvaluetype/)

### setType(FormatConditionValueType) {#setType-formatconditionvaluetype-}

Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set "Value" to null.

```javascript
setType(value: FormatConditionValueType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FormatConditionValueType](/nodejs-cpp/formatconditionvaluetype/) | The value to set. |

### isGTE() {#isGTE--}

Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true.

```javascript
isGTE() : boolean;
```


### setIsGTE(boolean) {#setIsGTE-boolean-}

Get or set the Greater Than Or Equal flag. Use only for icon sets, determines whether this threshold value uses the greater than or equal to operator. 'false' indicates 'greater than' is used instead of 'greater than or equal to'. Default value is true.

```javascript
setIsGTE(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |


