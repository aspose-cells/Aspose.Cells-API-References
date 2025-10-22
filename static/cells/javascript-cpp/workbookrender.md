##WorkbookRender
Represents a Workbook render. The constructor of this class  must be used after modification of pagesetup cell style.
## WorkbookRender class
Represents a Workbook render. The constructor of this class , must be used after modification of pagesetup, cell style.
```javascript
class WorkbookRender;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(Workbook, ImageOrPrintOptions)](#constructor-workbook-imageorprintoptions-)| The construct of WorkbookRender |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [pageCount](#pageCount--)| number | Readonly. Gets the total page count of workbook. |
## Methods
| Method | Description |
| --- | --- |
| [getPageSizeInch(number)](#getPageSizeInch-number-)| Get page size in inch of output image. |
| [toImage()](#toImage--)| Render whole workbook as Tiff Image to stream. |
| [toImage(string)](#toImage-string-)| Render whole workbook as Tiff Image to a file. |
| [toImage(number, string)](#toImage-number-string-)| Render certain page to a file. |
| [toImage(number)](#toImage-number-)| Render certain page to a stream. |
| [dispose()](#dispose--)| Releases resources created and used for rendering. |
### constructor(Workbook, ImageOrPrintOptions) {#constructor-workbook-imageorprintoptions-}
The construct of WorkbookRender
```javascript
constructor(workbook: Workbook, options: ImageOrPrintOptions);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| workbook | [Workbook](../workbook/) | Indicate which workbook to be rendered. |
| options | [ImageOrPrintOptions](../imageorprintoptions/) | ImageOrPrintOptions contains some property of output image |
### pageCount {#pageCount--}
Readonly. Gets the total page count of workbook.
```javascript
pageCount : number;
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
### toImage() {#toImage--}
Render whole workbook as Tiff Image to stream.
```javascript
toImage() : Uint8Array;
```
**Returns**
The result stream
### toImage(string) {#toImage-string-}
Render whole workbook as Tiff Image to a file.
```javascript
toImage(filename: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | string | the filename of the output image |
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
### dispose() {#dispose--}
Releases resources created and used for rendering.
```javascript
dispose() : void;
```
