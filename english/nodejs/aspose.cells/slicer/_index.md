---
title: "Slicer"
linktitle: "Slicer"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "summary description of Slicer View"
type: docs
weight: 3710
url: /nodejs/aspose.cells/slicer/
---

## Slicer class

summary description of Slicer View

## Methods

| Name | Description |
| --- | --- |
| [addPivotConnection(pivot)](#addpivotconnection) | Adds PivotTable connection. |
| [clearFilter()](#clearfilter) |  |
| [getAlternativeText()](#getalternativetext) | Returns or sets the descriptive (alternative) text string of the Slicer object. |
| [getCaption()](#getcaption) | Returns or sets the caption of the specified slicer. |
| [getCaptionVisible()](#getcaptionvisible) | Returns or sets whether the header that displays the slicer Caption is visible the default value is true |
| [getColumnWidth()](#getcolumnwidth) | Returns or sets the width, in points, of each column in the slicer. |
| [getColumnWidthPixel()](#getcolumnwidthpixel) | Gets or sets the width in unit of pixels for each column of the slicer. |
| [getFirstItemIndex()](#getfirstitemindex) |  |
| [getHeight()](#getheight) | Returns or sets the height of the specified slicer, in points. |
| [getHeightPixel()](#getheightpixel) | Returns or sets the height of the specified slicer, in pixels. |
| [getLeftPixel()](#getleftpixel) | Returns or sets the horizontal offset of slicer shape from its left column, in pixels. |
| [getLockedAspectRatio()](#getlockedaspectratio) | Indicates whether locking aspect ratio. |
| [getLockedPosition()](#getlockedposition) | Indicates whether the specified slicer can be moved or resized by using the user interface. |
| [getName()](#getname) | Returns or sets the name of the specified slicer |
| [getNumberOfColumns()](#getnumberofcolumns) | Returns or sets the number of columns in the specified slicer. |
| [getParent()](#getparent) | Returns the Worksheet object which contains this slicer. Read-only. |
| [getPlacement()](#getplacement) | Represents the way the drawing object is attached to the cells below it. The property controls the placement of an objec |
| [getRowHeight()](#getrowheight) | Returns or sets the height, in points, of each row in the specified slicer. |
| [getRowHeightPixel()](#getrowheightpixel) | Returns or sets the height, in pixels, of each row in the specified slicer. |
| [getShape()](#getshape) | Returns the Shape object associated with the specified slicer. Read-only. |
| [getShowAllItems()](#getshowallitems) |  |
| [getShowCaption()](#getshowcaption) |  |
| [getShowMissing()](#getshowmissing) |  |
| [getShowTypeOfItemsWithNoData()](#getshowtypeofitemswithnodata) | The value of the property is ItemsWithNoDataShowMode integer constant. |
| [getSlicerCache()](#getslicercache) | Returns the SlicerCache object associated with the slicer. Read-only. |
| [getSortOrderType()](#getsortordertype) | The value of the property is SortOrder integer constant. |
| [getStyleType()](#getstyletype) | Specify the type of Built-in slicer style the default type is SlicerStyleLight1 The value of the property is SlicerStyle |
| [getTitle()](#gettitle) | Specifies the title of the current Slicer object. |
| [getTopPixel()](#gettoppixel) | Returns or sets the vertical offset of slicer shape from its top row, in pixels. |
| [getWidth()](#getwidth) | Returns or sets the width of the specified slicer, in points. |
| [getWidthPixel()](#getwidthpixel) | Returns or sets the width of the specified slicer, in pixels. |
| [getWorksheet()](#getworksheet) |  |
| [isLocked()](#islocked) | Indicates whether the slicer shape is locked. |
| [isPrintable()](#isprintable) | Indicates whether the slicer object is printable. |
| [refresh()](#refresh) | Refreshing the slicer.Meanwhile, Refreshing and Calculating relative PivotTables. |
| [removePivotConnection(pivot)](#removepivotconnection) | Removes PivotTable connection. |
| [selectItems()](#selectitems) |  |
| [setAlternativeText()](#setalternativetext) | Returns or sets the descriptive (alternative) text string of the Slicer object. |
| [setCaption()](#setcaption) | Returns or sets the caption of the specified slicer. |
| [setCaptionVisible()](#setcaptionvisible) | Returns or sets whether the header that displays the slicer Caption is visible the default value is true |
| [setColumnWidth()](#setcolumnwidth) | Returns or sets the width, in points, of each column in the slicer. |
| [setColumnWidthPixel()](#setcolumnwidthpixel) | Gets or sets the width in unit of pixels for each column of the slicer. |
| [setFirstItemIndex()](#setfirstitemindex) |  |
| [setHeight()](#setheight) | Returns or sets the height of the specified slicer, in points. |
| [setHeightPixel()](#setheightpixel) | Returns or sets the height of the specified slicer, in pixels. |
| [setLeftPixel()](#setleftpixel) | Returns or sets the horizontal offset of slicer shape from its left column, in pixels. |
| [setLocked()](#setlocked) | Indicates whether the slicer shape is locked. |
| [setLockedAspectRatio()](#setlockedaspectratio) | Indicates whether locking aspect ratio. |
| [setLockedPosition()](#setlockedposition) | Indicates whether the specified slicer can be moved or resized by using the user interface. |
| [setName()](#setname) | Returns or sets the name of the specified slicer |
| [setNumberOfColumns()](#setnumberofcolumns) | Returns or sets the number of columns in the specified slicer. |
| [setPlacement()](#setplacement) | Represents the way the drawing object is attached to the cells below it. The property controls the placement of an objec |
| [setPrintable()](#setprintable) | Indicates whether the slicer object is printable. |
| [setRowHeight()](#setrowheight) | Returns or sets the height, in points, of each row in the specified slicer. |
| [setRowHeightPixel()](#setrowheightpixel) | Returns or sets the height, in pixels, of each row in the specified slicer. |
| [setShowAllItems()](#setshowallitems) |  |
| [setShowCaption()](#setshowcaption) |  |
| [setShowMissing()](#setshowmissing) |  |
| [setShowTypeOfItemsWithNoData()](#setshowtypeofitemswithnodata) | The value of the property is ItemsWithNoDataShowMode integer constant. |
| [setSortOrderType()](#setsortordertype) | The value of the property is SortOrder integer constant. |
| [setStyleType()](#setstyletype) | Specify the type of Built-in slicer style the default type is SlicerStyleLight1 The value of the property is SlicerStyle |
| [setTitle()](#settitle) | Specifies the title of the current Slicer object. |
| [setTopPixel()](#settoppixel) | Returns or sets the vertical offset of slicer shape from its top row, in pixels. |
| [setWidth()](#setwidth) | Returns or sets the width of the specified slicer, in points. |
| [setWidthPixel()](#setwidthpixel) | Returns or sets the width of the specified slicer, in pixels. |
| [unselectItems()](#unselectitems) |  |

### addPivotConnection(pivot) {#addpivotconnection}

Adds PivotTable connection.

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | The PivotTable object |

### clearFilter() {#clearfilter}

### getAlternativeText() {#getalternativetext}

Returns or sets the descriptive (alternative) text string of the Slicer object.

### getCaption() {#getcaption}

Returns or sets the caption of the specified slicer.

### getCaptionVisible() {#getcaptionvisible}

Returns or sets whether the header that displays the slicer Caption is visible the default value is true

### getColumnWidth() {#getcolumnwidth}

Returns or sets the width, in points, of each column in the slicer.

### getColumnWidthPixel() {#getcolumnwidthpixel}

Gets or sets the width in unit of pixels for each column of the slicer.

### getFirstItemIndex() {#getfirstitemindex}

### getHeight() {#getheight}

Returns or sets the height of the specified slicer, in points.

### getHeightPixel() {#getheightpixel}

Returns or sets the height of the specified slicer, in pixels.

### getLeftPixel() {#getleftpixel}

Returns or sets the horizontal offset of slicer shape from its left column, in pixels.

### getLockedAspectRatio() {#getlockedaspectratio}

Indicates whether locking aspect ratio.

### getLockedPosition() {#getlockedposition}

Indicates whether the specified slicer can be moved or resized by using the user interface.

### getName() {#getname}

Returns or sets the name of the specified slicer

### getNumberOfColumns() {#getnumberofcolumns}

Returns or sets the number of columns in the specified slicer.

### getParent() {#getparent}

Returns the Worksheet object which contains this slicer. Read-only.

### getPlacement() {#getplacement}

Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. The value of the property is PlacementType integer constant.

### getRowHeight() {#getrowheight}

Returns or sets the height, in points, of each row in the specified slicer.

### getRowHeightPixel() {#getrowheightpixel}

Returns or sets the height, in pixels, of each row in the specified slicer.

### getShape() {#getshape}

Returns the Shape object associated with the specified slicer. Read-only.

### getShowAllItems() {#getshowallitems}

### getShowCaption() {#getshowcaption}

### getShowMissing() {#getshowmissing}

### getShowTypeOfItemsWithNoData() {#getshowtypeofitemswithnodata}

The value of the property is ItemsWithNoDataShowMode integer constant.

### getSlicerCache() {#getslicercache}

Returns the SlicerCache object associated with the slicer. Read-only.

### getSortOrderType() {#getsortordertype}

The value of the property is SortOrder integer constant.

### getStyleType() {#getstyletype}

Specify the type of Built-in slicer style the default type is SlicerStyleLight1 The value of the property is SlicerStyleType integer constant.

### getTitle() {#gettitle}

Specifies the title of the current Slicer object.

### getTopPixel() {#gettoppixel}

Returns or sets the vertical offset of slicer shape from its top row, in pixels.

### getWidth() {#getwidth}

Returns or sets the width of the specified slicer, in points.

### getWidthPixel() {#getwidthpixel}

Returns or sets the width of the specified slicer, in pixels.

### getWorksheet() {#getworksheet}

### isLocked() {#islocked}

Indicates whether the slicer shape is locked.

### isPrintable() {#isprintable}

Indicates whether the slicer object is printable.

### refresh() {#refresh}

Refreshing the slicer.Meanwhile, Refreshing and Calculating relative PivotTables.

### removePivotConnection(pivot) {#removepivotconnection}

Removes PivotTable connection.

| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | The PivotTable object |

### selectItems() {#selectitems}

### setAlternativeText() {#setalternativetext}

Returns or sets the descriptive (alternative) text string of the Slicer object.

### setCaption() {#setcaption}

Returns or sets the caption of the specified slicer.

### setCaptionVisible() {#setcaptionvisible}

Returns or sets whether the header that displays the slicer Caption is visible the default value is true

### setColumnWidth() {#setcolumnwidth}

Returns or sets the width, in points, of each column in the slicer.

### setColumnWidthPixel() {#setcolumnwidthpixel}

Gets or sets the width in unit of pixels for each column of the slicer.

### setFirstItemIndex() {#setfirstitemindex}

### setHeight() {#setheight}

Returns or sets the height of the specified slicer, in points.

### setHeightPixel() {#setheightpixel}

Returns or sets the height of the specified slicer, in pixels.

### setLeftPixel() {#setleftpixel}

Returns or sets the horizontal offset of slicer shape from its left column, in pixels.

### setLocked() {#setlocked}

Indicates whether the slicer shape is locked.

### setLockedAspectRatio() {#setlockedaspectratio}

Indicates whether locking aspect ratio.

### setLockedPosition() {#setlockedposition}

Indicates whether the specified slicer can be moved or resized by using the user interface.

### setName() {#setname}

Returns or sets the name of the specified slicer

### setNumberOfColumns() {#setnumberofcolumns}

Returns or sets the number of columns in the specified slicer.

### setPlacement() {#setplacement}

Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. The value of the property is PlacementType integer constant.

### setPrintable() {#setprintable}

Indicates whether the slicer object is printable.

### setRowHeight() {#setrowheight}

Returns or sets the height, in points, of each row in the specified slicer.

### setRowHeightPixel() {#setrowheightpixel}

Returns or sets the height, in pixels, of each row in the specified slicer.

### setShowAllItems() {#setshowallitems}

### setShowCaption() {#setshowcaption}

### setShowMissing() {#setshowmissing}

### setShowTypeOfItemsWithNoData() {#setshowtypeofitemswithnodata}

The value of the property is ItemsWithNoDataShowMode integer constant.

### setSortOrderType() {#setsortordertype}

The value of the property is SortOrder integer constant.

### setStyleType() {#setstyletype}

Specify the type of Built-in slicer style the default type is SlicerStyleLight1 The value of the property is SlicerStyleType integer constant.

### setTitle() {#settitle}

Specifies the title of the current Slicer object.

### setTopPixel() {#settoppixel}

Returns or sets the vertical offset of slicer shape from its top row, in pixels.

### setWidth() {#setwidth}

Returns or sets the width of the specified slicer, in points.

### setWidthPixel() {#setwidthpixel}

Returns or sets the width of the specified slicer, in pixels.

### unselectItems() {#unselectitems}
