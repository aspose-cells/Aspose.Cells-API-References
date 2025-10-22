##TableStyleElement
Represents the element of the table style.
## TableStyleElement class
Represents the element of the table style.
```javascript
class TableStyleElement;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [size](#size--)| number | Number of rows or columns in a single band of striping. Applies only when type is firstRowStripe, secondRowStripe, firstColumnStripe, or secondColumnStripe. |
| [type](#type--)| TableStyleElementType | Readonly. Gets the element type. |
## Methods
| Method | Description |
| --- | --- |
| [getElementStyle()](#getElementStyle--)| Gets the element style. |
| [setElementStyle(Style)](#setElementStyle-style-)| Sets the element style. |
### size {#size--}
Number of rows or columns in a single band of striping. Applies only when type is firstRowStripe, secondRowStripe, firstColumnStripe, or secondColumnStripe.
```javascript
size : number;
```
### type {#type--}
Readonly. Gets the element type.
```javascript
type : TableStyleElementType;
```
### getElementStyle() {#getElementStyle--}
Gets the element style.
```javascript
getElementStyle() : Style;
```
**Returns**
Returns the [Style](../style/) object.
### setElementStyle(Style) {#setElementStyle-style-}
Sets the element style.
```javascript
setElementStyle(style: Style) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) | The element style. |
