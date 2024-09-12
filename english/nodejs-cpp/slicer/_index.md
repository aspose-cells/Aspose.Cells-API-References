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


## Methods

| Method | Description |
| --- | --- |
| [getTitle()](#getTitle--)| Specifies the title of the current Slicer object. |
| [setTitle(string)](#setTitle-string-)| Specifies the title of the current Slicer object. |
| [getAlternativeText()](#getAlternativeText--)| Returns or sets the descriptive (alternative) text string of the Slicer object. |
| [setAlternativeText(string)](#setAlternativeText-string-)| Returns or sets the descriptive (alternative) text string of the Slicer object. |
| [isPrintable()](#isPrintable--)| Indicates whether the slicer object is printable. |
| [setIsPrintable(boolean)](#setIsPrintable-boolean-)| Indicates whether the slicer object is printable. |
| [isLocked()](#isLocked--)| Indicates whether the slicer shape is locked. |
| [setIsLocked(boolean)](#setIsLocked-boolean-)| Indicates whether the slicer shape is locked. |
| [getPlacement()](#getPlacement--)| Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. |
| [setPlacement(PlacementType)](#setPlacement-placementtype-)| Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. |
| [getLockedAspectRatio()](#getLockedAspectRatio--)| Indicates whether locking aspect ratio. |
| [setLockedAspectRatio(boolean)](#setLockedAspectRatio-boolean-)| Indicates whether locking aspect ratio. |
| [getLockedPosition()](#getLockedPosition--)| Indicates whether the specified slicer can be moved or resized by using the user interface. |
| [setLockedPosition(boolean)](#setLockedPosition-boolean-)| Indicates whether the specified slicer can be moved or resized by using the user interface. |
| [getSlicerCache()](#getSlicerCache--)| Returns the SlicerCache object associated with the slicer. Read-only. |
| [getParent()](#getParent--)| Returns the [Worksheet](../worksheet/) object which contains this slicer. Read-only. |
| [getStyleType()](#getStyleType--)| Specify the type of Built-in slicer style the default type is SlicerStyleLight1 |
| [setStyleType(SlicerStyleType)](#setStyleType-slicerstyletype-)| Specify the type of Built-in slicer style the default type is SlicerStyleLight1 |
| [getName()](#getName--)| Returns or sets the name of the specified slicer |
| [setName(string)](#setName-string-)| Returns or sets the name of the specified slicer |
| [getCaption()](#getCaption--)| Returns or sets the caption of the specified slicer. |
| [setCaption(string)](#setCaption-string-)| Returns or sets the caption of the specified slicer. |
| [getCaptionVisible()](#getCaptionVisible--)| Returns or sets whether the header that displays the slicer Caption is visible the default value is true |
| [setCaptionVisible(boolean)](#setCaptionVisible-boolean-)| Returns or sets whether the header that displays the slicer Caption is visible the default value is true |
| [getNumberOfColumns()](#getNumberOfColumns--)| Returns or sets the number of columns in the specified slicer. |
| [setNumberOfColumns(number)](#setNumberOfColumns-number-)| Returns or sets the number of columns in the specified slicer. |
| [getLeftPixel()](#getLeftPixel--)| Returns or sets the horizontal offset of slicer shape from its left column, in pixels. |
| [setLeftPixel(number)](#setLeftPixel-number-)| Returns or sets the horizontal offset of slicer shape from its left column, in pixels. |
| [getTopPixel()](#getTopPixel--)| Returns or sets the vertical offset of slicer shape from its top row, in pixels. |
| [setTopPixel(number)](#setTopPixel-number-)| Returns or sets the vertical offset of slicer shape from its top row, in pixels. |
| [getWidth()](#getWidth--)| Returns or sets the width of the specified slicer, in points. |
| [setWidth(number)](#setWidth-number-)| Returns or sets the width of the specified slicer, in points. |
| [getWidthPixel()](#getWidthPixel--)| Returns or sets the width of the specified slicer, in pixels. |
| [setWidthPixel(number)](#setWidthPixel-number-)| Returns or sets the width of the specified slicer, in pixels. |
| [getHeight()](#getHeight--)| Returns or sets the height of the specified slicer, in points. |
| [setHeight(number)](#setHeight-number-)| Returns or sets the height of the specified slicer, in points. |
| [getHeightPixel()](#getHeightPixel--)| Returns or sets the height of the specified slicer, in pixels. |
| [setHeightPixel(number)](#setHeightPixel-number-)| Returns or sets the height of the specified slicer, in pixels. |
| [getColumnWidthPixel()](#getColumnWidthPixel--)| Gets or sets the width in unit of pixels for each column of the slicer. |
| [setColumnWidthPixel(number)](#setColumnWidthPixel-number-)| Gets or sets the width in unit of pixels for each column of the slicer. |
| [getColumnWidth()](#getColumnWidth--)| Returns or sets the width, in points, of each column in the slicer. |
| [setColumnWidth(number)](#setColumnWidth-number-)| Returns or sets the width, in points, of each column in the slicer. |
| [getRowHeightPixel()](#getRowHeightPixel--)| Returns or sets the height, in pixels, of each row in the specified slicer. |
| [setRowHeightPixel(number)](#setRowHeightPixel-number-)| Returns or sets the height, in pixels, of each row in the specified slicer. |
| [getRowHeight()](#getRowHeight--)| Returns or sets the height, in points, of each row in the specified slicer. |
| [setRowHeight(number)](#setRowHeight-number-)| Returns or sets the height, in points, of each row in the specified slicer. |
| [addPivotConnection(PivotTable)](#addPivotConnection-pivottable-)| Adds PivotTable connection. |
| [removePivotConnection(PivotTable)](#removePivotConnection-pivottable-)| Removes PivotTable connection. |
| [refresh()](#refresh--)| Refreshing the slicer.Meanwhile, Refreshing and Calculating  relative PivotTables. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getTitle() {#getTitle--}

Specifies the title of the current Slicer object.

```javascript
getTitle() : string;
```


### setTitle(string) {#setTitle-string-}

Specifies the title of the current Slicer object.

```javascript
setTitle(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getAlternativeText() {#getAlternativeText--}

Returns or sets the descriptive (alternative) text string of the Slicer object.

```javascript
getAlternativeText() : string;
```


### setAlternativeText(string) {#setAlternativeText-string-}

Returns or sets the descriptive (alternative) text string of the Slicer object.

```javascript
setAlternativeText(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isPrintable() {#isPrintable--}

Indicates whether the slicer object is printable.

```javascript
isPrintable() : boolean;
```


### setIsPrintable(boolean) {#setIsPrintable-boolean-}

Indicates whether the slicer object is printable.

```javascript
setIsPrintable(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isLocked() {#isLocked--}

Indicates whether the slicer shape is locked.

```javascript
isLocked() : boolean;
```


### setIsLocked(boolean) {#setIsLocked-boolean-}

Indicates whether the slicer shape is locked.

```javascript
setIsLocked(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPlacement() {#getPlacement--}

Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.

```javascript
getPlacement() : PlacementType;
```


**Returns**

[PlacementType](../placementtype/)

### setPlacement(PlacementType) {#setPlacement-placementtype-}

Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.

```javascript
setPlacement(value: PlacementType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PlacementType](../placementtype/) | The value to set. |

### getLockedAspectRatio() {#getLockedAspectRatio--}

Indicates whether locking aspect ratio.

```javascript
getLockedAspectRatio() : boolean;
```


### setLockedAspectRatio(boolean) {#setLockedAspectRatio-boolean-}

Indicates whether locking aspect ratio.

```javascript
setLockedAspectRatio(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getLockedPosition() {#getLockedPosition--}

Indicates whether the specified slicer can be moved or resized by using the user interface.

```javascript
getLockedPosition() : boolean;
```


### setLockedPosition(boolean) {#setLockedPosition-boolean-}

Indicates whether the specified slicer can be moved or resized by using the user interface.

```javascript
setLockedPosition(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSlicerCache() {#getSlicerCache--}

Returns the SlicerCache object associated with the slicer. Read-only.

```javascript
getSlicerCache() : SlicerCache;
```


**Returns**

[SlicerCache](../slicercache/)

### getParent() {#getParent--}

Returns the [Worksheet](../worksheet/) object which contains this slicer. Read-only.

```javascript
getParent() : Worksheet;
```


**Returns**

[Worksheet](../worksheet/)

### getStyleType() {#getStyleType--}

Specify the type of Built-in slicer style the default type is SlicerStyleLight1

```javascript
getStyleType() : SlicerStyleType;
```


**Returns**

[SlicerStyleType](../slicerstyletype/)

### setStyleType(SlicerStyleType) {#setStyleType-slicerstyletype-}

Specify the type of Built-in slicer style the default type is SlicerStyleLight1

```javascript
setStyleType(value: SlicerStyleType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SlicerStyleType](../slicerstyletype/) | The value to set. |

### getName() {#getName--}

Returns or sets the name of the specified slicer

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

Returns or sets the name of the specified slicer

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getCaption() {#getCaption--}

Returns or sets the caption of the specified slicer.

```javascript
getCaption() : string;
```


### setCaption(string) {#setCaption-string-}

Returns or sets the caption of the specified slicer.

```javascript
setCaption(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getCaptionVisible() {#getCaptionVisible--}

Returns or sets whether the header that displays the slicer Caption is visible the default value is true

```javascript
getCaptionVisible() : boolean;
```


### setCaptionVisible(boolean) {#setCaptionVisible-boolean-}

Returns or sets whether the header that displays the slicer Caption is visible the default value is true

```javascript
setCaptionVisible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getNumberOfColumns() {#getNumberOfColumns--}

Returns or sets the number of columns in the specified slicer.

```javascript
getNumberOfColumns() : number;
```


### setNumberOfColumns(number) {#setNumberOfColumns-number-}

Returns or sets the number of columns in the specified slicer.

```javascript
setNumberOfColumns(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLeftPixel() {#getLeftPixel--}

Returns or sets the horizontal offset of slicer shape from its left column, in pixels.

```javascript
getLeftPixel() : number;
```


### setLeftPixel(number) {#setLeftPixel-number-}

Returns or sets the horizontal offset of slicer shape from its left column, in pixels.

```javascript
setLeftPixel(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getTopPixel() {#getTopPixel--}

Returns or sets the vertical offset of slicer shape from its top row, in pixels.

```javascript
getTopPixel() : number;
```


### setTopPixel(number) {#setTopPixel-number-}

Returns or sets the vertical offset of slicer shape from its top row, in pixels.

```javascript
setTopPixel(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWidth() {#getWidth--}

Returns or sets the width of the specified slicer, in points.

```javascript
getWidth() : number;
```


### setWidth(number) {#setWidth-number-}

Returns or sets the width of the specified slicer, in points.

```javascript
setWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWidthPixel() {#getWidthPixel--}

Returns or sets the width of the specified slicer, in pixels.

```javascript
getWidthPixel() : number;
```


### setWidthPixel(number) {#setWidthPixel-number-}

Returns or sets the width of the specified slicer, in pixels.

```javascript
setWidthPixel(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeight() {#getHeight--}

Returns or sets the height of the specified slicer, in points.

```javascript
getHeight() : number;
```


### setHeight(number) {#setHeight-number-}

Returns or sets the height of the specified slicer, in points.

```javascript
setHeight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeightPixel() {#getHeightPixel--}

Returns or sets the height of the specified slicer, in pixels.

```javascript
getHeightPixel() : number;
```


### setHeightPixel(number) {#setHeightPixel-number-}

Returns or sets the height of the specified slicer, in pixels.

```javascript
setHeightPixel(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getColumnWidthPixel() {#getColumnWidthPixel--}

Gets or sets the width in unit of pixels for each column of the slicer.

```javascript
getColumnWidthPixel() : number;
```


### setColumnWidthPixel(number) {#setColumnWidthPixel-number-}

Gets or sets the width in unit of pixels for each column of the slicer.

```javascript
setColumnWidthPixel(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getColumnWidth() {#getColumnWidth--}

Returns or sets the width, in points, of each column in the slicer.

```javascript
getColumnWidth() : number;
```


### setColumnWidth(number) {#setColumnWidth-number-}

Returns or sets the width, in points, of each column in the slicer.

```javascript
setColumnWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getRowHeightPixel() {#getRowHeightPixel--}

Returns or sets the height, in pixels, of each row in the specified slicer.

```javascript
getRowHeightPixel() : number;
```


### setRowHeightPixel(number) {#setRowHeightPixel-number-}

Returns or sets the height, in pixels, of each row in the specified slicer.

```javascript
setRowHeightPixel(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getRowHeight() {#getRowHeight--}

Returns or sets the height, in points, of each row in the specified slicer.

```javascript
getRowHeight() : number;
```


### setRowHeight(number) {#setRowHeight-number-}

Returns or sets the height, in points, of each row in the specified slicer.

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



