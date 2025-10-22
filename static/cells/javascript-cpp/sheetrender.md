##SheetRender
Represents a worksheet render which can render worksheet to various images such as BMP PNG JPEG TIFF.. The constructor of this class  must be used after modification of pagesetup cell style.
## SheetRender class
Represents a worksheet render which can render worksheet to various images such as (BMP, PNG, JPEG, TIFF..) The constructor of this class , must be used after modification of pagesetup, cell style.
```javascript
class SheetRender;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(Worksheet, ImageOrPrintOptions)](#constructor-worksheet-imageorprintoptions-)| the construct of SheetRender, need worksheet and ImageOrPrintOptions as params |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [pageCount](#pageCount--)| number | Readonly. Gets the total page count of current worksheet. |
| [pageScale](#pageScale--)| number | Readonly. Gets calculated page scale of the sheet. Returns the set scale if [PageSetup.Zoom](../pagesetup.zoom/) is set. Otherwise, returns the calculated scale according to [PageSetup.FitToPagesWide](../pagesetup.fittopageswide/) and [PageSetup.FitToPagesTall](../pagesetup.fittopagestall/). |
## Methods
| Method | Description |
| --- | --- |
| [getPageSizeInch(number)](#getPageSizeInch-number-)| Get page size in inch of output image. |
| [toImageAsync(number, string)](#toImageAsync-number-string-)| Render certain page to a file. |
| [toImageAsync(number)](#toImageAsync-number-)| Render certain page to a stream. |
| [toImage(number, string)](#toImage-number-string-)| Render certain page to a file. |
| [toImage(number)](#toImage-number-)| Render certain page to a stream. |
| [toTiffAsync()](#toTiffAsync--)| Render whole worksheet as Tiff Image to stream. |
| [toTiffAsync(string)](#toTiffAsync-string-)| Render whole worksheet as Tiff Image to a file. |
| [toTiff()](#toTiff--)| Render whole worksheet as Tiff Image to stream. |
| [toTiff(string)](#toTiff-string-)| Render whole worksheet as Tiff Image to a file. |
| [dispose()](#dispose--)| Releases resources created and used for rendering. |
### constructor(Worksheet, ImageOrPrintOptions) {#constructor-worksheet-imageorprintoptions-}
the construct of SheetRender, need worksheet and ImageOrPrintOptions as params
```javascript
constructor(worksheet: Worksheet, options: ImageOrPrintOptions);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| worksheet | [Worksheet](../worksheet/) | Indicate which spreadsheet to be rendered. |
| options | [ImageOrPrintOptions](../imageorprintoptions/) | ImageOrPrintOptions contains some property of output image |
### pageCount {#pageCount--}
Readonly. Gets the total page count of current worksheet.
```javascript
pageCount : number;
```
### pageScale {#pageScale--}
Readonly. Gets calculated page scale of the sheet. Returns the set scale if [PageSetup.Zoom](../pagesetup.zoom/) is set. Otherwise, returns the calculated scale according to [PageSetup.FitToPagesWide](../pagesetup.fittopageswide/) and [PageSetup.FitToPagesTall](../pagesetup.fittopagestall/).
```javascript
pageScale : number;
```
### getPageSizeInch(number) {#getPageSizeInch-number-}
Get page size in inch of output image.
```javascript
getPageSizeInch(pageIndex: number) : number[];
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | number | The page index is based on zero. |
**Returns**
Page size of image, [0] for width and [1] for height
### toImageAsync(number, string) {#toImageAsync-number-string-}
Render certain page to a file.
```javascript
toImageAsync(pageIndex: number, fileName: string) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | number | indicate which page is to be converted |
| fileName | string | filename of the output image |
**Returns**
[Promise<void>](../promise<void>/)
### toImageAsync(number) {#toImageAsync-number-}
Render certain page to a stream.
```javascript
toImageAsync(pageIndex: number) : Promise<Uint8Array>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | number | indicate which page is to be converted |
**Returns**
The result stream
### toImage(number, string) {#toImage-number-string-}
Render certain page to a file.
```javascript
toImage(pageIndex: number, fileName: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | number | indicate which page is to be converted |
| fileName | string | filename of the output image |
### toImage(number) {#toImage-number-}
Render certain page to a stream.
```javascript
toImage(pageIndex: number) : Uint8Array;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | number | indicate which page is to be converted |
**Returns**
The result stream
### toTiffAsync() {#toTiffAsync--}
Render whole worksheet as Tiff Image to stream.
```javascript
toTiffAsync() : Promise<Uint8Array>;
```
**Returns**
The result stream
### toTiffAsync(string) {#toTiffAsync-string-}
Render whole worksheet as Tiff Image to a file.
```javascript
toTiffAsync(filename: string) : Promise<void>;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | string | the filename of the output image |
**Returns**
[Promise<void>](../promise<void>/)
### toTiff() {#toTiff--}
Render whole worksheet as Tiff Image to stream.
```javascript
toTiff() : Uint8Array;
```
**Returns**
The result stream
### toTiff(string) {#toTiff-string-}
Render whole worksheet as Tiff Image to a file.
```javascript
toTiff(filename: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | string | the filename of the output image |
### dispose() {#dispose--}
Releases resources created and used for rendering.
```javascript
dispose() : void;
```
