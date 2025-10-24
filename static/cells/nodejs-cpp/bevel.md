##Bevel
Represents a bevel of a shape
## Bevel class
Represents a bevel of a shape
```javascript
class Bevel;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [width](#width--)| number | Gets and sets the width of the bevel, or how far into the shape it is applied. In unit of Points. |
| [height](#height--)| number | Gets and sets the height of the bevel, or how far above the shape it is applied. In unit of Points. |
| [type](#type--)| BevelPresetType | Gets and sets the preset bevel type. |
## Methods
| Method | Description |
| --- | --- |
| [getWidth()](#getWidth--)| <b>@deprecated.</b> Please use the 'width' property instead. Gets and sets the width of the bevel, or how far into the shape it is applied. In unit of Points. |
| [setWidth(number)](#setWidth-number-)| <b>@deprecated.</b> Please use the 'width' property instead. Gets and sets the width of the bevel, or how far into the shape it is applied. In unit of Points. |
| [getHeight()](#getHeight--)| <b>@deprecated.</b> Please use the 'height' property instead. Gets and sets the height of the bevel, or how far above the shape it is applied. In unit of Points. |
| [setHeight(number)](#setHeight-number-)| <b>@deprecated.</b> Please use the 'height' property instead. Gets and sets the height of the bevel, or how far above the shape it is applied. In unit of Points. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets and sets the preset bevel type. |
| [setType(BevelPresetType)](#setType-bevelpresettype-)| <b>@deprecated.</b> Please use the 'type' property instead. Gets and sets the preset bevel type. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### width {#width--}
Gets and sets the width of the bevel, or how far into the shape it is applied. In unit of Points.
```javascript
width : number;
```
### height {#height--}
Gets and sets the height of the bevel, or how far above the shape it is applied. In unit of Points.
```javascript
height : number;
```
### type {#type--}
Gets and sets the preset bevel type.
```javascript
type : BevelPresetType;
```
### getWidth() {#getWidth--}
```javascript
getWidth() : number;
```
### setWidth(number) {#setWidth-number-}
```javascript
setWidth(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getHeight() {#getHeight--}
```javascript
getHeight() : number;
```
### setHeight(number) {#setHeight-number-}
```javascript
setHeight(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getType() {#getType--}
```javascript
getType() : BevelPresetType;
```
**Returns**
[BevelPresetType](../bevelpresettype/)
### setType(BevelPresetType) {#setType-bevelpresettype-}
```javascript
setType(value: BevelPresetType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [BevelPresetType](../bevelpresettype/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
