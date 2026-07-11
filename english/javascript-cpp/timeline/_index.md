---
title: Timeline
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Summary description of Timeline View Due to MS Excel Excel 2003 does not support Timeline
type: docs
url: /javascript-cpp/timeline/
---

## Timeline class

Summary description of Timeline View Due to MS Excel, Excel 2003 does not support Timeline

```javascript
class Timeline;
```


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [showHeader](#showHeader--)| boolean | Indicates whether to display the header of this timeline. |
| [showSelectionLabel](#showSelectionLabel--)| boolean | Indicates whether to display the selction label. |
| [showTimeLevel](#showTimeLevel--)| boolean | Indicates whether to display the drop-down selection box of the time level. |
| [showHorizontalScrollbar](#showHorizontalScrollbar--)| boolean | Indicates whether to display the horizontal scroll bar. |
| [startDate](#startDate--)| Date | Gets and sets the start date of the timespan scrolling position of this [Timeline](../timeline/). |
| [currentLevel](#currentLevel--)| TimelineLevelType | The current time level of the Timeline. |
| [selectionLevel](#selectionLevel--)| TimelineLevelType | Gets and sets the time level at which the current selection was made for the Timeline. |
| [caption](#caption--)| string | Gets or sets the caption of this Timeline. |
| [shape](#shape--)| TimelineShape | Readonly. Returns the [TimelineShape](../timelineshape/) object associated with this Timeline. |
| [name](#name--)| string | Returns or sets the name of the specified Timeline |
| [leftPixel](#leftPixel--)| number | Returns or sets the horizontal offset of timeline shape from its left column, in pixels. |
| [topPixel](#topPixel--)| number | Returns or sets the vertical offset of timeline shape from its top row, in pixels. |
| [widthPixel](#widthPixel--)| number | Returns or sets the width of the specified timeline, in pixels. |
| [heightPixel](#heightPixel--)| number | Returns or sets the height of the specified timeline, in pixels. |

## Methods

| Method | Description |
| --- | --- |
| [getSelectedDateTimeRange()](#getSelectedDateTimeRange--)| Gets the selected range of date time. |
| [select(Date, Date, boolean)](#select-date-date-boolean-)| Select item between the date time. |


### showHeader {#showHeader--}

Indicates whether to display the header of this timeline.

```javascript
showHeader : boolean;
```


### showSelectionLabel {#showSelectionLabel--}

Indicates whether to display the selction label.

```javascript
showSelectionLabel : boolean;
```


### showTimeLevel {#showTimeLevel--}

Indicates whether to display the drop-down selection box of the time level.

```javascript
showTimeLevel : boolean;
```


### showHorizontalScrollbar {#showHorizontalScrollbar--}

Indicates whether to display the horizontal scroll bar.

```javascript
showHorizontalScrollbar : boolean;
```


### startDate {#startDate--}

Gets and sets the start date of the timespan scrolling position of this [Timeline](../timeline/).

```javascript
startDate : Date;
```


### currentLevel {#currentLevel--}

The current time level of the Timeline.

```javascript
currentLevel : TimelineLevelType;
```


### selectionLevel {#selectionLevel--}

Gets and sets the time level at which the current selection was made for the Timeline.

```javascript
selectionLevel : TimelineLevelType;
```


### caption {#caption--}

Gets or sets the caption of this Timeline.

```javascript
caption : string;
```


### shape {#shape--}

Readonly. Returns the [TimelineShape](../timelineshape/) object associated with this Timeline.

```javascript
shape : TimelineShape;
```


### name {#name--}

Returns or sets the name of the specified Timeline

```javascript
name : string;
```


### leftPixel {#leftPixel--}

Returns or sets the horizontal offset of timeline shape from its left column, in pixels.

```javascript
leftPixel : number;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use Shape.Left property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.

### topPixel {#topPixel--}

Returns or sets the vertical offset of timeline shape from its top row, in pixels.

```javascript
topPixel : number;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use Shape.Top property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.

### widthPixel {#widthPixel--}

Returns or sets the width of the specified timeline, in pixels.

```javascript
widthPixel : number;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use Shape.Width property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.

### heightPixel {#heightPixel--}

Returns or sets the height of the specified timeline, in pixels.

```javascript
heightPixel : number;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use Shape.Height property. This property will be removed 12 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.

### getSelectedDateTimeRange() {#getSelectedDateTimeRange--}

Gets the selected range of date time.

```javascript
getSelectedDateTimeRange() : Date[];
```


**Returns**

Date[]

### select(Date, Date, boolean) {#select-date-date-boolean-}

Select item between the date time.

```javascript
select(start: Date, end: Date, calculate: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | Date | The start date time |
| end | Date | The end date time |
| calculate | boolean | Indicates whether to calculate relative pivot tables |

**Remarks**

[Timeline.CurrentLevel](../timeline.currentlevel/) must be set before calling this method. If this method is called, [Timeline.SelectionLevel](../timeline.selectionlevel/) will be [Timeline.CurrentLevel](../timeline.currentlevel/).


