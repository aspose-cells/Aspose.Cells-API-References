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
