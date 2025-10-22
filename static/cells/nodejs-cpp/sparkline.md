##Sparkline
A sparkline represents a tiny chart or graphic in a worksheet cell that provides a visual representation of data.
## Sparkline class
A sparkline represents a tiny chart or graphic in a worksheet cell that provides a visual representation of data.
```javascript
class Sparkline;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [dataRange](#dataRange--)| string | Represents the data range of the sparkline. |
| [row](#row--)| number | Readonly. Gets the row index of the sparkline. |
| [column](#column--)| number | Readonly. Gets the column index of the sparkline. |
## Methods
| Method | Description |
| --- | --- |
| [getDataRange()](#getDataRange--)| <b>@deprecated.</b> Please use the 'dataRange' property instead. Represents the data range of the sparkline. |
| [setDataRange(string)](#setDataRange-string-)| <b>@deprecated.</b> Please use the 'dataRange' property instead. Represents the data range of the sparkline. |
| [getRow()](#getRow--)| <b>@deprecated.</b> Please use the 'row' property instead. Gets the row index of the sparkline. |
| [getColumn()](#getColumn--)| <b>@deprecated.</b> Please use the 'column' property instead. Gets the column index of the sparkline. |
| [toImage(string, ImageOrPrintOptions)](#toImage-string-imageorprintoptions-)| Converts a sparkline to an image. |
| [toImage(ImageOrPrintOptions)](#toImage-imageorprintoptions-)| Converts a sparkline to an image. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### dataRange {#dataRange--}
Represents the data range of the sparkline.
```javascript
dataRange : string;
```
### row {#row--}
Readonly. Gets the row index of the sparkline.
```javascript
row : number;
```
### column {#column--}
Readonly. Gets the column index of the sparkline.
```javascript
column : number;
```
### getDataRange() {#getDataRange--}
```javascript
getDataRange() : string;
```
### setDataRange(string) {#setDataRange-string-}
```javascript
setDataRange(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getRow() {#getRow--}
```javascript
getRow() : number;
```
### getColumn() {#getColumn--}
```javascript
getColumn() : number;
```
### toImage(string, ImageOrPrintOptions) {#toImage-string-imageorprintoptions-}
Converts a sparkline to an image.
```javascript
toImage(fileName: string, options: ImageOrPrintOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | string | The image file name. |
| options | [ImageOrPrintOptions](../imageorprintoptions/) | The image options |
### toImage(ImageOrPrintOptions) {#toImage-imageorprintoptions-}
Converts a sparkline to an image.
```javascript
toImage(options: ImageOrPrintOptions) : Uint8Array;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../imageorprintoptions/) | The image options. |
**Returns**
The result stream
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
