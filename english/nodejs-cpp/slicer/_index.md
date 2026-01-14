---
title: Slicer
second_title: Aspose.Cells for Node.js via C++ API Reference
description: summary description of Slicer View
type: docs
url: /nodejs-cpp/slicer/
---

## Slicer class

summary description of Slicer View

```javascript
class Slicer;
```


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [sortOrderType](#sortOrderType--)| SortOrder | Indicates the type of sorting items. |
| [showMissing](#showMissing--)| boolean | Indicates whether to show items deteleted from the data source. |
| [showTypeOfItemsWithNoData](#showTypeOfItemsWithNoData--)| ItemsWithNoDataShowMode | Indicates whether to show items deteleted from the data source. |
| [showAllItems](#showAllItems--)| boolean | Indicates whether to show all items even if there are no data or they are deleted. Default value is true; |
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
| [worksheet](#worksheet--)| Worksheet | Readonly. Returns the [Worksheet](../worksheet/) object which contains this slicer. Read-only. |
| [styleType](#styleType--)| SlicerStyleType | Specify the type of Built-in slicer style. The default type is SlicerStyleLight1. |
| [name](#name--)| string | Returns or sets the name of the specified slicer |
| [caption](#caption--)| string | Returns or sets the caption of the specified slicer. |
| [firstItemIndex](#firstItemIndex--)| number | Specifies the zero-based index of the first slicer item. |
| [captionVisible](#captionVisible--)| boolean | Returns or sets whether the header that displays the slicer Caption is visible. The default value is true |
| [showCaption](#showCaption--)| boolean | Indicates whether the header of the slicer is visible. The default value is true |
| [numberOfColumns](#numberOfColumns--)| number | Returns or sets the number of columns in the specified slicer. The default value is 1. |
| [leftPixel](#leftPixel--)| number | Returns or sets the horizontal offset of slicer shape from its left column, in pixels. |
| [topPixel](#topPixel--)| number | Returns or sets the vertical offset of slicer shape from its top row, in pixels. |
| [width](#width--)| number | Returns or sets the width of the specified slicer, in points. |
| [widthPixel](#widthPixel--)| number | Returns or sets the width of the specified slicer, in pixels. |
| [height](#height--)| number | Returns or sets the height of the specified slicer, in points. |
| [heightPixel](#heightPixel--)| number | Returns or sets the height of the specified slicer, in pixels. |
| [columnWidthPixel](#columnWidthPixel--)| number | Gets or sets the width of each column in the slicer, in unit of pixels. |
| [columnWidth](#columnWidth--)| number | Returns or sets the width of each column in the slicer in unit of points. |
| [rowHeightPixel](#rowHeightPixel--)| number | Returns or sets the height of each row in the specified slicer, in unit of pixels. |
| [rowHeight](#rowHeight--)| number | Returns or sets the height of each row in the specified slicer in unit of points. |

## Methods

| Method | Description |
| --- | --- |
| [getSortOrderType()](#getSortOrderType--)| <b>@deprecated.</b> Please use the 'sortOrderType' property instead. Indicates the type of sorting items. |
| [setSortOrderType(SortOrder)](#setSortOrderType-sortorder-)| <b>@deprecated.</b> Please use the 'sortOrderType' property instead. Indicates the type of sorting items. |
| [getShowMissing()](#getShowMissing--)| <b>@deprecated.</b> Please use the 'showMissing' property instead. Indicates whether to show items deteleted from the data source. |
| [setShowMissing(boolean)](#setShowMissing-boolean-)| <b>@deprecated.</b> Please use the 'showMissing' property instead. Indicates whether to show items deteleted from the data source. |
| [getShowTypeOfItemsWithNoData()](#getShowTypeOfItemsWithNoData--)| <b>@deprecated.</b> Please use the 'showTypeOfItemsWithNoData' property instead. Indicates whether to show items deteleted from the data source. |
| [setShowTypeOfItemsWithNoData(ItemsWithNoDataShowMode)](#setShowTypeOfItemsWithNoData-itemswithnodatashowmode-)| <b>@deprecated.</b> Please use the 'showTypeOfItemsWithNoData' property instead. Indicates whether to show items deteleted from the data source. |
| [getShowAllItems()](#getShowAllItems--)| <b>@deprecated.</b> Please use the 'showAllItems' property instead. Indicates whether to show all items even if there are no data or they are deleted. Default value is true; |
| [setShowAllItems(boolean)](#setShowAllItems-boolean-)| <b>@deprecated.</b> Please use the 'showAllItems' property instead. Indicates whether to show all items even if there are no data or they are deleted. Default value is true; |
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
| [getWorksheet()](#getWorksheet--)| <b>@deprecated.</b> Please use the 'worksheet' property instead. Returns the [Worksheet](../worksheet/) object which contains this slicer. Read-only. |
| [getStyleType()](#getStyleType--)| <b>@deprecated.</b> Please use the 'styleType' property instead. Specify the type of Built-in slicer style. The default type is SlicerStyleLight1. |
| [setStyleType(SlicerStyleType)](#setStyleType-slicerstyletype-)| <b>@deprecated.</b> Please use the 'styleType' property instead. Specify the type of Built-in slicer style. The default type is SlicerStyleLight1. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Returns or sets the name of the specified slicer |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Returns or sets the name of the specified slicer |
| [getCaption()](#getCaption--)| <b>@deprecated.</b> Please use the 'caption' property instead. Returns or sets the caption of the specified slicer. |
| [setCaption(string)](#setCaption-string-)| <b>@deprecated.</b> Please use the 'caption' property instead. Returns or sets the caption of the specified slicer. |
| [getFirstItemIndex()](#getFirstItemIndex--)| <b>@deprecated.</b> Please use the 'firstItemIndex' property instead. Specifies the zero-based index of the first slicer item. |
| [setFirstItemIndex(number)](#setFirstItemIndex-number-)| <b>@deprecated.</b> Please use the 'firstItemIndex' property instead. Specifies the zero-based index of the first slicer item. |
| [getCaptionVisible()](#getCaptionVisible--)| <b>@deprecated.</b> Please use the 'captionVisible' property instead. Returns or sets whether the header that displays the slicer Caption is visible. The default value is true |
| [setCaptionVisible(boolean)](#setCaptionVisible-boolean-)| <b>@deprecated.</b> Please use the 'captionVisible' property instead. Returns or sets whether the header that displays the slicer Caption is visible. The default value is true |
| [getShowCaption()](#getShowCaption--)| <b>@deprecated.</b> Please use the 'showCaption' property instead. Indicates whether the header of the slicer is visible. The default value is true |
| [setShowCaption(boolean)](#setShowCaption-boolean-)| <b>@deprecated.</b> Please use the 'showCaption' property instead. Indicates whether the header of the slicer is visible. The default value is true |
| [getNumberOfColumns()](#getNumberOfColumns--)| <b>@deprecated.</b> Please use the 'numberOfColumns' property instead. Returns or sets the number of columns in the specified slicer. The default value is 1. |
| [setNumberOfColumns(number)](#setNumberOfColumns-number-)| <b>@deprecated.</b> Please use the 'numberOfColumns' property instead. Returns or sets the number of columns in the specified slicer. The default value is 1. |
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
| [getColumnWidth()](#getColumnWidth--)| <b>@deprecated.</b> Please use the 'columnWidth' property instead. Returns or sets the width of each column in the slicer in unit of points. |
| [setColumnWidth(number)](#setColumnWidth-number-)| <b>@deprecated.</b> Please use the 'columnWidth' property instead. Returns or sets the width of each column in the slicer in unit of points. |
| [getRowHeightPixel()](#getRowHeightPixel--)| <b>@deprecated.</b> Please use the 'rowHeightPixel' property instead. Returns or sets the height of each row in the specified slicer, in unit of pixels. |
| [setRowHeightPixel(number)](#setRowHeightPixel-number-)| <b>@deprecated.</b> Please use the 'rowHeightPixel' property instead. Returns or sets the height of each row in the specified slicer, in unit of pixels. |
| [getRowHeight()](#getRowHeight--)| <b>@deprecated.</b> Please use the 'rowHeight' property instead. Returns or sets the height of each row in the specified slicer in unit of points. |
| [setRowHeight(number)](#setRowHeight-number-)| <b>@deprecated.</b> Please use the 'rowHeight' property instead. Returns or sets the height of each row in the specified slicer in unit of points. |
| [addPivotConnection(PivotTable)](#addPivotConnection-pivottable-)| Adds PivotTable connection. |
| [removePivotConnection(PivotTable)](#removePivotConnection-pivottable-)| Removes PivotTable connection. |
| [refresh()](#refresh--)| Refreshing the slicer. Meanwhile, Refreshing and Calculating PivotTables which this slicer based on. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### sortOrderType {#sortOrderType--}

Indicates the type of sorting items.

```javascript
sortOrderType : SortOrder;
```


### showMissing {#showMissing--}

Indicates whether to show items deteleted from the data source.

```javascript
showMissing : boolean;
```


**Remarks**

Only works when [Slicer.ShowAllItems](../slicer.showallitems/) is true.

### showTypeOfItemsWithNoData {#showTypeOfItemsWithNoData--}

Indicates whether to show items deteleted from the data source.

```javascript
showTypeOfItemsWithNoData : ItemsWithNoDataShowMode;
```


**Remarks**

Only works when [Slicer.ShowAllItems](../slicer.showallitems/) is true.

### showAllItems {#showAllItems--}

Indicates whether to show all items even if there are no data or they are deleted. Default value is true;

```javascript
showAllItems : boolean;
```


### title {#title--}

Specifies the title of the current Slicer object.

```javascript
title : string;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use [Shape.Title](../shape.title/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### alternativeText {#alternativeText--}

Returns or sets the descriptive (alternative) text string of the Slicer object.

```javascript
alternativeText : string;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use [Shape.AlternativeText](../shape.alternativetext/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### isPrintable {#isPrintable--}

Indicates whether the slicer object is printable.

```javascript
isPrintable : boolean;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use [Shape.IsPrintable](../shape.isprintable/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### isLocked {#isLocked--}

Indicates whether the slicer shape is locked.

```javascript
isLocked : boolean;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use [Shape.IsLocked](../shape.islocked/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### placement {#placement--}

Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.

```javascript
placement : PlacementType;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use [Shape.Placement](../shape.placement/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### lockedAspectRatio {#lockedAspectRatio--}

Indicates whether locking aspect ratio.

```javascript
lockedAspectRatio : boolean;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use [Shape.GetLockedProperty()](../shape.getlockedproperty()/) method. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

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


**Remarks**

NOTE: This member is now obsolete. Instead, please use [Slicer.Worksheet](../slicer.worksheet/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### worksheet {#worksheet--}

Readonly. Returns the [Worksheet](../worksheet/) object which contains this slicer. Read-only.

```javascript
worksheet : Worksheet;
```


### styleType {#styleType--}

Specify the type of Built-in slicer style. The default type is SlicerStyleLight1.

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


### firstItemIndex {#firstItemIndex--}

Specifies the zero-based index of the first slicer item.

```javascript
firstItemIndex : number;
```


### captionVisible {#captionVisible--}

Returns or sets whether the header that displays the slicer Caption is visible. The default value is true

```javascript
captionVisible : boolean;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use [Slicer.ShowCaption](../slicer.showcaption/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### showCaption {#showCaption--}

Indicates whether the header of the slicer is visible. The default value is true

```javascript
showCaption : boolean;
```


### numberOfColumns {#numberOfColumns--}

Returns or sets the number of columns in the specified slicer. The default value is 1.

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

Returns or sets the width of each column in the slicer in unit of points.

```javascript
columnWidth : number;
```


### rowHeightPixel {#rowHeightPixel--}

Returns or sets the height of each row in the specified slicer, in unit of pixels.

```javascript
rowHeightPixel : number;
```


### rowHeight {#rowHeight--}

Returns or sets the height of each row in the specified slicer in unit of points.

```javascript
rowHeight : number;
```


### getSortOrderType() {#getSortOrderType--}

<b>@deprecated.</b> Please use the 'sortOrderType' property instead. Indicates the type of sorting items.

```javascript
getSortOrderType() : SortOrder;
```


**Returns**

[SortOrder](../sortorder/)

### setSortOrderType(SortOrder) {#setSortOrderType-sortorder-}

<b>@deprecated.</b> Please use the 'sortOrderType' property instead. Indicates the type of sorting items.

```javascript
setSortOrderType(value: SortOrder) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SortOrder](../sortorder/) | The value to set. |

### getShowMissing() {#getShowMissing--}

<b>@deprecated.</b> Please use the 'showMissing' property instead. Indicates whether to show items deteleted from the data source.

```javascript
getShowMissing() : boolean;
```


**Remarks**

Only works when [Slicer.ShowAllItems](../slicer.showallitems/) is true.

### setShowMissing(boolean) {#setShowMissing-boolean-}

<b>@deprecated.</b> Please use the 'showMissing' property instead. Indicates whether to show items deteleted from the data source.

```javascript
setShowMissing(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only works when [Slicer.ShowAllItems](../slicer.showallitems/) is true.

### getShowTypeOfItemsWithNoData() {#getShowTypeOfItemsWithNoData--}

<b>@deprecated.</b> Please use the 'showTypeOfItemsWithNoData' property instead. Indicates whether to show items deteleted from the data source.

```javascript
getShowTypeOfItemsWithNoData() : ItemsWithNoDataShowMode;
```


**Returns**

[ItemsWithNoDataShowMode](../itemswithnodatashowmode/)

**Remarks**

Only works when [Slicer.ShowAllItems](../slicer.showallitems/) is true.

### setShowTypeOfItemsWithNoData(ItemsWithNoDataShowMode) {#setShowTypeOfItemsWithNoData-itemswithnodatashowmode-}

<b>@deprecated.</b> Please use the 'showTypeOfItemsWithNoData' property instead. Indicates whether to show items deteleted from the data source.

```javascript
setShowTypeOfItemsWithNoData(value: ItemsWithNoDataShowMode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ItemsWithNoDataShowMode](../itemswithnodatashowmode/) | The value to set. |

**Remarks**

Only works when [Slicer.ShowAllItems](../slicer.showallitems/) is true.

### getShowAllItems() {#getShowAllItems--}

<b>@deprecated.</b> Please use the 'showAllItems' property instead. Indicates whether to show all items even if there are no data or they are deleted. Default value is true;

```javascript
getShowAllItems() : boolean;
```


### setShowAllItems(boolean) {#setShowAllItems-boolean-}

<b>@deprecated.</b> Please use the 'showAllItems' property instead. Indicates whether to show all items even if there are no data or they are deleted. Default value is true;

```javascript
setShowAllItems(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getTitle() {#getTitle--}

<b>@deprecated.</b> Please use the 'title' property instead. Specifies the title of the current Slicer object.

```javascript
getTitle() : string;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use [Shape.Title](../shape.title/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### setTitle(string) {#setTitle-string-}

<b>@deprecated.</b> Please use the 'title' property instead. Specifies the title of the current Slicer object.

```javascript
setTitle(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

NOTE: This member is now obsolete. Instead, please use [Shape.Title](../shape.title/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### getAlternativeText() {#getAlternativeText--}

<b>@deprecated.</b> Please use the 'alternativeText' property instead. Returns or sets the descriptive (alternative) text string of the Slicer object.

```javascript
getAlternativeText() : string;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use [Shape.AlternativeText](../shape.alternativetext/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### setAlternativeText(string) {#setAlternativeText-string-}

<b>@deprecated.</b> Please use the 'alternativeText' property instead. Returns or sets the descriptive (alternative) text string of the Slicer object.

```javascript
setAlternativeText(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

NOTE: This member is now obsolete. Instead, please use [Shape.AlternativeText](../shape.alternativetext/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### isPrintable() {#isPrintable--}

<b>@deprecated.</b> Please use the 'isPrintable' property instead. Indicates whether the slicer object is printable.

```javascript
isPrintable() : boolean;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use [Shape.IsPrintable](../shape.isprintable/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### setIsPrintable(boolean) {#setIsPrintable-boolean-}

<b>@deprecated.</b> Please use the 'isPrintable' property instead. Indicates whether the slicer object is printable.

```javascript
setIsPrintable(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

NOTE: This member is now obsolete. Instead, please use [Shape.IsPrintable](../shape.isprintable/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### isLocked() {#isLocked--}

<b>@deprecated.</b> Please use the 'isLocked' property instead. Indicates whether the slicer shape is locked.

```javascript
isLocked() : boolean;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use [Shape.IsLocked](../shape.islocked/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### setIsLocked(boolean) {#setIsLocked-boolean-}

<b>@deprecated.</b> Please use the 'isLocked' property instead. Indicates whether the slicer shape is locked.

```javascript
setIsLocked(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

NOTE: This member is now obsolete. Instead, please use [Shape.IsLocked](../shape.islocked/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### getPlacement() {#getPlacement--}

<b>@deprecated.</b> Please use the 'placement' property instead. Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.

```javascript
getPlacement() : PlacementType;
```


**Returns**

[PlacementType](../placementtype/)

**Remarks**

NOTE: This member is now obsolete. Instead, please use [Shape.Placement](../shape.placement/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### setPlacement(PlacementType) {#setPlacement-placementtype-}

<b>@deprecated.</b> Please use the 'placement' property instead. Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.

```javascript
setPlacement(value: PlacementType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PlacementType](../placementtype/) | The value to set. |

**Remarks**

NOTE: This member is now obsolete. Instead, please use [Shape.Placement](../shape.placement/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### getLockedAspectRatio() {#getLockedAspectRatio--}

<b>@deprecated.</b> Please use the 'lockedAspectRatio' property instead. Indicates whether locking aspect ratio.

```javascript
getLockedAspectRatio() : boolean;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use [Shape.GetLockedProperty()](../shape.getlockedproperty()/) method. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### setLockedAspectRatio(boolean) {#setLockedAspectRatio-boolean-}

<b>@deprecated.</b> Please use the 'lockedAspectRatio' property instead. Indicates whether locking aspect ratio.

```javascript
setLockedAspectRatio(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

NOTE: This member is now obsolete. Instead, please use [Shape.GetLockedProperty()](../shape.getlockedproperty()/) method. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### getLockedPosition() {#getLockedPosition--}

<b>@deprecated.</b> Please use the 'lockedPosition' property instead. Indicates whether the specified slicer can be moved or resized by using the user interface.

```javascript
getLockedPosition() : boolean;
```


### setLockedPosition(boolean) {#setLockedPosition-boolean-}

<b>@deprecated.</b> Please use the 'lockedPosition' property instead. Indicates whether the specified slicer can be moved or resized by using the user interface.

```javascript
setLockedPosition(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShape() {#getShape--}

<b>@deprecated.</b> Please use the 'shape' property instead. Returns the Shape object associated with the specified slicer. Read-only.

```javascript
getShape() : SlicerShape;
```


**Returns**

[SlicerShape](../slicershape/)

### getSlicerCache() {#getSlicerCache--}

<b>@deprecated.</b> Please use the 'slicerCache' property instead. Returns the SlicerCache object associated with the slicer. Read-only.

```javascript
getSlicerCache() : SlicerCache;
```


**Returns**

[SlicerCache](../slicercache/)

### getParent() {#getParent--}

<b>@deprecated.</b> Please use the 'parent' property instead. Returns the [Worksheet](../worksheet/) object which contains this slicer. Read-only.

```javascript
getParent() : Worksheet;
```


**Returns**

[Worksheet](../worksheet/)

**Remarks**

NOTE: This member is now obsolete. Instead, please use [Slicer.Worksheet](../slicer.worksheet/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### getWorksheet() {#getWorksheet--}

<b>@deprecated.</b> Please use the 'worksheet' property instead. Returns the [Worksheet](../worksheet/) object which contains this slicer. Read-only.

```javascript
getWorksheet() : Worksheet;
```


**Returns**

[Worksheet](../worksheet/)

### getStyleType() {#getStyleType--}

<b>@deprecated.</b> Please use the 'styleType' property instead. Specify the type of Built-in slicer style. The default type is SlicerStyleLight1.

```javascript
getStyleType() : SlicerStyleType;
```


**Returns**

[SlicerStyleType](../slicerstyletype/)

### setStyleType(SlicerStyleType) {#setStyleType-slicerstyletype-}

<b>@deprecated.</b> Please use the 'styleType' property instead. Specify the type of Built-in slicer style. The default type is SlicerStyleLight1.

```javascript
setStyleType(value: SlicerStyleType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SlicerStyleType](../slicerstyletype/) | The value to set. |

### getName() {#getName--}

<b>@deprecated.</b> Please use the 'name' property instead. Returns or sets the name of the specified slicer

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

<b>@deprecated.</b> Please use the 'name' property instead. Returns or sets the name of the specified slicer

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getCaption() {#getCaption--}

<b>@deprecated.</b> Please use the 'caption' property instead. Returns or sets the caption of the specified slicer.

```javascript
getCaption() : string;
```


### setCaption(string) {#setCaption-string-}

<b>@deprecated.</b> Please use the 'caption' property instead. Returns or sets the caption of the specified slicer.

```javascript
setCaption(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getFirstItemIndex() {#getFirstItemIndex--}

<b>@deprecated.</b> Please use the 'firstItemIndex' property instead. Specifies the zero-based index of the first slicer item.

```javascript
getFirstItemIndex() : number;
```


### setFirstItemIndex(number) {#setFirstItemIndex-number-}

<b>@deprecated.</b> Please use the 'firstItemIndex' property instead. Specifies the zero-based index of the first slicer item.

```javascript
setFirstItemIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getCaptionVisible() {#getCaptionVisible--}

<b>@deprecated.</b> Please use the 'captionVisible' property instead. Returns or sets whether the header that displays the slicer Caption is visible. The default value is true

```javascript
getCaptionVisible() : boolean;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use [Slicer.ShowCaption](../slicer.showcaption/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### setCaptionVisible(boolean) {#setCaptionVisible-boolean-}

<b>@deprecated.</b> Please use the 'captionVisible' property instead. Returns or sets whether the header that displays the slicer Caption is visible. The default value is true

```javascript
setCaptionVisible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

NOTE: This member is now obsolete. Instead, please use [Slicer.ShowCaption](../slicer.showcaption/) property. This property will be removed 12 months later since January 2026. Aspose apologizes for any inconvenience you may have experienced.

### getShowCaption() {#getShowCaption--}

<b>@deprecated.</b> Please use the 'showCaption' property instead. Indicates whether the header of the slicer is visible. The default value is true

```javascript
getShowCaption() : boolean;
```


### setShowCaption(boolean) {#setShowCaption-boolean-}

<b>@deprecated.</b> Please use the 'showCaption' property instead. Indicates whether the header of the slicer is visible. The default value is true

```javascript
setShowCaption(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getNumberOfColumns() {#getNumberOfColumns--}

<b>@deprecated.</b> Please use the 'numberOfColumns' property instead. Returns or sets the number of columns in the specified slicer. The default value is 1.

```javascript
getNumberOfColumns() : number;
```


### setNumberOfColumns(number) {#setNumberOfColumns-number-}

<b>@deprecated.</b> Please use the 'numberOfColumns' property instead. Returns or sets the number of columns in the specified slicer. The default value is 1.

```javascript
setNumberOfColumns(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLeftPixel() {#getLeftPixel--}

<b>@deprecated.</b> Please use the 'leftPixel' property instead. Returns or sets the horizontal offset of slicer shape from its left column, in pixels.

```javascript
getLeftPixel() : number;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use Shape.Left property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.

### setLeftPixel(number) {#setLeftPixel-number-}

<b>@deprecated.</b> Please use the 'leftPixel' property instead. Returns or sets the horizontal offset of slicer shape from its left column, in pixels.

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

<b>@deprecated.</b> Please use the 'topPixel' property instead. Returns or sets the vertical offset of slicer shape from its top row, in pixels.

```javascript
getTopPixel() : number;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use Shape.Top property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.

### setTopPixel(number) {#setTopPixel-number-}

<b>@deprecated.</b> Please use the 'topPixel' property instead. Returns or sets the vertical offset of slicer shape from its top row, in pixels.

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

<b>@deprecated.</b> Please use the 'width' property instead. Returns or sets the width of the specified slicer, in points.

```javascript
getWidth() : number;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use Shape.WidthPt property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.

### setWidth(number) {#setWidth-number-}

<b>@deprecated.</b> Please use the 'width' property instead. Returns or sets the width of the specified slicer, in points.

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

<b>@deprecated.</b> Please use the 'widthPixel' property instead. Returns or sets the width of the specified slicer, in pixels.

```javascript
getWidthPixel() : number;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use Shape.Width property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.

### setWidthPixel(number) {#setWidthPixel-number-}

<b>@deprecated.</b> Please use the 'widthPixel' property instead. Returns or sets the width of the specified slicer, in pixels.

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

<b>@deprecated.</b> Please use the 'height' property instead. Returns or sets the height of the specified slicer, in points.

```javascript
getHeight() : number;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use Shape.HeightPt property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.

### setHeight(number) {#setHeight-number-}

<b>@deprecated.</b> Please use the 'height' property instead. Returns or sets the height of the specified slicer, in points.

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

<b>@deprecated.</b> Please use the 'heightPixel' property instead. Returns or sets the height of the specified slicer, in pixels.

```javascript
getHeightPixel() : number;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use Shape.Height property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.

### setHeightPixel(number) {#setHeightPixel-number-}

<b>@deprecated.</b> Please use the 'heightPixel' property instead. Returns or sets the height of the specified slicer, in pixels.

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

<b>@deprecated.</b> Please use the 'columnWidthPixel' property instead. Gets or sets the width of each column in the slicer, in unit of pixels.

```javascript
getColumnWidthPixel() : number;
```


### setColumnWidthPixel(number) {#setColumnWidthPixel-number-}

<b>@deprecated.</b> Please use the 'columnWidthPixel' property instead. Gets or sets the width of each column in the slicer, in unit of pixels.

```javascript
setColumnWidthPixel(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getColumnWidth() {#getColumnWidth--}

<b>@deprecated.</b> Please use the 'columnWidth' property instead. Returns or sets the width of each column in the slicer in unit of points.

```javascript
getColumnWidth() : number;
```


### setColumnWidth(number) {#setColumnWidth-number-}

<b>@deprecated.</b> Please use the 'columnWidth' property instead. Returns or sets the width of each column in the slicer in unit of points.

```javascript
setColumnWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getRowHeightPixel() {#getRowHeightPixel--}

<b>@deprecated.</b> Please use the 'rowHeightPixel' property instead. Returns or sets the height of each row in the specified slicer, in unit of pixels.

```javascript
getRowHeightPixel() : number;
```


### setRowHeightPixel(number) {#setRowHeightPixel-number-}

<b>@deprecated.</b> Please use the 'rowHeightPixel' property instead. Returns or sets the height of each row in the specified slicer, in unit of pixels.

```javascript
setRowHeightPixel(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getRowHeight() {#getRowHeight--}

<b>@deprecated.</b> Please use the 'rowHeight' property instead. Returns or sets the height of each row in the specified slicer in unit of points.

```javascript
getRowHeight() : number;
```


### setRowHeight(number) {#setRowHeight-number-}

<b>@deprecated.</b> Please use the 'rowHeight' property instead. Returns or sets the height of each row in the specified slicer in unit of points.

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

Refreshing the slicer. Meanwhile, Refreshing and Calculating PivotTables which this slicer based on.

```javascript
refresh() : void;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



