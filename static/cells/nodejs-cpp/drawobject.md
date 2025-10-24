##DrawObject
DrawObject will be initialized and returned when rendering.
## DrawObject class
DrawObject will be initialized and returned when rendering.
```javascript
class DrawObject;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [cell](#cell--)| Cell | Readonly. Indicates the Cell object when rendering. All properties of cell can be accessed. |
| [shape](#shape--)| Shape | Readonly. Indicates the Shape object when rendering. All properties of shape can be accessed. |
| [imageBytes](#imageBytes--)| Uint8Array | Readonly. Indicates image bytes of rendered Chart, Shape when rendering. |
| [type](#type--)| DrawObjectEnum | Readonly. Indicates the type of DrawObject. |
| [currentPage](#currentPage--)| number | Readonly. Indicates the page index of DrawObject. Page index is based on zero. One Sheet contains several pages when rendering. |
| [totalPages](#totalPages--)| number | Readonly. Indicates total pages in current rendering. |
| [sheetIndex](#sheetIndex--)| number | Readonly. Indicates current sheet index of DrawObject. |
## Methods
| Method | Description |
| --- | --- |
| [getCell()](#getCell--)| <b>@deprecated.</b> Please use the 'cell' property instead. Indicates the Cell object when rendering. All properties of cell can be accessed. |
| [getShape()](#getShape--)| <b>@deprecated.</b> Please use the 'shape' property instead. Indicates the Shape object when rendering. All properties of shape can be accessed. |
| [getImageBytes()](#getImageBytes--)| <b>@deprecated.</b> Please use the 'imageBytes' property instead. Indicates image bytes of rendered Chart, Shape when rendering. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Indicates the type of DrawObject. |
| [getCurrentPage()](#getCurrentPage--)| <b>@deprecated.</b> Please use the 'currentPage' property instead. Indicates the page index of DrawObject. Page index is based on zero. One Sheet contains several pages when rendering. |
| [getTotalPages()](#getTotalPages--)| <b>@deprecated.</b> Please use the 'totalPages' property instead. Indicates total pages in current rendering. |
| [getSheetIndex()](#getSheetIndex--)| <b>@deprecated.</b> Please use the 'sheetIndex' property instead. Indicates current sheet index of DrawObject. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### cell {#cell--}
Readonly. Indicates the Cell object when rendering. All properties of cell can be accessed.
```javascript
cell : Cell;
```
### shape {#shape--}
Readonly. Indicates the Shape object when rendering. All properties of shape can be accessed.
```javascript
shape : Shape;
```
### imageBytes {#imageBytes--}
Readonly. Indicates image bytes of rendered Chart, Shape when rendering.
```javascript
imageBytes : Uint8Array;
```
### type {#type--}
Readonly. Indicates the type of DrawObject.
```javascript
type : DrawObjectEnum;
```
### currentPage {#currentPage--}
Readonly. Indicates the page index of DrawObject. Page index is based on zero. One Sheet contains several pages when rendering.
```javascript
currentPage : number;
```
### totalPages {#totalPages--}
Readonly. Indicates total pages in current rendering.
```javascript
totalPages : number;
```
### sheetIndex {#sheetIndex--}
Readonly. Indicates current sheet index of DrawObject.
```javascript
sheetIndex : number;
```
### getCell() {#getCell--}
```javascript
getCell() : Cell;
```
**Returns**
[Cell](../cell/)
### getShape() {#getShape--}
```javascript
getShape() : Shape;
```
**Returns**
[Shape](../shape/)
### getImageBytes() {#getImageBytes--}
```javascript
getImageBytes() : Uint8Array;
```
### getType() {#getType--}
```javascript
getType() : DrawObjectEnum;
```
**Returns**
[DrawObjectEnum](../drawobjectenum/)
### getCurrentPage() {#getCurrentPage--}
```javascript
getCurrentPage() : number;
```
### getTotalPages() {#getTotalPages--}
```javascript
getTotalPages() : number;
```
### getSheetIndex() {#getSheetIndex--}
```javascript
getSheetIndex() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
