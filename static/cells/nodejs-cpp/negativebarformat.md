##NegativeBarFormat
Represents the color settings of the data bars for negative values that are defined by a data bar conditional formatting rule.
## NegativeBarFormat class
Represents the color settings of the data bars for negative values that are defined by a data bar conditional formatting rule.
```javascript
class NegativeBarFormat;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [borderColor](#borderColor--)| Color | Gets or sets a FormatColor object that you can use to specify the border color for negative data bars. |
| [borderColorType](#borderColorType--)| DataBarNegativeColorType | Gets whether to use the same border color as positive data bars. |
| [color](#color--)| Color | Gets or sets a FormatColor object that you can use to specify the fill color for negative data bars. |
| [colorType](#colorType--)| DataBarNegativeColorType | Gets or sets whether to use the same fill color as positive data bars. |
## Methods
| Method | Description |
| --- | --- |
| [getBorderColor()](#getBorderColor--)| <b>@deprecated.</b> Please use the 'borderColor' property instead. Gets or sets a FormatColor object that you can use to specify the border color for negative data bars. |
| [setBorderColor(Color)](#setBorderColor-color-)| <b>@deprecated.</b> Please use the 'borderColor' property instead. Gets or sets a FormatColor object that you can use to specify the border color for negative data bars. |
| [getBorderColorType()](#getBorderColorType--)| <b>@deprecated.</b> Please use the 'borderColorType' property instead. Gets whether to use the same border color as positive data bars. |
| [setBorderColorType(DataBarNegativeColorType)](#setBorderColorType-databarnegativecolortype-)| <b>@deprecated.</b> Please use the 'borderColorType' property instead. Gets whether to use the same border color as positive data bars. |
| [getColor()](#getColor--)| <b>@deprecated.</b> Please use the 'color' property instead. Gets or sets a FormatColor object that you can use to specify the fill color for negative data bars. |
| [setColor(Color)](#setColor-color-)| <b>@deprecated.</b> Please use the 'color' property instead. Gets or sets a FormatColor object that you can use to specify the fill color for negative data bars. |
| [getColorType()](#getColorType--)| <b>@deprecated.</b> Please use the 'colorType' property instead. Gets or sets whether to use the same fill color as positive data bars. |
| [setColorType(DataBarNegativeColorType)](#setColorType-databarnegativecolortype-)| <b>@deprecated.</b> Please use the 'colorType' property instead. Gets or sets whether to use the same fill color as positive data bars. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### borderColor {#borderColor--}
Gets or sets a FormatColor object that you can use to specify the border color for negative data bars.
```javascript
borderColor : Color;
```
### borderColorType {#borderColorType--}
Gets whether to use the same border color as positive data bars.
```javascript
borderColorType : DataBarNegativeColorType;
```
### color {#color--}
Gets or sets a FormatColor object that you can use to specify the fill color for negative data bars.
```javascript
color : Color;
```
### colorType {#colorType--}
Gets or sets whether to use the same fill color as positive data bars.
```javascript
colorType : DataBarNegativeColorType;
```
### getBorderColor() {#getBorderColor--}
```javascript
getBorderColor() : Color;
```
**Returns**
[Color](../color/)
### setBorderColor(Color) {#setBorderColor-color-}
```javascript
setBorderColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getBorderColorType() {#getBorderColorType--}
```javascript
getBorderColorType() : DataBarNegativeColorType;
```
**Returns**
[DataBarNegativeColorType](../databarnegativecolortype/)
### setBorderColorType(DataBarNegativeColorType) {#setBorderColorType-databarnegativecolortype-}
```javascript
setBorderColorType(value: DataBarNegativeColorType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DataBarNegativeColorType](../databarnegativecolortype/) | The value to set. |
### getColor() {#getColor--}
```javascript
getColor() : Color;
```
**Returns**
[Color](../color/)
### setColor(Color) {#setColor-color-}
```javascript
setColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getColorType() {#getColorType--}
```javascript
getColorType() : DataBarNegativeColorType;
```
**Returns**
[DataBarNegativeColorType](../databarnegativecolortype/)
### setColorType(DataBarNegativeColorType) {#setColorType-databarnegativecolortype-}
```javascript
setColorType(value: DataBarNegativeColorType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DataBarNegativeColorType](../databarnegativecolortype/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
