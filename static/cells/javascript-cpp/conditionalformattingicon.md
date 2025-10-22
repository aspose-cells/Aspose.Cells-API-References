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
| [getImageData(Cell)](#getImageData-cell-)| Gets the image data with the setting of cell. |
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
