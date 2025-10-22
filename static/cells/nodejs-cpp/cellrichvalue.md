##CellRichValue
Represents rich value of the cell.
## CellRichValue class
Represents rich value of the cell.
```javascript
class CellRichValue;
```
## Methods
| Method | Description |
| --- | --- |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getErrorValue()](#getErrorValue--)| Gets the error value type of the cell. |
| [getImage()](#getImage--)| Gets the image data of the cell. |
| [getAltText()](#getAltText--)| Gets the alt text associated with the image. |
| [setAltText(string)](#setAltText-string-)| Gets the alt text associated with the image. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getErrorValue() {#getErrorValue--}
Gets the error value type of the cell.
```javascript
getErrorValue() : ErrorCellValueType;
```
**Returns**
[ErrorCellValueType](../errorcellvaluetype/)
### getImage() {#getImage--}
Gets the image data of the cell.
```javascript
getImage() : Uint8Array;
```
### getAltText() {#getAltText--}
Gets the alt text associated with the image.
```javascript
getAltText() : string;
```
### setAltText(string) {#setAltText-string-}
Gets the alt text associated with the image.
```javascript
setAltText(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
