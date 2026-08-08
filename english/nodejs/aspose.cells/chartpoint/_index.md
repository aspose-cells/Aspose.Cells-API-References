---
title: "ChartPoint"
linktitle: "ChartPoint"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents a single point in a series in a chart."
type: docs
weight: 560
url: /nodejs/aspose.cells/chartpoint/
---

## ChartPoint class

Represents a single point in a series in a chart.

## Methods

| Name | Description |
| --- | --- |
| [getArcEndPointXPx()](#getarcendpointxpx) | Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Dough |
| [getArcEndPointYPx()](#getarcendpointypx) | Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Dough |
| [getArcStartPointXPx()](#getarcstartpointxpx) | Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Dou |
| [getArcStartPointYPx()](#getarcstartpointypx) | Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Dou |
| [getArea()](#getarea) | Gets the Area. |
| [getBorder()](#getborder) | Gets the Line. |
| [getBorderWidthPx()](#getborderwidthpx) | Gets the width of border in units of pixels after calls Chart.Calculate() method. |
| [getBottomPointCount()](#getbottompointcount) | Gets the number of bottom points after calls Chart.Calculate() method. |
| [getBottomPointXPx()](#getbottompointxpx) | Gets x-coordinate of the bottom point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, |
| [getBottomPointYPx()](#getbottompointypx) | Gets y-coordinate of the bottom point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, |
| [getDataLabels()](#getdatalabels) | Returns a DataLabels object that represents the data label associated with this chart point. |
| [getDoughnutInnerRadius()](#getdoughnutinnerradius) |  |
| [getEndAngle()](#getendangle) | Gets the ending angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() m |
| [getExplosion()](#getexplosion) | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [getInnerArcEndPointXPx()](#getinnerarcendpointxpx) | Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut char |
| [getInnerArcEndPointYPx()](#getinnerarcendpointypx) | Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut char |
| [getInnerArcStartPointXPx()](#getinnerarcstartpointxpx) | Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut ch |
| [getInnerArcStartPointYPx()](#getinnerarcstartpointypx) | Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut ch |
| [getInnerRadiusPx()](#getinnerradiuspx) | Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut cha |
| [getMarker()](#getmarker) | Gets the Marker. |
| [getOnCategoryAxisPointCount()](#getoncategoryaxispointcount) | Gets the number of the points on category axis after calls Chart.Calculate() method. Only applies to area chart. Area 2D |
| [getOnCategoryAxisPointXPx()](#getoncategoryaxispointxpx) | Gets x-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart. Area 2 |
| [getOnCategoryAxisPointYPx()](#getoncategoryaxispointypx) | Gets y-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart. Area 2 |
| [getRadiusPx()](#getradiuspx) | Gets the radius of bubble, pie or doughnut in units of pixels after calls Chart.Calculate() method. |
| [getShadow()](#getshadow) | True if the chartpoint has a shadow. |
| [getShapeHeight()](#getshapeheight) | Gets the height in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [getShapeHeightPx()](#getshapeheightpx) | Gets the height in units of pixels after calls Chart.Calculate() method. |
| [getShapeProperties()](#getshapeproperties) | Gets the ShapePropertyCollection object that holds the visual shape properties of the ChartPoint. |
| [getShapeWidth()](#getshapewidth) | Gets the width in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [getShapeWidthPx()](#getshapewidthpx) | Gets the width in units of pixels after calls Chart.Calculate() method. |
| [getShapeX()](#getshapex) | Gets the x coordinate of the upper left corner in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [getShapeXPx()](#getshapexpx) | Gets the x coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method. |
| [getShapeY()](#getshapey) | Gets the y coordinate of the upper left corner in units of 1/4000 of chart's height after calls Chart.Calculate() method |
| [getShapeYPx()](#getshapeypx) | Gets the y coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method. |
| [getStartAngle()](#getstartangle) | Gets the starting angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() |
| [getTopPointCount()](#gettoppointcount) | Gets the number of top points after calls Chart.Calculate() method. |
| [getTopPointXPx()](#gettoppointxpx) | Gets x-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Co |
| [getTopPointYPx()](#gettoppointypx) | Gets y-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Co |
| [getXValue()](#getxvalue) | Gets or sets the X value of the chart point. |
| [getXValueType()](#getxvaluetype) | Gets X value type of the chart point. The value of the property is CellValueType integer constant. |
| [getYValue()](#getyvalue) | Gets or sets the Y value of the chart point. |
| [getYValueType()](#getyvaluetype) | Gets Y value type of the chart point. The value of the property is CellValueType integer constant. |
| [isInSecondaryPlot()](#isinsecondaryplot) | Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart |
| [setExplosion()](#setexplosion) | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [setInSecondaryPlot()](#setinsecondaryplot) | Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart |
| [setShadow()](#setshadow) | True if the chartpoint has a shadow. |
| [setXValue()](#setxvalue) | Gets or sets the X value of the chart point. |
| [setYValue()](#setyvalue) | Gets or sets the Y value of the chart point. |

### getArcEndPointXPx() {#getarcendpointxpx}

Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart.

### getArcEndPointYPx() {#getarcendpointypx}

Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart.

### getArcStartPointXPx() {#getarcstartpointxpx}

Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart.

### getArcStartPointYPx() {#getarcstartpointypx}

Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart.

### getArea() {#getarea}

Gets the Area.

### getBorder() {#getborder}

Gets the Line.

### getBorderWidthPx() {#getborderwidthpx}

Gets the width of border in units of pixels after calls Chart.Calculate() method.

### getBottomPointCount() {#getbottompointcount}

Gets the number of bottom points after calls Chart.Calculate() method.

### getBottomPointXPx() {#getbottompointxpx}

Gets x-coordinate of the bottom point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid

### getBottomPointYPx() {#getbottompointypx}

Gets y-coordinate of the bottom point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid

### getDataLabels() {#getdatalabels}

Returns a DataLabels object that represents the data label associated with this chart point.

### getDoughnutInnerRadius() {#getdoughnutinnerradius}

### getEndAngle() {#getendangle}

Gets the ending angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart.

### getExplosion() {#getexplosion}

The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.

### getInnerArcEndPointXPx() {#getinnerarcendpointxpx}

Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.

### getInnerArcEndPointYPx() {#getinnerarcendpointypx}

Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.

### getInnerArcStartPointXPx() {#getinnerarcstartpointxpx}

Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.

### getInnerArcStartPointYPx() {#getinnerarcstartpointypx}

Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.

### getInnerRadiusPx() {#getinnerradiuspx}

Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut chart.

### getMarker() {#getmarker}

Gets the Marker.

### getOnCategoryAxisPointCount() {#getoncategoryaxispointcount}

Gets the number of the points on category axis after calls Chart.Calculate() method. Only applies to area chart. Area 2D chart return 1 Area 3D chart return 2.

### getOnCategoryAxisPointXPx() {#getoncategoryaxispointxpx}

Gets x-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart. Area 2D chart: index is 0. Area 3D chart: index is 0 or 1.

### getOnCategoryAxisPointYPx() {#getoncategoryaxispointypx}

Gets y-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart. Area 2D chart: index is 0. Area 3D chart: index is 0 or 1.

### getRadiusPx() {#getradiuspx}

Gets the radius of bubble, pie or doughnut in units of pixels after calls Chart.Calculate() method.

### getShadow() {#getshadow}

True if the chartpoint has a shadow.

### getShapeHeight() {#getshapeheight}

Gets the height in units of 1/4000 of chart's height after calls Chart.Calculate() method.

### getShapeHeightPx() {#getshapeheightpx}

Gets the height in units of pixels after calls Chart.Calculate() method.

### getShapeProperties() {#getshapeproperties}

Gets the ShapePropertyCollection object that holds the visual shape properties of the ChartPoint.

### getShapeWidth() {#getshapewidth}

Gets the width in units of 1/4000 of chart's width after calls Chart.Calculate() method.

### getShapeWidthPx() {#getshapewidthpx}

Gets the width in units of pixels after calls Chart.Calculate() method.

### getShapeX() {#getshapex}

Gets the x coordinate of the upper left corner in units of 1/4000 of chart's width after calls Chart.Calculate() method.

### getShapeXPx() {#getshapexpx}

Gets the x coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method.

### getShapeY() {#getshapey}

Gets the y coordinate of the upper left corner in units of 1/4000 of chart's height after calls Chart.Calculate() method.

### getShapeYPx() {#getshapeypx}

Gets the y coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method.

### getStartAngle() {#getstartangle}

Gets the starting angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart.

### getTopPointCount() {#gettoppointcount}

Gets the number of top points after calls Chart.Calculate() method.

### getTopPointXPx() {#gettoppointxpx}

Gets x-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D

### getTopPointYPx() {#gettoppointypx}

Gets y-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D

### getXValue() {#getxvalue}

Gets or sets the X value of the chart point.

### getXValueType() {#getxvaluetype}

Gets X value type of the chart point. The value of the property is CellValueType integer constant.

### getYValue() {#getyvalue}

Gets or sets the Y value of the chart point.

### getYValueType() {#getyvaluetype}

Gets Y value type of the chart point. The value of the property is CellValueType integer constant.

### isInSecondaryPlot() {#isinsecondaryplot}

Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart

### setExplosion() {#setexplosion}

The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.

### setInSecondaryPlot() {#setinsecondaryplot}

Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart

### setShadow() {#setshadow}

True if the chartpoint has a shadow.

### setXValue() {#setxvalue}

Gets or sets the X value of the chart point.

### setYValue() {#setyvalue}

Gets or sets the Y value of the chart point.
