##DataBarBorder
Represents the border of the data bars specified by a conditional formatting rule.
## DataBarBorder class
Represents the border of the data bars specified by a conditional formatting rule.
```javascript
class DataBarBorder;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [color](#color--)| Color | Gets or sets the border's color of data bars specified by a conditional formatting rule. |
| [type](#type--)| DataBarBorderType | Gets or sets the border's type of data bars specified by a conditional formatting rule. |
## Methods
| Method | Description |
| --- | --- |
| [getColor()](#getColor--)| <b>@deprecated.</b> Please use the 'color' property instead. Gets or sets the border's color of data bars specified by a conditional formatting rule. |
| [setColor(Color)](#setColor-color-)| <b>@deprecated.</b> Please use the 'color' property instead. Gets or sets the border's color of data bars specified by a conditional formatting rule. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets or sets the border's type of data bars specified by a conditional formatting rule. |
| [setType(DataBarBorderType)](#setType-databarbordertype-)| <b>@deprecated.</b> Please use the 'type' property instead. Gets or sets the border's type of data bars specified by a conditional formatting rule. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### color {#color--}
Gets or sets the border's color of data bars specified by a conditional formatting rule.
```javascript
color : Color;
```
### type {#type--}
Gets or sets the border's type of data bars specified by a conditional formatting rule.
```javascript
type : DataBarBorderType;
```
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
### getType() {#getType--}
```javascript
getType() : DataBarBorderType;
```
**Returns**
[DataBarBorderType](../databarbordertype/)
### setType(DataBarBorderType) {#setType-databarbordertype-}
```javascript
setType(value: DataBarBorderType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DataBarBorderType](../databarbordertype/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
