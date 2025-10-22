##ConditionalFormattingResult
Represents the result of conditional formatting which applies to a cell.
## ConditionalFormattingResult class
Represents the result of conditional formatting which applies to a cell.
```javascript
class ConditionalFormattingResult;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [conditionalStyle](#conditionalStyle--)| Style | Readonly. Gets the conditional result style. |
| [conditionalFormattingIcon](#conditionalFormattingIcon--)| ConditionalFormattingIcon | Readonly. Gets the image of icon set. |
| [conditionalFormattingDataBar](#conditionalFormattingDataBar--)| DataBar | Readonly. Gets the DataBar object. |
| [conditionalFormattingColorScale](#conditionalFormattingColorScale--)| ColorScale | Readonly. Gets the ColorScale object. |
| [colorScaleResult](#colorScaleResult--)| Color | Readonly. Gets the display color of color scale. |
## Methods
| Method | Description |
| --- | --- |
| [getConditionalStyle()](#getConditionalStyle--)| <b>@deprecated.</b> Please use the 'conditionalStyle' property instead. Gets the conditional result style. |
| [getConditionalFormattingIcon()](#getConditionalFormattingIcon--)| <b>@deprecated.</b> Please use the 'conditionalFormattingIcon' property instead. Gets the image of icon set. |
| [getConditionalFormattingDataBar()](#getConditionalFormattingDataBar--)| <b>@deprecated.</b> Please use the 'conditionalFormattingDataBar' property instead. Gets the DataBar object. |
| [getConditionalFormattingColorScale()](#getConditionalFormattingColorScale--)| <b>@deprecated.</b> Please use the 'conditionalFormattingColorScale' property instead. Gets the ColorScale object. |
| [getColorScaleResult()](#getColorScaleResult--)| <b>@deprecated.</b> Please use the 'colorScaleResult' property instead. Gets the display color of color scale. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### conditionalStyle {#conditionalStyle--}
Readonly. Gets the conditional result style.
```javascript
conditionalStyle : Style;
```
### conditionalFormattingIcon {#conditionalFormattingIcon--}
Readonly. Gets the image of icon set.
```javascript
conditionalFormattingIcon : ConditionalFormattingIcon;
```
### conditionalFormattingDataBar {#conditionalFormattingDataBar--}
Readonly. Gets the DataBar object.
```javascript
conditionalFormattingDataBar : DataBar;
```
### conditionalFormattingColorScale {#conditionalFormattingColorScale--}
Readonly. Gets the ColorScale object.
```javascript
conditionalFormattingColorScale : ColorScale;
```
### colorScaleResult {#colorScaleResult--}
Readonly. Gets the display color of color scale.
```javascript
colorScaleResult : Color;
```
### getConditionalStyle() {#getConditionalStyle--}
```javascript
getConditionalStyle() : Style;
```
**Returns**
[Style](../style/)
### getConditionalFormattingIcon() {#getConditionalFormattingIcon--}
```javascript
getConditionalFormattingIcon() : ConditionalFormattingIcon;
```
**Returns**
[ConditionalFormattingIcon](../conditionalformattingicon/)
### getConditionalFormattingDataBar() {#getConditionalFormattingDataBar--}
```javascript
getConditionalFormattingDataBar() : DataBar;
```
**Returns**
[DataBar](../databar/)
### getConditionalFormattingColorScale() {#getConditionalFormattingColorScale--}
```javascript
getConditionalFormattingColorScale() : ColorScale;
```
**Returns**
[ColorScale](../colorscale/)
### getColorScaleResult() {#getColorScaleResult--}
```javascript
getColorScaleResult() : Color;
```
**Returns**
[Color](../color/)
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
