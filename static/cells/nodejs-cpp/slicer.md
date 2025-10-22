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
| [getTitle()](#getTitle--)| <b>@deprecated.</b> Please use the 'title' property instead. Specifies the title of the current Slicer object. |
| [setTitle(string)](#setTitle-string-)| <b>@deprecated.</b> Please use the 'title' property instead. Specifies the title of the current Slicer object. |
| [getAlternativeText()](#getAlternativeText--)| <b>@deprecated.</b> Please use the 'alternativeText' property instead. Returns or sets the descriptive (alternative) text string of the Slicer object. |
| [setAlternativeText(string)](#setAlternativeText-string-)| <b>@deprecated.</b> Please use the 'alternativeText' property instead. Returns or sets the descriptive (alternative) text string of the Slicer object. |
| [isPrintable()](#isPrintable--)| <b>@deprecated.</b> Please use the 'isPrintable' property instead. Indicates whether the slicer object is printable. |
| [setIsPrintable(boolean)](#setIsPrintable-boolean-)| <b>@deprecated.</b> Please use the 'isPrintable' property instead. Indicates whether the slicer object is printable. |
| [isLocked()](#isLocked--)| <b>@deprecated.</b> Please use the 'isLocked' property instead. Indicates whether the slicer shape is locked. |
| [setIsLocked(boolean)](#setIsLocked-boolean-)| <b>@deprecated.</b> Please use the 'isLocked' property instead. Indicates whether the slicer shape is locked. |
| [getPlacement()](#getPlacement--)| <b>@deprecated.</b> Please use the 'placement' property instead. Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. |
| [setPlacement(PlacementType)](#setPlacement-placementtype-)| <b>@deprecated.</b> Please use the 'placement' property instead. Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. |
| [getLockedAspectRatio()](#getLockedAspectRatio--)| <b>@deprecated.</b> Please use the 'lockedAspectRatio' property instead. Indicates whether locking aspect ratio. |
| [setLockedAspectRatio(boolean)](#setLockedAspectRatio-boolean-)| <b>@deprecated.</b> Please use the 'lockedAspectRatio' property instead. Indicates whether locking aspect ratio. |
| [getLockedPosition()](#getLockedPosition--)| <b>@deprecated.</b> Please use the 'lockedPosition' property instead. Indicates whether the specified slicer can be moved or resized by using the user interface. |
| [setLockedPosition(boolean)](#setLockedPosition-boolean-)| <b>@deprecated.</b> Please use the 'lockedPosition' property instead. Indicates whether the specified slicer can be moved or resized by using the user interface. |
| [getShape()](#getShape--)| <b>@deprecated.</b> Please use the 'shape' property instead. Returns the Shape object associated with the specified slicer. Read-only. |
| [getSlicerCache()](#getSlicerCache--)| <b>@deprecated.</b> Please use the 'slicerCache' property instead. Returns the SlicerCache object associated with the slicer. Read-only. |
| [getParent()](#getParent--)| <b>@deprecated.</b> Please use the 'parent' property instead. Returns the [Worksheet](../worksheet/) object which contains this slicer. Read-only. |
| [getStyleType()](#getStyleType--)| <b>@deprecated.</b> Please use the 'styleType' property instead. Specify the type of Built-in slicer style the default type is SlicerStyleLight1 |
| [setStyleType(SlicerStyleType)](#setStyleType-slicerstyletype-)| <b>@deprecated.</b> Please use the 'styleType' property instead. Specify the type of Built-in slicer style the default type is SlicerStyleLight1 |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Returns or sets the name of the specified slicer |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Returns or sets the name of the specified slicer |
| [getCaption()](#getCaption--)| <b>@deprecated.</b> Please use the 'caption' property instead. Returns or sets the caption of the specified slicer. |
| [setCaption(string)](#setCaption-string-)| <b>@deprecated.</b> Please use the 'caption' property instead. Returns or sets the caption of the specified slicer. |
| [getCaptionVisible()](#getCaptionVisible--)| <b>@deprecated.</b> Please use the 'captionVisible' property instead. Returns or sets whether the header that displays the slicer Caption is visible the default value is true |
| [setCaptionVisible(boolean)](#setCaptionVisible-boolean-)| <b>@deprecated.</b> Please use the 'captionVisible' property instead. Returns or sets whether the header that displays the slicer Caption is visible the default value is true |
| [getNumberOfColumns()](#getNumberOfColumns--)| <b>@deprecated.</b> Please use the 'numberOfColumns' property instead. Returns or sets the number of columns in the specified slicer. |
| [setNumberOfColumns(number)](#setNumberOfColumns-number-)| <b>@deprecated.</b> Please use the 'numberOfColumns' property instead. Returns or sets the number of columns in the specified slicer. |
| [getLeftPixel()](#getLeftPixel--)| <b>@deprecated.</b> Please use the 'leftPixel' property instead. Returns or sets the horizontal offset of slicer shape from its left column, in pixels. |
| [setLeftPixel(number)](#setLeftPixel-number-)| <b>@deprecated.</b> Please use the 'leftPixel' property instead. Returns or sets the horizontal offset of slicer shape from its left column, in pixels. |
| [getTopPixel()](#getTopPixel--)| <b>@deprecated.</b> Please use the 'topPixel' property instead. Returns or sets the vertical offset of slicer shape from its top row, in pixels. |
| [setTopPixel(number)](#setTopPixel-number-)| <b>@deprecated.</b> Please use the 'topPixel' property instead. Returns or sets the vertical offset of slicer shape from its top row, in pixels. |
| [getWidth()](#getWidth--)| <b>@deprecated.</b> Please use the 'width' property instead. Returns or sets the width of the specified slicer, in points. |
| [setWidth(number)](#setWidth-number-)| <b>@deprecated.</b> Please use the 'width' property instead. Returns or sets the width of the specified slicer, in points. |
| [getWidthPixel()](#getWidthPixel--)| <b>@deprecated.</b> Please use the 'widthPixel' property instead. Returns or sets the width of the specified slicer, in pixels. |
| [setWidthPixel(number)](#setWidthPixel-number-)| <b>@deprecated.</b> Please use the 'widthPixel' property instead. Returns or sets the width of the specified slicer, in pixels. |
| [getHeight()](#getHeight--)| <b>@deprecated.</b> Please use the 'height' property instead. Returns or sets the height of the specified slicer, in points. |
| [setHeight(number)](#setHeight-number-)| <b>@deprecated.</b> Please use the 'height' property instead. Returns or sets the height of the specified slicer, in points. |
| [getHeightPixel()](#getHeightPixel--)| <b>@deprecated.</b> Please use the 'heightPixel' property instead. Returns or sets the height of the specified slicer, in pixels. |
| [setHeightPixel(number)](#setHeightPixel-number-)| <b>@deprecated.</b> Please use the 'heightPixel' property instead. Returns or sets the height of the specified slicer, in pixels. |
| [getColumnWidthPixel()](#getColumnWidthPixel--)| <b>@deprecated.</b> Please use the 'columnWidthPixel' property instead. Gets or sets the width of each column in the slicer, in unit of pixels. |
| [setColumnWidthPixel(number)](#setColumnWidthPixel-number-)| <b>@deprecated.</b> Please use the 'columnWidthPixel' property instead. Gets or sets the width of each column in the slicer, in unit of pixels. |
| [getColumnWidth()](#getColumnWidth--)| <b>@deprecated.</b> Please use the 'columnWidth' property instead. Returns or sets the width, in points, of each column in the slicer. |
| [setColumnWidth(number)](#setColumnWidth-number-)| <b>@deprecated.</b> Please use the 'columnWidth' property instead. Returns or sets the width, in points, of each column in the slicer. |
| [getRowHeightPixel()](#getRowHeightPixel--)| <b>@deprecated.</b> Please use the 'rowHeightPixel' property instead. Returns or sets the height, in pixels, of each row in the specified slicer. |
| [setRowHeightPixel(number)](#setRowHeightPixel-number-)| <b>@deprecated.</b> Please use the 'rowHeightPixel' property instead. Returns or sets the height, in pixels, of each row in the specified slicer. |
| [getRowHeight()](#getRowHeight--)| <b>@deprecated.</b> Please use the 'rowHeight' property instead. Returns or sets the height, in points, of each row in the specified slicer. |
| [setRowHeight(number)](#setRowHeight-number-)| <b>@deprecated.</b> Please use the 'rowHeight' property instead. Returns or sets the height, in points, of each row in the specified slicer. |
| [addPivotConnection(PivotTable)](#addPivotConnection-pivottable-)| Adds PivotTable connection. |
| [removePivotConnection(PivotTable)](#removePivotConnection-pivottable-)| Removes PivotTable connection. |
| [refresh()](#refresh--)| Refreshing the slicer.Meanwhile, Refreshing and Calculating  relative PivotTables. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getTitle() {#getTitle--}
```javascript
getTitle() : string;
```
### setTitle(string) {#setTitle-string-}
```javascript
setTitle(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getAlternativeText() {#getAlternativeText--}
```javascript
getAlternativeText() : string;
```
### setAlternativeText(string) {#setAlternativeText-string-}
```javascript
setAlternativeText(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### isPrintable() {#isPrintable--}
```javascript
isPrintable() : boolean;
```
### setIsPrintable(boolean) {#setIsPrintable-boolean-}
```javascript
setIsPrintable(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isLocked() {#isLocked--}
```javascript
isLocked() : boolean;
```
### setIsLocked(boolean) {#setIsLocked-boolean-}
```javascript
setIsLocked(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getPlacement() {#getPlacement--}
```javascript
getPlacement() : PlacementType;
```
**Returns**
[PlacementType](../placementtype/)
### setPlacement(PlacementType) {#setPlacement-placementtype-}
```javascript
setPlacement(value: PlacementType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PlacementType](../placementtype/) | The value to set. |
### getLockedAspectRatio() {#getLockedAspectRatio--}
```javascript
getLockedAspectRatio() : boolean;
```
### setLockedAspectRatio(boolean) {#setLockedAspectRatio-boolean-}
```javascript
setLockedAspectRatio(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getLockedPosition() {#getLockedPosition--}
```javascript
getLockedPosition() : boolean;
```
### setLockedPosition(boolean) {#setLockedPosition-boolean-}
```javascript
setLockedPosition(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShape() {#getShape--}
```javascript
getShape() : SlicerShape;
```
**Returns**
[SlicerShape](../slicershape/)
### getSlicerCache() {#getSlicerCache--}
```javascript
getSlicerCache() : SlicerCache;
```
**Returns**
[SlicerCache](../slicercache/)
### getParent() {#getParent--}
```javascript
getParent() : Worksheet;
```
**Returns**
[Worksheet](../worksheet/)
### getStyleType() {#getStyleType--}
```javascript
getStyleType() : SlicerStyleType;
```
**Returns**
[SlicerStyleType](../slicerstyletype/)
### setStyleType(SlicerStyleType) {#setStyleType-slicerstyletype-}
```javascript
setStyleType(value: SlicerStyleType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SlicerStyleType](../slicerstyletype/) | The value to set. |
### getName() {#getName--}
```javascript
getName() : string;
```
### setName(string) {#setName-string-}
```javascript
setName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getCaption() {#getCaption--}
```javascript
getCaption() : string;
```
### setCaption(string) {#setCaption-string-}
```javascript
setCaption(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getCaptionVisible() {#getCaptionVisible--}
```javascript
getCaptionVisible() : boolean;
```
### setCaptionVisible(boolean) {#setCaptionVisible-boolean-}
```javascript
setCaptionVisible(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getNumberOfColumns() {#getNumberOfColumns--}
```javascript
getNumberOfColumns() : number;
```
### setNumberOfColumns(number) {#setNumberOfColumns-number-}
```javascript
setNumberOfColumns(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getLeftPixel() {#getLeftPixel--}
```javascript
getLeftPixel() : number;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Left property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### setLeftPixel(number) {#setLeftPixel-number-}
```javascript
setLeftPixel(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Left property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### getTopPixel() {#getTopPixel--}
```javascript
getTopPixel() : number;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Top property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### setTopPixel(number) {#setTopPixel-number-}
```javascript
setTopPixel(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Top property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### getWidth() {#getWidth--}
```javascript
getWidth() : number;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.WidthPt property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### setWidth(number) {#setWidth-number-}
```javascript
setWidth(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.WidthPt property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### getWidthPixel() {#getWidthPixel--}
```javascript
getWidthPixel() : number;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Width property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### setWidthPixel(number) {#setWidthPixel-number-}
```javascript
setWidthPixel(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Width property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### getHeight() {#getHeight--}
```javascript
getHeight() : number;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.HeightPt property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### setHeight(number) {#setHeight-number-}
```javascript
setHeight(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.HeightPt property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### getHeightPixel() {#getHeightPixel--}
```javascript
getHeightPixel() : number;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Height property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### setHeightPixel(number) {#setHeightPixel-number-}
```javascript
setHeightPixel(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
NOTE: This member is now obsolete. Instead, please use Shape.Height property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### getColumnWidthPixel() {#getColumnWidthPixel--}
```javascript
getColumnWidthPixel() : number;
```
### setColumnWidthPixel(number) {#setColumnWidthPixel-number-}
```javascript
setColumnWidthPixel(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getColumnWidth() {#getColumnWidth--}
```javascript
getColumnWidth() : number;
```
### setColumnWidth(number) {#setColumnWidth-number-}
```javascript
setColumnWidth(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getRowHeightPixel() {#getRowHeightPixel--}
```javascript
getRowHeightPixel() : number;
```
### setRowHeightPixel(number) {#setRowHeightPixel-number-}
```javascript
setRowHeightPixel(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getRowHeight() {#getRowHeight--}
```javascript
getRowHeight() : number;
```
### setRowHeight(number) {#setRowHeight-number-}
```javascript
setRowHeight(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
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
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
