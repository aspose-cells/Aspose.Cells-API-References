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
| [getSize()](#getSize--)| <b>@deprecated.</b> Please use the 'size' property instead. Number of rows or columns in a single band of striping. Applies only when type is firstRowStripe, secondRowStripe, firstColumnStripe, or secondColumnStripe. |
| [setSize(number)](#setSize-number-)| <b>@deprecated.</b> Please use the 'size' property instead. Number of rows or columns in a single band of striping. Applies only when type is firstRowStripe, secondRowStripe, firstColumnStripe, or secondColumnStripe. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets the element type. |
| [getElementStyle()](#getElementStyle--)| Gets the element style. |
| [setElementStyle(Style)](#setElementStyle-style-)| Sets the element style. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getSize() {#getSize--}
```javascript
getSize() : number;
```
### setSize(number) {#setSize-number-}
```javascript
setSize(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getType() {#getType--}
```javascript
getType() : TableStyleElementType;
```
**Returns**
[TableStyleElementType](../tablestyleelementtype/)
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
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
