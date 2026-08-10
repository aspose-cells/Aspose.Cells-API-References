---
title: "ChartPoint Class"
linktitle: "ChartPoint"
articleTitle: "ChartPoint"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents a single point in a series in a chart."
type: docs
weight: 820
url: /php/aspose.cells/chartpoint/
---

## ChartPoint class

Represents a single point in a series in a chart.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Explosion](#explosion) | Number | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [Shadow](#shadow) | boolean | True if the chartpoint has a shadow. |
| [Border](#border) | Line | Gets the Line . |
| [Area](#area) | Area | Gets the Area . |
| [Marker](#marker) | Marker | Gets the Marker . |
| [DataLabels](#datalabels) | DataLabels | Returns a DataLabels object that represents the data label associated with this chart point. |
| [YValue](#yvalue) | Object | Gets or sets the Y value of the chart point. |
| [YValueType](#yvaluetype) | Number | Gets Y value type of the chart point. The value of the property is CellValueType integer constant. |
| [XValue](#xvalue) | Object | Gets or sets the X value of the chart point. |
| [XValueType](#xvaluetype) | Number | Gets X value type of the chart point. The value of the property is CellValueType integer constant. |
| [ShapeProperties](#shapeproperties) | ShapePropertyCollection | Gets the ShapePropertyCollection object that holds the visual shape properties of the ChartPoint. |
| [IsInSecondaryPlot](#isinsecondaryplot) | boolean | Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart |
| [ShapeX](#shapex) | Number | Gets the x coordinate of the upper left corner in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [ShapeY](#shapey) | Number | Gets the y coordinate of the upper left corner in units of 1/4000 of chart's height after calls Chart.Calculate() method |
| [ShapeWidth](#shapewidth) | Number | Gets the width in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [ShapeHeight](#shapeheight) | Number | Gets the height in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [ShapeXPx](#shapexpx) | Number | Gets the x coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method. |
| [ShapeYPx](#shapeypx) | Number | Gets the y coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method. |
| [ShapeWidthPx](#shapewidthpx) | Number | Gets the width in units of pixels after calls Chart.Calculate() method. |
| [ShapeHeightPx](#shapeheightpx) | Number | Gets the height in units of pixels after calls Chart.Calculate() method. |
| [BorderWidthPx](#borderwidthpx) | Number | Gets the width of border in units of pixels after calls Chart.Calculate() method. |
| [RadiusPx](#radiuspx) | Number | Gets the radius of bubble, pie or doughnut in units of pixels after calls Chart.Calculate() method. |
| [DoughnutInnerRadius](#doughnutinnerradius) | Number | Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut cha |
| [InnerRadiusPx](#innerradiuspx) | Number | Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut cha |
| [StartAngle](#startangle) | Number | Gets the starting angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() |
| [EndAngle](#endangle) | Number | Gets the ending angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() m |
| [ArcStartPointXPx](#arcstartpointxpx) | Number | Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Dou |
| [ArcStartPointYPx](#arcstartpointypx) | Number | Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Dou |
| [ArcEndPointXPx](#arcendpointxpx) | Number | Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Dough |
| [ArcEndPointYPx](#arcendpointypx) | Number | Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Dough |
| [InnerArcStartPointXPx](#innerarcstartpointxpx) | Number | Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut ch |
| [InnerArcStartPointYPx](#innerarcstartpointypx) | Number | Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut ch |
| [InnerArcEndPointXPx](#innerarcendpointxpx) | Number | Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut char |
| [InnerArcEndPointYPx](#innerarcendpointypx) | Number | Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut char |

## Methods

| Name | Description |
| --- | --- |
| [getTopPointCount](#gettoppointcount) | Gets the number of top points after calls Chart.Calculate() method. |
| [getTopPointXPx](#gettoppointxpx) | Gets x-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Co |
| [getTopPointYPx](#gettoppointypx) | Gets y-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Co |
| [getBottomPointCount](#getbottompointcount) | Gets the number of bottom points after calls Chart.Calculate() method. |
| [getBottomPointXPx](#getbottompointxpx) | Gets x-coordinate of the bottom point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, |
| [getBottomPointYPx](#getbottompointypx) | Gets y-coordinate of the bottom point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, |
| [getOnCategoryAxisPointCount](#getoncategoryaxispointcount) | Gets the number of the points on category axis after calls Chart.Calculate() method. Only applies to area chart.

Area 2 |
| [getOnCategoryAxisPointXPx](#getoncategoryaxispointxpx) | Gets x-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart.

Area  |
| [getOnCategoryAxisPointYPx](#getoncategoryaxispointypx) | Gets y-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart.

Area  |

### ChartPoint.Explosion property {#explosion}

The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.

**Type:** Number

### ChartPoint.Shadow property {#shadow}

True if the chartpoint has a shadow.

**Type:** boolean

### ChartPoint.Border property {#border}

Gets the Line .

**Type:** Line

### ChartPoint.Area property {#area}

Gets the Area .

**Type:** Area

### ChartPoint.Marker property {#marker}

Gets the Marker .

**Type:** Marker

### ChartPoint.DataLabels property {#datalabels}

Returns a DataLabels object that represents the data label associated with this chart point.

**Type:** DataLabels

### ChartPoint.YValue property {#yvalue}

Gets or sets the Y value of the chart point.

**Type:** Object

### ChartPoint.YValueType property {#yvaluetype}

Gets Y value type of the chart point. The value of the property is CellValueType integer constant.

**Type:** Number

### ChartPoint.XValue property {#xvalue}

Gets or sets the X value of the chart point.

**Type:** Object

### ChartPoint.XValueType property {#xvaluetype}

Gets X value type of the chart point. The value of the property is CellValueType integer constant.

**Type:** Number

### ChartPoint.ShapeProperties property {#shapeproperties}

Gets the ShapePropertyCollection object that holds the visual shape properties of the ChartPoint.

**Type:** ShapePropertyCollection

### ChartPoint.IsInSecondaryPlot property {#isinsecondaryplot}

Gets or sets a value indicates whether this data points is in the second pie or bar on a pie of pie or bar of pie chart

**Type:** boolean

### ChartPoint.ShapeX property {#shapex}

Gets the x coordinate of the upper left corner in units of 1/4000 of chart's width after calls Chart.Calculate() method.

**Type:** Number

### ChartPoint.ShapeY property {#shapey}

Gets the y coordinate of the upper left corner in units of 1/4000 of chart's height after calls Chart.Calculate() method.

**Type:** Number

### ChartPoint.ShapeWidth property {#shapewidth}

Gets the width in units of 1/4000 of chart's width after calls Chart.Calculate() method.

**Type:** Number

### ChartPoint.ShapeHeight property {#shapeheight}

Gets the height in units of 1/4000 of chart's height after calls Chart.Calculate() method.

**Type:** Number

### ChartPoint.ShapeXPx property {#shapexpx}

Gets the x coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method.

**Type:** Number

### ChartPoint.ShapeYPx property {#shapeypx}

Gets the y coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method.

**Type:** Number

### ChartPoint.ShapeWidthPx property {#shapewidthpx}

Gets the width in units of pixels after calls Chart.Calculate() method.

**Type:** Number

### ChartPoint.ShapeHeightPx property {#shapeheightpx}

Gets the height in units of pixels after calls Chart.Calculate() method.

**Type:** Number

### ChartPoint.BorderWidthPx property {#borderwidthpx}

Gets the width of border in units of pixels after calls Chart.Calculate() method.

**Type:** Number

### ChartPoint.RadiusPx property {#radiuspx}

Gets the radius of bubble, pie or doughnut in units of pixels after calls Chart.Calculate() method.

**Type:** Number

### ChartPoint.DoughnutInnerRadius property {#doughnutinnerradius}

Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut chart.

**Type:** Number

### ChartPoint.InnerRadiusPx property {#innerradiuspx}

Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method. Applies to Doughnut chart. NOTE: This property is now obsolete. Instead, please use ChartPoint.DoughnutInnerRadius property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

**Type:** Number

### ChartPoint.StartAngle property {#startangle}

Gets the starting angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart.

**Type:** Number

### ChartPoint.EndAngle property {#endangle}

Gets the ending angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method. Applies to Pie chart.

**Type:** Number

### ChartPoint.ArcStartPointXPx property {#arcstartpointxpx}

Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart.

**Type:** Number

### ChartPoint.ArcStartPointYPx property {#arcstartpointypx}

Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart.

**Type:** Number

### ChartPoint.ArcEndPointXPx property {#arcendpointxpx}

Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart.

**Type:** Number

### ChartPoint.ArcEndPointYPx property {#arcendpointypx}

Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Pie and Doughnut chart.

**Type:** Number

### ChartPoint.InnerArcStartPointXPx property {#innerarcstartpointxpx}

Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.

**Type:** Number

### ChartPoint.InnerArcStartPointYPx property {#innerarcstartpointypx}

Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.

**Type:** Number

### ChartPoint.InnerArcEndPointXPx property {#innerarcendpointxpx}

Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.

**Type:** Number

### ChartPoint.InnerArcEndPointYPx property {#innerarcendpointypx}

Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method. Applies to Doughnut chart.

**Type:** Number

### getTopPointCount() {#gettoppointcount}

Gets the number of top points after calls Chart.Calculate() method.

### getTopPointXPx(index) {#gettoppointxpx}

Gets x-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D

### getTopPointYPx(index) {#gettoppointypx}

Gets y-coordinate of the top point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D

### getBottomPointCount() {#getbottompointcount}

Gets the number of bottom points after calls Chart.Calculate() method.

### getBottomPointXPx(index) {#getbottompointxpx}

Gets x-coordinate of the bottom point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid

### getBottomPointYPx(index) {#getbottompointypx}

Gets y-coordinate of the bottom point of shape after calls Chart.Calculate() method. Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid

### getOnCategoryAxisPointCount() {#getoncategoryaxispointcount}

Gets the number of the points on category axis after calls Chart.Calculate() method. Only applies to area chart.

Area 2D chart return 1 Area 3D chart return 2.

### getOnCategoryAxisPointXPx(index) {#getoncategoryaxispointxpx}

Gets x-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart.

Area 2D chart: index is 0. Area 3D chart: index is 0 or 1.

### getOnCategoryAxisPointYPx(index) {#getoncategoryaxispointypx}

Gets y-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart.

Area 2D chart: index is 0. Area 3D chart: index is 0 or 1.
