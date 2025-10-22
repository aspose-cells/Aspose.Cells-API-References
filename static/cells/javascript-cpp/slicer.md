##Slicer
summary description of Slicer View
## Slicer class
summary description of Slicer View
```javascript
class Slicer;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [title](#title--)| string | Specifies the title of the current Slicer object. |
| [alternativeText](#alternativeText--)| string | Returns or sets the descriptive (alternative) text string of the Slicer object. |
| [isPrintable](#isPrintable--)| boolean | Indicates whether the slicer object is printable. |
| [isLocked](#isLocked--)| boolean | Indicates whether the slicer shape is locked. |
| [placement](#placement--)| PlacementType | Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. |
| [lockedAspectRatio](#lockedAspectRatio--)| boolean | Indicates whether locking aspect ratio. |
| [lockedPosition](#lockedPosition--)| boolean | Indicates whether the specified slicer can be moved or resized by using the user interface. |
| [shape](#shape--)| SlicerShape | Readonly. Returns the Shape object associated with the specified slicer. Read-only. |
| [slicerCache](#slicerCache--)| SlicerCache | Readonly. Returns the SlicerCache object associated with the slicer. Read-only. |
| [parent](#parent--)| Worksheet | Readonly. Returns the [Worksheet](../worksheet/) object which contains this slicer. Read-only. |
| [styleType](#styleType--)| SlicerStyleType | Specify the type of Built-in slicer style the default type is SlicerStyleLight1 |
| [name](#name--)| string | Returns or sets the name of the specified slicer |
| [caption](#caption--)| string | Returns or sets the caption of the specified slicer. |
| [captionVisible](#captionVisible--)| boolean | Returns or sets whether the header that displays the slicer Caption is visible the default value is true |
| [numberOfColumns](#numberOfColumns--)| number | Returns or sets the number of columns in the specified slicer. |
| [leftPixel](#leftPixel--)| number | Returns or sets the horizontal offset of slicer shape from its left column, in pixels. |
| [topPixel](#topPixel--)| number | Returns or sets the vertical offset of slicer shape from its top row, in pixels. |
| [width](#width--)| number | Returns or sets the width of the specified slicer, in points. |
| [widthPixel](#widthPixel--)| number | Returns or sets the width of the specified slicer, in pixels. |
| [height](#height--)| number | Returns or sets the height of the specified slicer, in points. |
| [heightPixel](#heightPixel--)| number | Returns or sets the height of the specified slicer, in pixels. |
| [columnWidthPixel](#columnWidthPixel--)| number | Gets or sets the width of each column in the slicer, in unit of pixels. |
| [columnWidth](#columnWidth--)| number | Returns or sets the width, in points, of each column in the slicer. |
| [rowHeightPixel](#rowHeightPixel--)| number | Returns or sets the height, in pixels, of each row in the specified slicer. |
| [rowHeight](#rowHeight--)| number | Returns or sets the height, in points, of each row in the specified slicer. |
## Methods
| Method | Description |
| --- | --- |
| [addPivotConnection(PivotTable)](#addPivotConnection-pivottable-)| Adds PivotTable connection. |
| [removePivotConnection(PivotTable)](#removePivotConnection-pivottable-)| Removes PivotTable connection. |
| [refresh()](#refresh--)| Refreshing the slicer.Meanwhile, Refreshing and Calculating  relative PivotTables. |
### title {#title--}
Specifies the title of the current Slicer object.
```javascript
title : string;
```
### alternativeText {#alternativeText--}
Returns or sets the descriptive (alternative) text string of the Slicer object.
```javascript
alternativeText : string;
```
### isPrintable {#isPrintable--}
Indicates whether the slicer object is printable.
```javascript
isPrintable : boolean;
```
### isLocked {#isLocked--}
Indicates whether the slicer shape is locked.
```javascript
isLocked : boolean;
```
### placement {#placement--}
Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.
```javascript
placement : PlacementType;
```
### lockedAspectRatio {#lockedAspectRatio--}
Indicates whether locking aspect ratio.
```javascript
lockedAspectRatio : boolean;
```
### lockedPosition {#lockedPosition--}
Indicates whether the specified slicer can be moved or resized by using the user interface.
```javascript
lockedPosition : boolean;
```
### shape {#shape--}
Readonly. Returns the Shape object associated with the specified slicer. Read-only.
```javascript
shape : SlicerShape;
```
### slicerCache {#slicerCache--}
Readonly. Returns the SlicerCache object associated with the slicer. Read-only.
```javascript
slicerCache : SlicerCache;
```
### parent {#parent--}
Readonly. Returns the [Worksheet](../worksheet/) object which contains this slicer. Read-only.
```javascript
parent : Worksheet;
```
### styleType {#styleType--}
Specify the type of Built-in slicer style the default type is SlicerStyleLight1
```javascript
styleType : SlicerStyleType;
```
### name {#name--}
Returns or sets the name of the specified slicer
```javascript
name : string;
```
### caption {#caption--}
Returns or sets the caption of the specified slicer.
```javascript
caption : string;
```
### captionVisible {#captionVisible--}
Returns or sets whether the header that displays the slicer Caption is visible the default value is true
```javascript
captionVisible : boolean;
```
### numberOfColumns {#numberOfColumns--}
Returns or sets the number of columns in the specified slicer.
```javascript
numberOfColumns : number;
```
### leftPixel {#leftPixel--}
Returns or sets the horizontal offset of slicer shape from its left column, in pixels.
```javascript
leftPixel : number;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Left property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### topPixel {#topPixel--}
Returns or sets the vertical offset of slicer shape from its top row, in pixels.
```javascript
topPixel : number;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Top property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### width {#width--}
Returns or sets the width of the specified slicer, in points.
```javascript
width : number;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.WidthPt property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### widthPixel {#widthPixel--}
Returns or sets the width of the specified slicer, in pixels.
```javascript
widthPixel : number;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Width property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### height {#height--}
Returns or sets the height of the specified slicer, in points.
```javascript
height : number;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.HeightPt property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### heightPixel {#heightPixel--}
Returns or sets the height of the specified slicer, in pixels.
```javascript
heightPixel : number;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Height property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### columnWidthPixel {#columnWidthPixel--}
Gets or sets the width of each column in the slicer, in unit of pixels.
```javascript
columnWidthPixel : number;
```
### columnWidth {#columnWidth--}
Returns or sets the width, in points, of each column in the slicer.
```javascript
columnWidth : number;
```
### rowHeightPixel {#rowHeightPixel--}
Returns or sets the height, in pixels, of each row in the specified slicer.
```javascript
rowHeightPixel : number;
```
### rowHeight {#rowHeight--}
Returns or sets the height, in points, of each row in the specified slicer.
```javascript
rowHeight : number;
```
### addPivotConnection(PivotTable) {#addPivotConnection-pivottable-}
Adds PivotTable connection.
```javascript
addPivotConnection(pivot: PivotTable) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../pivottable/) | The PivotTable object |
### removePivotConnection(PivotTable) {#removePivotConnection-pivottable-}
Removes PivotTable connection.
```javascript
removePivotConnection(pivot: PivotTable) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../pivottable/) | The PivotTable object |
### refresh() {#refresh--}
Refreshing the slicer.Meanwhile, Refreshing and Calculating  relative PivotTables.
```javascript
refresh() : void;
```
