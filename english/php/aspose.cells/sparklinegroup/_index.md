---
title: "SparklineGroup Class"
linktitle: "SparklineGroup"
articleTitle: "SparklineGroup"
second_title: "Aspose.Cells for PHP via Java"
description: "Sparkline is organized into sparkline group."
type: docs
weight: 6300
url: /php/aspose.cells/sparklinegroup/
---

## SparklineGroup class

Sparkline is organized into sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [PresetStyle](#presetstyle) | Number | Gets and sets the preset style type of the sparkline group. The value of the property is SparklinePresetStyleType intege |
| [SparklineCollection](#sparklinecollection) | SparklineCollection | Gets the collection of Sparkline object. NOTE: This member is now obsolete. Instead, please use SparklineGroup.Sparkline |
| [Sparklines](#sparklines) | SparklineCollection | Gets the collection of Sparkline object. |
| [Type](#type) | Number | Indicates the sparkline type of the sparkline group. The value of the property is SparklineType integer constant. |
| [PlotEmptyCellsType](#plotemptycellstype) | Number | Indicates how to plot empty cells. The value of the property is PlotEmptyCellsType integer constant. |
| [DisplayHidden](#displayhidden) | boolean | Indicates whether to show data in hidden rows and columns. |
| [ShowHighPoint](#showhighpoint) | boolean | Indicates whether to highlight the highest points of data in the sparkline group. |
| [HighPointColor](#highpointcolor) | CellsColor | Gets and sets the color of the highest points of data in the sparkline group. |
| [ShowLowPoint](#showlowpoint) | boolean | Indicates whether to highlight the lowest points of data in the sparkline group. |
| [LowPointColor](#lowpointcolor) | CellsColor | Gets and sets the color of the lowest points of data in the sparkline group. |
| [ShowNegativePoints](#shownegativepoints) | boolean | Indicates whether to highlight the negative values on the sparkline group with a different color or marker. |
| [NegativePointsColor](#negativepointscolor) | CellsColor | Gets and sets the color of the negative values on the sparkline group. |
| [ShowFirstPoint](#showfirstpoint) | boolean | Indicates whether to highlight the first point of data in the sparkline group. |
| [FirstPointColor](#firstpointcolor) | CellsColor | Gets and sets the color of the first point of data in the sparkline group. |
| [ShowLastPoint](#showlastpoint) | boolean | Indicates whether to highlight the last point of data in the sparkline group. |
| [LastPointColor](#lastpointcolor) | CellsColor | Gets and sets the color of the last point of data in the sparkline group. |
| [ShowMarkers](#showmarkers) | boolean | Indicates whether to highlight each point in each line sparkline in the sparkline group. |
| [MarkersColor](#markerscolor) | CellsColor | Gets and sets the color of points in each line sparkline in the sparkline group. |
| [SeriesColor](#seriescolor) | CellsColor | Gets and sets the color of the sparklines in the sparkline group. |
| [PlotRightToLeft](#plotrighttoleft) | boolean | Indicates whether the plot data is right to left. |
| [LineWeight](#lineweight) | Number | Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points. |
| [HorizontalAxisColor](#horizontalaxiscolor) | CellsColor | Gets and sets the color of the horizontal axis in the sparkline group. |
| [ShowHorizontalAxis](#showhorizontalaxis) | boolean | Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that cros |
| [HorizontalAxisDateRange](#horizontalaxisdaterange) | String | Represents the range that contains the date values for the sparkline data. |
| [VerticalAxisMaxValueType](#verticalaxismaxvaluetype) | Number | Represents the vertical axis maximum value type. The value of the property is SparklineAxisMinMaxType integer constant. |
| [VerticalAxisMaxValue](#verticalaxismaxvalue) | Number | Gets and sets the custom maximum value for the vertical axis. |
| [VerticalAxisMinValueType](#verticalaxisminvaluetype) | Number | Represents the vertical axis minimum value type. The value of the property is SparklineAxisMinMaxType integer constant. |
| [VerticalAxisMinValue](#verticalaxisminvalue) | Number | Gets and sets the custom minimum value for the vertical axis. |

## Methods

| Name | Description |
| --- | --- |
| [resetRanges](#resetranges) | Resets the data range and location range of the sparkline group. This method will clear original sparkline items in the  |
| [setVerticalAxisMaxValue](#setverticalaxismaxvalue) |  |
| [setVerticalAxisMinValue](#setverticalaxisminvalue) |  |

### SparklineGroup.PresetStyle property {#presetstyle}

Gets and sets the preset style type of the sparkline group. The value of the property is SparklinePresetStyleType integer constant.

**Type:** Number

### SparklineGroup.SparklineCollection property {#sparklinecollection}

Gets the collection of Sparkline object. NOTE: This member is now obsolete. Instead, please use SparklineGroup.Sparklines property. This property will be removed 12 months later since November 2022. Aspose apologizes for any inconvenience you may have experienced.

**Type:** SparklineCollection

### SparklineGroup.Sparklines property {#sparklines}

Gets the collection of Sparkline object.

**Type:** SparklineCollection

### SparklineGroup.Type property {#type}

Indicates the sparkline type of the sparkline group. The value of the property is SparklineType integer constant.

**Type:** Number

### SparklineGroup.PlotEmptyCellsType property {#plotemptycellstype}

Indicates how to plot empty cells. The value of the property is PlotEmptyCellsType integer constant.

**Type:** Number

### SparklineGroup.DisplayHidden property {#displayhidden}

Indicates whether to show data in hidden rows and columns.

**Type:** boolean

### SparklineGroup.ShowHighPoint property {#showhighpoint}

Indicates whether to highlight the highest points of data in the sparkline group.

**Type:** boolean

### SparklineGroup.HighPointColor property {#highpointcolor}

Gets and sets the color of the highest points of data in the sparkline group.

**Type:** CellsColor

### SparklineGroup.ShowLowPoint property {#showlowpoint}

Indicates whether to highlight the lowest points of data in the sparkline group.

**Type:** boolean

### SparklineGroup.LowPointColor property {#lowpointcolor}

Gets and sets the color of the lowest points of data in the sparkline group.

**Type:** CellsColor

### SparklineGroup.ShowNegativePoints property {#shownegativepoints}

Indicates whether to highlight the negative values on the sparkline group with a different color or marker.

**Type:** boolean

### SparklineGroup.NegativePointsColor property {#negativepointscolor}

Gets and sets the color of the negative values on the sparkline group.

**Type:** CellsColor

### SparklineGroup.ShowFirstPoint property {#showfirstpoint}

Indicates whether to highlight the first point of data in the sparkline group.

**Type:** boolean

### SparklineGroup.FirstPointColor property {#firstpointcolor}

Gets and sets the color of the first point of data in the sparkline group.

**Type:** CellsColor

### SparklineGroup.ShowLastPoint property {#showlastpoint}

Indicates whether to highlight the last point of data in the sparkline group.

**Type:** boolean

### SparklineGroup.LastPointColor property {#lastpointcolor}

Gets and sets the color of the last point of data in the sparkline group.

**Type:** CellsColor

### SparklineGroup.ShowMarkers property {#showmarkers}

Indicates whether to highlight each point in each line sparkline in the sparkline group.

**Type:** boolean

### SparklineGroup.MarkersColor property {#markerscolor}

Gets and sets the color of points in each line sparkline in the sparkline group.

**Type:** CellsColor

### SparklineGroup.SeriesColor property {#seriescolor}

Gets and sets the color of the sparklines in the sparkline group.

**Type:** CellsColor

### SparklineGroup.PlotRightToLeft property {#plotrighttoleft}

Indicates whether the plot data is right to left.

**Type:** boolean

### SparklineGroup.LineWeight property {#lineweight}

Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points.

**Type:** Number

### SparklineGroup.HorizontalAxisColor property {#horizontalaxiscolor}

Gets and sets the color of the horizontal axis in the sparkline group.

**Type:** CellsColor

### SparklineGroup.ShowHorizontalAxis property {#showhorizontalaxis}

Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis.

**Type:** boolean

### SparklineGroup.HorizontalAxisDateRange property {#horizontalaxisdaterange}

Represents the range that contains the date values for the sparkline data.

**Type:** String

### SparklineGroup.VerticalAxisMaxValueType property {#verticalaxismaxvaluetype}

Represents the vertical axis maximum value type. The value of the property is SparklineAxisMinMaxType integer constant.

**Type:** Number

### SparklineGroup.VerticalAxisMaxValue property {#verticalaxismaxvalue}

Gets and sets the custom maximum value for the vertical axis.

**Type:** Number

### SparklineGroup.VerticalAxisMinValueType property {#verticalaxisminvaluetype}

Represents the vertical axis minimum value type. The value of the property is SparklineAxisMinMaxType integer constant.

**Type:** Number

### SparklineGroup.VerticalAxisMinValue property {#verticalaxisminvalue}

Gets and sets the custom minimum value for the vertical axis.

**Type:** Number

### resetRanges(dataRange, isVertical, locationRange) {#resetranges}

Resets the data range and location range of the sparkline group. This method will clear original sparkline items in the group and creates new sparkline items for the new ranges.

| Parameter | Type | Description |
| --- | --- | --- |
| dataRange | String | Specifies the new data range of the sparkline group. |
| isVertical | boolean | Specifies whether to plot the sparklines from the new data range by row or by column. |
| locationRange | CellArea | Specifies where the sparklines to be placed. |

### setVerticalAxisMaxValue(type, value) {#setverticalaxismaxvalue}

### setVerticalAxisMinValue(type, value) {#setverticalaxisminvalue}
