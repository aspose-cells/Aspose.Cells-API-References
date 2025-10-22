##TwoColorGradient
Represents two color gradient.
## TwoColorGradient class
Represents two color gradient.
```javascript
class TwoColorGradient;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(Color, Color, GradientStyleType, number)](#constructor-color-color-gradientstyletype-number-)|  |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [color1](#color1--)| Color | Gets and sets the first gradient color. |
| [color2](#color2--)| Color | Gets and sets the second gradient color. |
| [gradientStyleType](#gradientStyleType--)| GradientStyleType | Gets and sets gradient shading style. |
| [variant](#variant--)| number | Gets and sets the gradient variant. |
## Methods
| Method | Description |
| --- | --- |
| [getColor1()](#getColor1--)| <b>@deprecated.</b> Please use the 'color1' property instead. Gets and sets the first gradient color. |
| [setColor1(Color)](#setColor1-color-)| <b>@deprecated.</b> Please use the 'color1' property instead. Gets and sets the first gradient color. |
| [getColor2()](#getColor2--)| <b>@deprecated.</b> Please use the 'color2' property instead. Gets and sets the second gradient color. |
| [setColor2(Color)](#setColor2-color-)| <b>@deprecated.</b> Please use the 'color2' property instead. Gets and sets the second gradient color. |
| [getGradientStyleType()](#getGradientStyleType--)| <b>@deprecated.</b> Please use the 'gradientStyleType' property instead. Gets and sets gradient shading style. |
| [setGradientStyleType(GradientStyleType)](#setGradientStyleType-gradientstyletype-)| <b>@deprecated.</b> Please use the 'gradientStyleType' property instead. Gets and sets gradient shading style. |
| [getVariant()](#getVariant--)| <b>@deprecated.</b> Please use the 'variant' property instead. Gets and sets the gradient variant. |
| [setVariant(number)](#setVariant-number-)| <b>@deprecated.</b> Please use the 'variant' property instead. Gets and sets the gradient variant. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor(Color, Color, GradientStyleType, number) {#constructor-color-color-gradientstyletype-number-}
```javascript
constructor(color1: Color, color2: Color, gradientStyleType: GradientStyleType, variant: number);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | [Color](../color/) |  |
| color2 | [Color](../color/) |  |
| gradientStyleType | [GradientStyleType](../gradientstyletype/) |  |
| variant | number |  |
### color1 {#color1--}
Gets and sets the first gradient color.
```javascript
color1 : Color;
```
### color2 {#color2--}
Gets and sets the second gradient color.
```javascript
color2 : Color;
```
### gradientStyleType {#gradientStyleType--}
Gets and sets gradient shading style.
```javascript
gradientStyleType : GradientStyleType;
```
### variant {#variant--}
Gets and sets the gradient variant.
```javascript
variant : number;
```
### getColor1() {#getColor1--}
```javascript
getColor1() : Color;
```
**Returns**
[Color](../color/)
### setColor1(Color) {#setColor1-color-}
```javascript
setColor1(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getColor2() {#getColor2--}
```javascript
getColor2() : Color;
```
**Returns**
[Color](../color/)
### setColor2(Color) {#setColor2-color-}
```javascript
setColor2(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getGradientStyleType() {#getGradientStyleType--}
```javascript
getGradientStyleType() : GradientStyleType;
```
**Returns**
[GradientStyleType](../gradientstyletype/)
### setGradientStyleType(GradientStyleType) {#setGradientStyleType-gradientstyletype-}
```javascript
setGradientStyleType(value: GradientStyleType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GradientStyleType](../gradientstyletype/) | The value to set. |
### getVariant() {#getVariant--}
```javascript
getVariant() : number;
```
### setVariant(number) {#setVariant-number-}
```javascript
setVariant(value: number) : void;
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
