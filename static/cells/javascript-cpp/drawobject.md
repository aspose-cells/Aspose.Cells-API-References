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
