---
title: ColorScale
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Describe the ColorScale conditional formatting rule. This conditional formatting rule creates a gradated color scale on the cells.
type: docs
url: /nodejs-cpp/colorscale/
---

## ColorScale class

Describe the ColorScale conditional formatting rule. This conditional formatting rule creates a gradated color scale on the cells.

```javascript
class ColorScale;
```


## Methods

| Method | Description |
| --- | --- |
| [getIs3ColorScale()](#getIs3ColorScale--)| Indicates whether conditional formatting is 3 color scale. |
| [setIs3ColorScale(boolean)](#setIs3ColorScale-boolean-)| Indicates whether conditional formatting is 3 color scale. |
| [getMinCfvo()](#getMinCfvo--)| Get or set this ColorScale's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it. |
| [getMidCfvo()](#getMidCfvo--)| Get or set this ColorScale's mid value object. Cannot set CFValueObject with type FormatConditionValueType.Max or FormatConditionValueType.Min to it. |
| [getMaxCfvo()](#getMaxCfvo--)| Get or set this ColorScale's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it. |
| [getMinColor()](#getMinColor--)| Get or set the gradient color for the minimum value in the range. |
| [setMinColor(Color)](#setMinColor-color-)| Get or set the gradient color for the minimum value in the range. |
| [getMidColor()](#getMidColor--)| Get or set the gradient color for the middle value in the range. |
| [setMidColor(Color)](#setMidColor-color-)| Get or set the gradient color for the middle value in the range. |
| [getMaxColor()](#getMaxColor--)| Get or set the gradient color for the maximum value in the range. |
| [setMaxColor(Color)](#setMaxColor-color-)| Get or set the gradient color for the maximum value in the range. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getIs3ColorScale() {#getIs3ColorScale--}

Indicates whether conditional formatting is 3 color scale.

```javascript
getIs3ColorScale() : boolean;
```


### setIs3ColorScale(boolean) {#setIs3ColorScale-boolean-}

Indicates whether conditional formatting is 3 color scale.

```javascript
setIs3ColorScale(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMinCfvo() {#getMinCfvo--}

Get or set this ColorScale's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it.

```javascript
getMinCfvo() : ConditionalFormattingValue;
```


**Returns**

[ConditionalFormattingValue](../conditionalformattingvalue/)

### getMidCfvo() {#getMidCfvo--}

Get or set this ColorScale's mid value object. Cannot set CFValueObject with type FormatConditionValueType.Max or FormatConditionValueType.Min to it.

```javascript
getMidCfvo() : ConditionalFormattingValue;
```


**Returns**

[ConditionalFormattingValue](../conditionalformattingvalue/)

### getMaxCfvo() {#getMaxCfvo--}

Get or set this ColorScale's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it.

```javascript
getMaxCfvo() : ConditionalFormattingValue;
```


**Returns**

[ConditionalFormattingValue](../conditionalformattingvalue/)

### getMinColor() {#getMinColor--}

Get or set the gradient color for the minimum value in the range.

```javascript
getMinColor() : Color;
```


**Returns**

[Color](../color/)

### setMinColor(Color) {#setMinColor-color-}

Get or set the gradient color for the minimum value in the range.

```javascript
setMinColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### getMidColor() {#getMidColor--}

Get or set the gradient color for the middle value in the range.

```javascript
getMidColor() : Color;
```


**Returns**

[Color](../color/)

### setMidColor(Color) {#setMidColor-color-}

Get or set the gradient color for the middle value in the range.

```javascript
setMidColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### getMaxColor() {#getMaxColor--}

Get or set the gradient color for the maximum value in the range.

```javascript
getMaxColor() : Color;
```


**Returns**

[Color](../color/)

### setMaxColor(Color) {#setMaxColor-color-}

Get or set the gradient color for the maximum value in the range.

```javascript
setMaxColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



