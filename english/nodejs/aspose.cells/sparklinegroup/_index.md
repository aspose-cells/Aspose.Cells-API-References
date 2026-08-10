---
title: "SparklineGroup"
linktitle: "SparklineGroup"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Sparkline is organized into sparkline group."
type: docs
weight: 3870
url: /nodejs/aspose.cells/sparklinegroup/
---

## SparklineGroup class

Sparkline is organized into sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines.

## Methods

| Name | Description |
| --- | --- |
| [getDisplayHidden()](#getdisplayhidden) | Indicates whether to show data in hidden rows and columns. |
| [getFirstPointColor()](#getfirstpointcolor) | Gets and sets the color of the first point of data in the sparkline group. |
| [getHighPointColor()](#gethighpointcolor) | Gets and sets the color of the highest points of data in the sparkline group. |
| [getHorizontalAxisColor()](#gethorizontalaxiscolor) | Gets and sets the color of the horizontal axis in the sparkline group. |
| [getHorizontalAxisDateRange()](#gethorizontalaxisdaterange) | Represents the range that contains the date values for the sparkline data. |
| [getLastPointColor()](#getlastpointcolor) | Gets and sets the color of the last point of data in the sparkline group. |
| [getLineWeight()](#getlineweight) | Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points. |
| [getLowPointColor()](#getlowpointcolor) | Gets and sets the color of the lowest points of data in the sparkline group. |
| [getMarkersColor()](#getmarkerscolor) | Gets and sets the color of points in each line sparkline in the sparkline group. |
| [getNegativePointsColor()](#getnegativepointscolor) | Gets and sets the color of the negative values on the sparkline group. |
| [getPlotEmptyCellsType()](#getplotemptycellstype) | Indicates how to plot empty cells. The value of the property is PlotEmptyCellsType integer constant. |
| [getPlotRightToLeft()](#getplotrighttoleft) | Indicates whether the plot data is right to left. |
| [getPresetStyle()](#getpresetstyle) | Gets and sets the preset style type of the sparkline group. The value of the property is SparklinePresetStyleType intege |
| [getSeriesColor()](#getseriescolor) | Gets and sets the color of the sparklines in the sparkline group. |
| [getShowFirstPoint()](#getshowfirstpoint) | Indicates whether to highlight the first point of data in the sparkline group. |
| [getShowHighPoint()](#getshowhighpoint) | Indicates whether to highlight the highest points of data in the sparkline group. |
| [getShowHorizontalAxis()](#getshowhorizontalaxis) | Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that cros |
| [getShowLastPoint()](#getshowlastpoint) | Indicates whether to highlight the last point of data in the sparkline group. |
| [getShowLowPoint()](#getshowlowpoint) | Indicates whether to highlight the lowest points of data in the sparkline group. |
| [getShowMarkers()](#getshowmarkers) | Indicates whether to highlight each point in each line sparkline in the sparkline group. |
| [getShowNegativePoints()](#getshownegativepoints) | Indicates whether to highlight the negative values on the sparkline group with a different color or marker. |
| [getSparklineCollection()](#getsparklinecollection) | Gets the collection of Sparkline object. NOTE: This member is now obsolete. Instead, please use SparklineGroup.Sparkline |
| [getSparklines()](#getsparklines) | Gets the collection of Sparkline object. |
| [getType()](#gettype) | Indicates the sparkline type of the sparkline group. The value of the property is SparklineType integer constant. |
| [getVerticalAxisMaxValue()](#getverticalaxismaxvalue) | Gets and sets the custom maximum value for the vertical axis. |
| [getVerticalAxisMaxValueType()](#getverticalaxismaxvaluetype) | Represents the vertical axis maximum value type. The value of the property is SparklineAxisMinMaxType integer constant. |
| [getVerticalAxisMinValue()](#getverticalaxisminvalue) | Gets and sets the custom minimum value for the vertical axis. |
| [getVerticalAxisMinValueType()](#getverticalaxisminvaluetype) | Represents the vertical axis minimum value type. The value of the property is SparklineAxisMinMaxType integer constant. |
| [resetRanges(dataRange, isVertical, locationRange)](#resetranges) | Resets the data range and location range of the sparkline group. This method will clear original sparkline items in the  |
| [setDisplayHidden()](#setdisplayhidden) | Indicates whether to show data in hidden rows and columns. |
| [setFirstPointColor()](#setfirstpointcolor) | Gets and sets the color of the first point of data in the sparkline group. |
| [setHighPointColor()](#sethighpointcolor) | Gets and sets the color of the highest points of data in the sparkline group. |
| [setHorizontalAxisColor()](#sethorizontalaxiscolor) | Gets and sets the color of the horizontal axis in the sparkline group. |
| [setHorizontalAxisDateRange()](#sethorizontalaxisdaterange) | Represents the range that contains the date values for the sparkline data. |
| [setLastPointColor()](#setlastpointcolor) | Gets and sets the color of the last point of data in the sparkline group. |
| [setLineWeight()](#setlineweight) | Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points. |
| [setLowPointColor()](#setlowpointcolor) | Gets and sets the color of the lowest points of data in the sparkline group. |
| [setMarkersColor()](#setmarkerscolor) | Gets and sets the color of points in each line sparkline in the sparkline group. |
| [setNegativePointsColor()](#setnegativepointscolor) | Gets and sets the color of the negative values on the sparkline group. |
| [setPlotEmptyCellsType()](#setplotemptycellstype) | Indicates how to plot empty cells. The value of the property is PlotEmptyCellsType integer constant. |
| [setPlotRightToLeft()](#setplotrighttoleft) | Indicates whether the plot data is right to left. |
| [setPresetStyle()](#setpresetstyle) | Gets and sets the preset style type of the sparkline group. The value of the property is SparklinePresetStyleType intege |
| [setSeriesColor()](#setseriescolor) | Gets and sets the color of the sparklines in the sparkline group. |
| [setShowFirstPoint()](#setshowfirstpoint) | Indicates whether to highlight the first point of data in the sparkline group. |
| [setShowHighPoint()](#setshowhighpoint) | Indicates whether to highlight the highest points of data in the sparkline group. |
| [setShowHorizontalAxis()](#setshowhorizontalaxis) | Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that cros |
| [setShowLastPoint()](#setshowlastpoint) | Indicates whether to highlight the last point of data in the sparkline group. |
| [setShowLowPoint()](#setshowlowpoint) | Indicates whether to highlight the lowest points of data in the sparkline group. |
| [setShowMarkers()](#setshowmarkers) | Indicates whether to highlight each point in each line sparkline in the sparkline group. |
| [setShowNegativePoints()](#setshownegativepoints) | Indicates whether to highlight the negative values on the sparkline group with a different color or marker. |
| [setType()](#settype) | Indicates the sparkline type of the sparkline group. The value of the property is SparklineType integer constant. |
| [setVerticalAxisMaxValue()](#setverticalaxismaxvalue) | Gets and sets the custom maximum value for the vertical axis. |
| [setVerticalAxisMaxValue()](#setverticalaxismaxvalue-1) |  |
| [setVerticalAxisMaxValueType()](#setverticalaxismaxvaluetype) | Represents the vertical axis maximum value type. The value of the property is SparklineAxisMinMaxType integer constant. |
| [setVerticalAxisMinValue()](#setverticalaxisminvalue) | Gets and sets the custom minimum value for the vertical axis. |
| [setVerticalAxisMinValue()](#setverticalaxisminvalue-1) |  |
| [setVerticalAxisMinValueType()](#setverticalaxisminvaluetype) | Represents the vertical axis minimum value type. The value of the property is SparklineAxisMinMaxType integer constant. |

### getDisplayHidden() {#getdisplayhidden}

Indicates whether to show data in hidden rows and columns.

### getFirstPointColor() {#getfirstpointcolor}

Gets and sets the color of the first point of data in the sparkline group.

### getHighPointColor() {#gethighpointcolor}

Gets and sets the color of the highest points of data in the sparkline group.

### getHorizontalAxisColor() {#gethorizontalaxiscolor}

Gets and sets the color of the horizontal axis in the sparkline group.

### getHorizontalAxisDateRange() {#gethorizontalaxisdaterange}

Represents the range that contains the date values for the sparkline data.

### getLastPointColor() {#getlastpointcolor}

Gets and sets the color of the last point of data in the sparkline group.

### getLineWeight() {#getlineweight}

Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points.

### getLowPointColor() {#getlowpointcolor}

Gets and sets the color of the lowest points of data in the sparkline group.

### getMarkersColor() {#getmarkerscolor}

Gets and sets the color of points in each line sparkline in the sparkline group.

### getNegativePointsColor() {#getnegativepointscolor}

Gets and sets the color of the negative values on the sparkline group.

### getPlotEmptyCellsType() {#getplotemptycellstype}

Indicates how to plot empty cells. The value of the property is PlotEmptyCellsType integer constant.

### getPlotRightToLeft() {#getplotrighttoleft}

Indicates whether the plot data is right to left.

### getPresetStyle() {#getpresetstyle}

Gets and sets the preset style type of the sparkline group. The value of the property is SparklinePresetStyleType integer constant.

### getSeriesColor() {#getseriescolor}

Gets and sets the color of the sparklines in the sparkline group.

### getShowFirstPoint() {#getshowfirstpoint}

Indicates whether to highlight the first point of data in the sparkline group.

### getShowHighPoint() {#getshowhighpoint}

Indicates whether to highlight the highest points of data in the sparkline group.

### getShowHorizontalAxis() {#getshowhorizontalaxis}

Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis.

### getShowLastPoint() {#getshowlastpoint}

Indicates whether to highlight the last point of data in the sparkline group.

### getShowLowPoint() {#getshowlowpoint}

Indicates whether to highlight the lowest points of data in the sparkline group.

### getShowMarkers() {#getshowmarkers}

Indicates whether to highlight each point in each line sparkline in the sparkline group.

### getShowNegativePoints() {#getshownegativepoints}

Indicates whether to highlight the negative values on the sparkline group with a different color or marker.

### getSparklineCollection() {#getsparklinecollection}

Gets the collection of Sparkline object. NOTE: This member is now obsolete. Instead, please use SparklineGroup.Sparklines property. This property will be removed 12 months later since November 2022. Aspose apologizes for any inconvenience you may have experienced.

### getSparklines() {#getsparklines}

Gets the collection of Sparkline object.

### getType() {#gettype}

Indicates the sparkline type of the sparkline group. The value of the property is SparklineType integer constant.

### getVerticalAxisMaxValue() {#getverticalaxismaxvalue}

Gets and sets the custom maximum value for the vertical axis.

### getVerticalAxisMaxValueType() {#getverticalaxismaxvaluetype}

Represents the vertical axis maximum value type. The value of the property is SparklineAxisMinMaxType integer constant.

### getVerticalAxisMinValue() {#getverticalaxisminvalue}

Gets and sets the custom minimum value for the vertical axis.

### getVerticalAxisMinValueType() {#getverticalaxisminvaluetype}

Represents the vertical axis minimum value type. The value of the property is SparklineAxisMinMaxType integer constant.

### resetRanges(dataRange, isVertical, locationRange) {#resetranges}

Resets the data range and location range of the sparkline group. This method will clear original sparkline items in the group and creates new sparkline items for the new ranges.

| Parameter | Type | Description |
| --- | --- | --- |
| dataRange | String | Specifies the new data range of the sparkline group. |
| isVertical | boolean | Specifies whether to plot the sparklines from the new data range by row or by column. |
| locationRange | CellArea | Specifies where the sparklines to be placed. |

### setDisplayHidden() {#setdisplayhidden}

Indicates whether to show data in hidden rows and columns.

### setFirstPointColor() {#setfirstpointcolor}

Gets and sets the color of the first point of data in the sparkline group.

### setHighPointColor() {#sethighpointcolor}

Gets and sets the color of the highest points of data in the sparkline group.

### setHorizontalAxisColor() {#sethorizontalaxiscolor}

Gets and sets the color of the horizontal axis in the sparkline group.

### setHorizontalAxisDateRange() {#sethorizontalaxisdaterange}

Represents the range that contains the date values for the sparkline data.

### setLastPointColor() {#setlastpointcolor}

Gets and sets the color of the last point of data in the sparkline group.

### setLineWeight() {#setlineweight}

Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points.

### setLowPointColor() {#setlowpointcolor}

Gets and sets the color of the lowest points of data in the sparkline group.

### setMarkersColor() {#setmarkerscolor}

Gets and sets the color of points in each line sparkline in the sparkline group.

### setNegativePointsColor() {#setnegativepointscolor}

Gets and sets the color of the negative values on the sparkline group.

### setPlotEmptyCellsType() {#setplotemptycellstype}

Indicates how to plot empty cells. The value of the property is PlotEmptyCellsType integer constant.

### setPlotRightToLeft() {#setplotrighttoleft}

Indicates whether the plot data is right to left.

### setPresetStyle() {#setpresetstyle}

Gets and sets the preset style type of the sparkline group. The value of the property is SparklinePresetStyleType integer constant.

### setSeriesColor() {#setseriescolor}

Gets and sets the color of the sparklines in the sparkline group.

### setShowFirstPoint() {#setshowfirstpoint}

Indicates whether to highlight the first point of data in the sparkline group.

### setShowHighPoint() {#setshowhighpoint}

Indicates whether to highlight the highest points of data in the sparkline group.

### setShowHorizontalAxis() {#setshowhorizontalaxis}

Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis.

### setShowLastPoint() {#setshowlastpoint}

Indicates whether to highlight the last point of data in the sparkline group.

### setShowLowPoint() {#setshowlowpoint}

Indicates whether to highlight the lowest points of data in the sparkline group.

### setShowMarkers() {#setshowmarkers}

Indicates whether to highlight each point in each line sparkline in the sparkline group.

### setShowNegativePoints() {#setshownegativepoints}

Indicates whether to highlight the negative values on the sparkline group with a different color or marker.

### setType() {#settype}

Indicates the sparkline type of the sparkline group. The value of the property is SparklineType integer constant.

### setVerticalAxisMaxValue() {#setverticalaxismaxvalue}

Gets and sets the custom maximum value for the vertical axis.

### setVerticalAxisMaxValue() {#setverticalaxismaxvalue-1}

### setVerticalAxisMaxValueType() {#setverticalaxismaxvaluetype}

Represents the vertical axis maximum value type. The value of the property is SparklineAxisMinMaxType integer constant.

### setVerticalAxisMinValue() {#setverticalaxisminvalue}

Gets and sets the custom minimum value for the vertical axis.

### setVerticalAxisMinValue() {#setverticalaxisminvalue-1}

### setVerticalAxisMinValueType() {#setverticalaxisminvaluetype}

Represents the vertical axis minimum value type. The value of the property is SparklineAxisMinMaxType integer constant.
