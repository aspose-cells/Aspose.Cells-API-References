---
title: SparklineGroup
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Sparkline..sparkline is organized into sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type display settings and axis settings for the sparklines.
type: docs
url: /javascript-cpp/sparklinegroup/
---

## SparklineGroup class

[Sparkline](../sparkline/) is organized into sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines.

```javascript
class SparklineGroup;
```


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [presetStyle](#presetStyle--)| SparklinePresetStyleType | Gets and sets the preset style type of the sparkline group. |
| [sparklines](#sparklines--)| SparklineCollection | Readonly. Gets the collection of [Sparkline](../sparkline/) object. |
| [type](#type--)| SparklineType | Indicates the sparkline type of the sparkline group. |
| [plotEmptyCellsType](#plotEmptyCellsType--)| PlotEmptyCellsType | Indicates how to plot empty cells. |
| [displayHidden](#displayHidden--)| boolean | Indicates whether to show data in hidden rows and columns. |
| [showHighPoint](#showHighPoint--)| boolean | Indicates whether to highlight the highest points of data in the sparkline group. |
| [highPointColor](#highPointColor--)| CellsColor | Gets and sets the color of the highest points of data in the sparkline group. |
| [showLowPoint](#showLowPoint--)| boolean | Indicates whether to highlight the lowest points of data in the sparkline group. |
| [lowPointColor](#lowPointColor--)| CellsColor | Gets and sets the color of the lowest points of data in the sparkline group. |
| [showNegativePoints](#showNegativePoints--)| boolean | Indicates whether to highlight the negative values on the sparkline group with a different color or marker. |
| [negativePointsColor](#negativePointsColor--)| CellsColor | Gets and sets the color of the negative values on the sparkline group. |
| [showFirstPoint](#showFirstPoint--)| boolean | Indicates whether to highlight the first point of data in the sparkline group. |
| [firstPointColor](#firstPointColor--)| CellsColor | Gets and sets the color of the first point of data in the sparkline group. |
| [showLastPoint](#showLastPoint--)| boolean | Indicates whether to highlight the last point of data in the sparkline group. |
| [lastPointColor](#lastPointColor--)| CellsColor | Gets and sets the color of the last point of data in the sparkline group. |
| [showMarkers](#showMarkers--)| boolean | Indicates whether to highlight each point in each line sparkline in the sparkline group. |
| [markersColor](#markersColor--)| CellsColor | Gets and sets the color of points in each line sparkline in the sparkline group. |
| [seriesColor](#seriesColor--)| CellsColor | Gets and sets the color of the sparklines in the sparkline group. |
| [plotRightToLeft](#plotRightToLeft--)| boolean | Indicates whether the plot data is right to left. |
| [lineWeight](#lineWeight--)| number | Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points. |
| [horizontalAxisColor](#horizontalAxisColor--)| CellsColor | Gets and sets the color of the horizontal axis in the sparkline group. |
| [showHorizontalAxis](#showHorizontalAxis--)| boolean | Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis. |
| [horizontalAxisDateRange](#horizontalAxisDateRange--)| string | Represents the range that contains the date values for the sparkline data. |
| [verticalAxisMaxValueType](#verticalAxisMaxValueType--)| SparklineAxisMinMaxType | Represents the vertical axis maximum value type. |
| [verticalAxisMaxValue](#verticalAxisMaxValue--)| number | Gets and sets the custom maximum value for the vertical axis. |
| [verticalAxisMinValueType](#verticalAxisMinValueType--)| SparklineAxisMinMaxType | Represents the vertical axis minimum value type. |
| [verticalAxisMinValue](#verticalAxisMinValue--)| number | Gets and sets the custom minimum value for the vertical axis. |

## Methods

| Method | Description |
| --- | --- |
| [resetRanges(string, boolean, CellArea)](#resetRanges-string-boolean-cellarea-)| Resets the data range and location range of the sparkline group. This method will clear original sparkline items in the group and creates new sparkline items for the new ranges. |


### presetStyle {#presetStyle--}

Gets and sets the preset style type of the sparkline group.

```javascript
presetStyle : SparklinePresetStyleType;
```


### sparklines {#sparklines--}

Readonly. Gets the collection of [Sparkline](../sparkline/) object.

```javascript
sparklines : SparklineCollection;
```


### type {#type--}

Indicates the sparkline type of the sparkline group.

```javascript
type : SparklineType;
```


### plotEmptyCellsType {#plotEmptyCellsType--}

Indicates how to plot empty cells.

```javascript
plotEmptyCellsType : PlotEmptyCellsType;
```


### displayHidden {#displayHidden--}

Indicates whether to show data in hidden rows and columns.

```javascript
displayHidden : boolean;
```


### showHighPoint {#showHighPoint--}

Indicates whether to highlight the highest points of data in the sparkline group.

```javascript
showHighPoint : boolean;
```


### highPointColor {#highPointColor--}

Gets and sets the color of the highest points of data in the sparkline group.

```javascript
highPointColor : CellsColor;
```


### showLowPoint {#showLowPoint--}

Indicates whether to highlight the lowest points of data in the sparkline group.

```javascript
showLowPoint : boolean;
```


### lowPointColor {#lowPointColor--}

Gets and sets the color of the lowest points of data in the sparkline group.

```javascript
lowPointColor : CellsColor;
```


### showNegativePoints {#showNegativePoints--}

Indicates whether to highlight the negative values on the sparkline group with a different color or marker.

```javascript
showNegativePoints : boolean;
```


### negativePointsColor {#negativePointsColor--}

Gets and sets the color of the negative values on the sparkline group.

```javascript
negativePointsColor : CellsColor;
```


### showFirstPoint {#showFirstPoint--}

Indicates whether to highlight the first point of data in the sparkline group.

```javascript
showFirstPoint : boolean;
```


### firstPointColor {#firstPointColor--}

Gets and sets the color of the first point of data in the sparkline group.

```javascript
firstPointColor : CellsColor;
```


### showLastPoint {#showLastPoint--}

Indicates whether to highlight the last point of data in the sparkline group.

```javascript
showLastPoint : boolean;
```


### lastPointColor {#lastPointColor--}

Gets and sets the color of the last point of data in the sparkline group.

```javascript
lastPointColor : CellsColor;
```


### showMarkers {#showMarkers--}

Indicates whether to highlight each point in each line sparkline in the sparkline group.

```javascript
showMarkers : boolean;
```


### markersColor {#markersColor--}

Gets and sets the color of points in each line sparkline in the sparkline group.

```javascript
markersColor : CellsColor;
```


### seriesColor {#seriesColor--}

Gets and sets the color of the sparklines in the sparkline group.

```javascript
seriesColor : CellsColor;
```


### plotRightToLeft {#plotRightToLeft--}

Indicates whether the plot data is right to left.

```javascript
plotRightToLeft : boolean;
```


### lineWeight {#lineWeight--}

Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points.

```javascript
lineWeight : number;
```


### horizontalAxisColor {#horizontalAxisColor--}

Gets and sets the color of the horizontal axis in the sparkline group.

```javascript
horizontalAxisColor : CellsColor;
```


### showHorizontalAxis {#showHorizontalAxis--}

Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis.

```javascript
showHorizontalAxis : boolean;
```


### horizontalAxisDateRange {#horizontalAxisDateRange--}

Represents the range that contains the date values for the sparkline data.

```javascript
horizontalAxisDateRange : string;
```


### verticalAxisMaxValueType {#verticalAxisMaxValueType--}

Represents the vertical axis maximum value type.

```javascript
verticalAxisMaxValueType : SparklineAxisMinMaxType;
```


### verticalAxisMaxValue {#verticalAxisMaxValue--}

Gets and sets the custom maximum value for the vertical axis.

```javascript
verticalAxisMaxValue : number;
```


**Remarks**

If this property is set, [VerticalAxisMaxValueType](../verticalaxismaxvaluetype/) will be <see  cref="SparklineAxisMinMaxType.Custom"/>.

### verticalAxisMinValueType {#verticalAxisMinValueType--}

Represents the vertical axis minimum value type.

```javascript
verticalAxisMinValueType : SparklineAxisMinMaxType;
```


### verticalAxisMinValue {#verticalAxisMinValue--}

Gets and sets the custom minimum value for the vertical axis.

```javascript
verticalAxisMinValue : number;
```


**Remarks**

If this property is set, [VerticalAxisMinValueType](../verticalaxisminvaluetype/) will be <see  cref="SparklineAxisMinMaxType.Custom"/>.

### resetRanges(string, boolean, CellArea) {#resetRanges-string-boolean-cellarea-}

Resets the data range and location range of the sparkline group. This method will clear original sparkline items in the group and creates new sparkline items for the new ranges.

```javascript
resetRanges(dataRange: string, isVertical: boolean, locationRange: CellArea) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dataRange | string | Specifies the new data range of the sparkline group. |
| isVertical | boolean | Specifies whether to plot the sparklines from the new data range by row or by column. |
| locationRange | [CellArea](../cellarea/) | Specifies where the sparklines to be placed. |


