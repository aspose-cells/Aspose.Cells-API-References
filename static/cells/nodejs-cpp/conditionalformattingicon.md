##ConditionalFormattingIcon
Represents  the custom  icon of conditional formatting rule.
## ConditionalFormattingIcon class
Represents  the custom  icon of conditional formatting rule.
```javascript
class ConditionalFormattingIcon;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [imageData](#imageData--)| Uint8Array | Readonly. Gets the icon set data. |
| [type](#type--)| IconSetType | Gets and sets the icon set type. |
| [index](#index--)| number | Gets and sets the icon's index in the icon set. |
## Methods
| Method | Description |
| --- | --- |
| [getImageData()](#getImageData--)| <b>@deprecated.</b> Please use the 'imageData' property instead. Gets the icon set data. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets and sets the icon set type. |
| [setType(IconSetType)](#setType-iconsettype-)| <b>@deprecated.</b> Please use the 'type' property instead. Gets and sets the icon set type. |
| [getIndex()](#getIndex--)| <b>@deprecated.</b> Please use the 'index' property instead. Gets and sets the icon's index in the icon set. |
| [setIndex(number)](#setIndex-number-)| <b>@deprecated.</b> Please use the 'index' property instead. Gets and sets the icon's index in the icon set. |
| [getImageData(Cell)](#getImageData-cell-)| Gets the image data with the setting of cell. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| static [getIconImageData(IconSetType, number)](#getIconImageData-iconsettype-number-)| Get the icon set data |
### imageData {#imageData--}
Readonly. Gets the icon set data.
```javascript
imageData : Uint8Array;
```
### type {#type--}
Gets and sets the icon set type.
```javascript
type : IconSetType;
```
### index {#index--}
Gets and sets the icon's index in the icon set.
```javascript
index : number;
```
### getImageData() {#getImageData--}
```javascript
getImageData() : Uint8Array;
```
### getType() {#getType--}
```javascript
getType() : IconSetType;
```
**Returns**
[IconSetType](../iconsettype/)
### setType(IconSetType) {#setType-iconsettype-}
```javascript
setType(value: IconSetType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IconSetType](../iconsettype/) | The value to set. |
### getIndex() {#getIndex--}
```javascript
getIndex() : number;
```
### setIndex(number) {#setIndex-number-}
```javascript
setIndex(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getImageData(Cell) {#getImageData-cell-}
Gets the image data with the setting of cell.
```javascript
getImageData(cell: Cell) : Uint8Array;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cell | [Cell](../cell/) | The setting of cell. |
**Returns**
Returns the image data of icon.
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getIconImageData(IconSetType, number) {#getIconImageData-iconsettype-number-}
Get the icon set data
```javascript
static getIconImageData(type: IconSetType, index: number) : Uint8Array;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [IconSetType](../iconsettype/) | icon's type |
| index | number | icon's index |
