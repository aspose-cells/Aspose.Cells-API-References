##ColorScale
Describe the ColorScale conditional formatting rule. This conditional formatting rule creates a gradated color scale on the cells.
## ColorScale class
Describe the ColorScale conditional formatting rule. This conditional formatting rule creates a gradated color scale on the cells.
```javascript
class ColorScale;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [is3ColorScale](#is3ColorScale--)| boolean | Indicates whether conditional formatting is 3 color scale. |
| [minCfvo](#minCfvo--)| ConditionalFormattingValue | Readonly. Get or set this ColorScale's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it. |
| [midCfvo](#midCfvo--)| ConditionalFormattingValue | Readonly. Get or set this ColorScale's mid value object. Cannot set CFValueObject with type FormatConditionValueType.Max or FormatConditionValueType.Min to it. |
| [maxCfvo](#maxCfvo--)| ConditionalFormattingValue | Readonly. Get or set this ColorScale's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it. |
| [minColor](#minColor--)| Color | Get or set the gradient color for the minimum value in the range. |
| [midColor](#midColor--)| Color | Get or set the gradient color for the middle value in the range. |
| [maxColor](#maxColor--)| Color | Get or set the gradient color for the maximum value in the range. |
## Methods
| Method | Description |
| --- | --- |
| [getIs3ColorScale()](#getIs3ColorScale--)| <b>@deprecated.</b> Please use the 'is3ColorScale' property instead. Indicates whether conditional formatting is 3 color scale. |
| [setIs3ColorScale(boolean)](#setIs3ColorScale-boolean-)| <b>@deprecated.</b> Please use the 'is3ColorScale' property instead. Indicates whether conditional formatting is 3 color scale. |
| [getMinCfvo()](#getMinCfvo--)| <b>@deprecated.</b> Please use the 'minCfvo' property instead. Get or set this ColorScale's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it. |
| [getMidCfvo()](#getMidCfvo--)| <b>@deprecated.</b> Please use the 'midCfvo' property instead. Get or set this ColorScale's mid value object. Cannot set CFValueObject with type FormatConditionValueType.Max or FormatConditionValueType.Min to it. |
| [getMaxCfvo()](#getMaxCfvo--)| <b>@deprecated.</b> Please use the 'maxCfvo' property instead. Get or set this ColorScale's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it. |
| [getMinColor()](#getMinColor--)| <b>@deprecated.</b> Please use the 'minColor' property instead. Get or set the gradient color for the minimum value in the range. |
| [setMinColor(Color)](#setMinColor-color-)| <b>@deprecated.</b> Please use the 'minColor' property instead. Get or set the gradient color for the minimum value in the range. |
| [getMidColor()](#getMidColor--)| <b>@deprecated.</b> Please use the 'midColor' property instead. Get or set the gradient color for the middle value in the range. |
| [setMidColor(Color)](#setMidColor-color-)| <b>@deprecated.</b> Please use the 'midColor' property instead. Get or set the gradient color for the middle value in the range. |
| [getMaxColor()](#getMaxColor--)| <b>@deprecated.</b> Please use the 'maxColor' property instead. Get or set the gradient color for the maximum value in the range. |
| [setMaxColor(Color)](#setMaxColor-color-)| <b>@deprecated.</b> Please use the 'maxColor' property instead. Get or set the gradient color for the maximum value in the range. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### is3ColorScale {#is3ColorScale--}
Indicates whether conditional formatting is 3 color scale.
```javascript
is3ColorScale : boolean;
```
### minCfvo {#minCfvo--}
Readonly. Get or set this ColorScale's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it.
```javascript
minCfvo : ConditionalFormattingValue;
```
### midCfvo {#midCfvo--}
Readonly. Get or set this ColorScale's mid value object. Cannot set CFValueObject with type FormatConditionValueType.Max or FormatConditionValueType.Min to it.
```javascript
midCfvo : ConditionalFormattingValue;
```
### maxCfvo {#maxCfvo--}
Readonly. Get or set this ColorScale's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it.
```javascript
maxCfvo : ConditionalFormattingValue;
```
### minColor {#minColor--}
Get or set the gradient color for the minimum value in the range.
```javascript
minColor : Color;
```
### midColor {#midColor--}
Get or set the gradient color for the middle value in the range.
```javascript
midColor : Color;
```
### maxColor {#maxColor--}
Get or set the gradient color for the maximum value in the range.
```javascript
maxColor : Color;
```
### getIs3ColorScale() {#getIs3ColorScale--}
```javascript
getIs3ColorScale() : boolean;
```
### setIs3ColorScale(boolean) {#setIs3ColorScale-boolean-}
```javascript
setIs3ColorScale(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getMinCfvo() {#getMinCfvo--}
```javascript
getMinCfvo() : ConditionalFormattingValue;
```
**Returns**
[ConditionalFormattingValue](../conditionalformattingvalue/)
### getMidCfvo() {#getMidCfvo--}
```javascript
getMidCfvo() : ConditionalFormattingValue;
```
**Returns**
[ConditionalFormattingValue](../conditionalformattingvalue/)
### getMaxCfvo() {#getMaxCfvo--}
```javascript
getMaxCfvo() : ConditionalFormattingValue;
```
**Returns**
[ConditionalFormattingValue](../conditionalformattingvalue/)
### getMinColor() {#getMinColor--}
```javascript
getMinColor() : Color;
```
**Returns**
[Color](../color/)
### setMinColor(Color) {#setMinColor-color-}
```javascript
setMinColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getMidColor() {#getMidColor--}
```javascript
getMidColor() : Color;
```
**Returns**
[Color](../color/)
### setMidColor(Color) {#setMidColor-color-}
```javascript
setMidColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getMaxColor() {#getMaxColor--}
```javascript
getMaxColor() : Color;
```
**Returns**
[Color](../color/)
### setMaxColor(Color) {#setMaxColor-color-}
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
