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
| [toImage(string, ImageOrPrintOptions)](#toImage-string-imageorprintoptions-)| Converts a sparkline to an image. |
| [toImage(ImageOrPrintOptions)](#toImage-imageorprintoptions-)| Converts a sparkline to an image. |
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
