---
title: "PlotArea"
linktitle: "PlotArea"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates the object that represents the plot area in a chart."
type: docs
weight: 2960
url: /nodejs/aspose.cells/plotarea/
---

## PlotArea class

Encapsulates the object that represents the plot area in a chart.

## Methods

| Name | Description |
| --- | --- |
| [getArea()](#getarea) | Gets the area. |
| [getAutoScaleFont()](#getautoscalefont) | True if the text in the object changes font size when the object size changes. The default value is True. |
| [getBackground()](#getbackground) | Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant.NOTE: This |
| [getBackgroundMode()](#getbackgroundmode) | Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. |
| [getBorder()](#getborder) | Gets the Line. |
| [getChart()](#getchart) | Gets the chart to which this object belongs. |
| [getDefaultHeight()](#getdefaultheight) | Represents height of default position |
| [getDefaultHeightRatioToChart()](#getdefaultheightratiotochart) |  |
| [getDefaultWidth()](#getdefaultwidth) | Represents width of default position |
| [getDefaultWidthRatioToChart()](#getdefaultwidthratiotochart) |  |
| [getDefaultX()](#getdefaultx) | Represents x of default position |
| [getDefaultXRatioToChart()](#getdefaultxratiotochart) |  |
| [getDefaultY()](#getdefaulty) | Represents y of default position |
| [getDefaultYRatioToChart()](#getdefaultyratiotochart) |  |
| [getFont()](#getfont) | Gets a Font object of the specified ChartFrame object. |
| [getHeight()](#getheight) | Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box inclu |
| [getHeightPixel()](#getheightpixel) | Represents height |
| [getHeightRatioToChart()](#getheightratiotochart) |  |
| [getInnerHeight()](#getinnerheight) | Gets or sets the height of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot  |
| [getInnerHeightRatioToChart()](#getinnerheightratiotochart) |  |
| [getInnerWidth()](#getinnerwidth) | Gets or sets the width of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot a |
| [getInnerWidthRatioToChart()](#getinnerwidthratiotochart) |  |
| [getInnerX()](#getinnerx) | Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. The plot-area b |
| [getInnerXRatioToChart()](#getinnerxratiotochart) |  |
| [getInnerY()](#getinnery) | Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. The plot-area b |
| [getInnerYRatioToChart()](#getinneryratiotochart) |  |
| [getShadow()](#getshadow) | True if the frame has a shadow. |
| [getShapeProperties()](#getshapeproperties) | Gets the ShapeProperties object. |
| [getTextFont()](#gettextfont) | Gets a Font object of the specified ChartFrame object. NOTE: This member is now obsolete. Instead, please use ChartFrame |
| [getTextOptions()](#gettextoptions) | Gets and sets the options of the text. |
| [getWidth()](#getwidth) | Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includ |
| [getWidthPixel()](#getwidthpixel) | Represents width |
| [getWidthRatioToChart()](#getwidthratiotochart) |  |
| [getX()](#getx) | Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of 1/4000 of the chart area. T |
| [getXPixel()](#getxpixel) |  |
| [getXRatioToChart()](#getxratiotochart) |  |
| [getY()](#gety) | Gets or gets the y coordinate of the upper top corner of plot-area bounding box in units of 1/4000 of the chart area. Th |
| [getYPixel()](#getypixel) |  |
| [getYRatioToChart()](#getyratiotochart) |  |
| [isAutomaticSize()](#isautomaticsize) | Indicates whether the plot area is automatic sized. |
| [isDefaultPosBeSet()](#isdefaultposbeset) | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [isInnerMode()](#isinnermode) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the  |
| [setAutoScaleFont()](#setautoscalefont) | True if the text in the object changes font size when the object size changes. The default value is True. |
| [setAutomaticSize()](#setautomaticsize) | Indicates whether the plot area is automatic sized. |
| [setBackground()](#setbackground) | Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant.NOTE: This |
| [setBackgroundMode()](#setbackgroundmode) | Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. |
| [setHeight()](#setheight) | Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box inclu |
| [setHeightPixel()](#setheightpixel) | Represents height |
| [setHeightRatioToChart()](#setheightratiotochart) |  |
| [setInnerHeight()](#setinnerheight) | Gets or sets the height of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot  |
| [setInnerHeightRatioToChart()](#setinnerheightratiotochart) |  |
| [setInnerMode()](#setinnermode) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the  |
| [setInnerWidth()](#setinnerwidth) | Gets or sets the width of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot a |
| [setInnerWidthRatioToChart()](#setinnerwidthratiotochart) |  |
| [setInnerX()](#setinnerx) | Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. The plot-area b |
| [setInnerXRatioToChart()](#setinnerxratiotochart) |  |
| [setInnerY()](#setinnery) | Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. The plot-area b |
| [setInnerYRatioToChart()](#setinneryratiotochart) |  |
| [setPositionAuto()](#setpositionauto) | Set position of the plot area to automatic |
| [setShadow()](#setshadow) | True if the frame has a shadow. |
| [setWidth()](#setwidth) | Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includ |
| [setWidthPixel()](#setwidthpixel) | Represents width |
| [setWidthRatioToChart()](#setwidthratiotochart) |  |
| [setX()](#setx) | Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of 1/4000 of the chart area. T |
| [setXPixel()](#setxpixel) |  |
| [setXRatioToChart()](#setxratiotochart) |  |
| [setY()](#sety) | Gets or gets the y coordinate of the upper top corner of plot-area bounding box in units of 1/4000 of the chart area. Th |
| [setYPixel()](#setypixel) |  |
| [setYRatioToChart()](#setyratiotochart) |  |

### getArea() {#getarea}

Gets the area.

### getAutoScaleFont() {#getautoscalefont}

True if the text in the object changes font size when the object size changes. The default value is True.

### getBackground() {#getbackground}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant.NOTE: This member is now obsolete. Instead, please use ChartFrame.BackgroundMode property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

### getBackgroundMode() {#getbackgroundmode}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant.

### getBorder() {#getborder}

Gets the Line.

### getChart() {#getchart}

Gets the chart to which this object belongs.

### getDefaultHeight() {#getdefaultheight}

Represents height of default position

### getDefaultHeightRatioToChart() {#getdefaultheightratiotochart}

### getDefaultWidth() {#getdefaultwidth}

Represents width of default position

### getDefaultWidthRatioToChart() {#getdefaultwidthratiotochart}

### getDefaultX() {#getdefaultx}

Represents x of default position

### getDefaultXRatioToChart() {#getdefaultxratiotochart}

### getDefaultY() {#getdefaulty}

Represents y of default position

### getDefaultYRatioToChart() {#getdefaultyratiotochart}

### getFont() {#getfont}

Gets a Font object of the specified ChartFrame object.

### getHeight() {#getheight}

Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X, Y, Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX, InnerY, InnerWidth and InnerHeight properties.For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

### getHeightPixel() {#getheightpixel}

Represents height

### getHeightRatioToChart() {#getheightratiotochart}

### getInnerHeight() {#getinnerheight}

Gets or sets the height of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X, Y, Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX, InnerY, InnerWidth and InnerHeight properties.For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

### getInnerHeightRatioToChart() {#getinnerheightratiotochart}

### getInnerWidth() {#getinnerwidth}

Gets or sets the width of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X, Y, Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX, InnerY, InnerWidth and InnerHeight properties.For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

### getInnerWidthRatioToChart() {#getinnerwidthratiotochart}

### getInnerX() {#getinnerx}

Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X, Y, Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX, InnerY, InnerWidth and InnerHeight properties.For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

### getInnerXRatioToChart() {#getinnerxratiotochart}

### getInnerY() {#getinnery}

Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X, Y, Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX, InnerY, InnerWidth and InnerHeight properties.For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

### getInnerYRatioToChart() {#getinneryratiotochart}

### getShadow() {#getshadow}

True if the frame has a shadow.

### getShapeProperties() {#getshapeproperties}

Gets the ShapeProperties object.

### getTextFont() {#gettextfont}

Gets a Font object of the specified ChartFrame object. NOTE: This member is now obsolete. Instead, please use ChartFrame.Font property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

### getTextOptions() {#gettextoptions}

Gets and sets the options of the text.

### getWidth() {#getwidth}

Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X, Y, Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX, InnerY, InnerWidth and InnerHeight properties.For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

### getWidthPixel() {#getwidthpixel}

Represents width

### getWidthRatioToChart() {#getwidthratiotochart}

### getX() {#getx}

Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X, Y, Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX, InnerY, InnerWidth and InnerHeight properties.For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

### getXPixel() {#getxpixel}

### getXRatioToChart() {#getxratiotochart}

### getY() {#gety}

Gets or gets the y coordinate of the upper top corner of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X, Y, Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX, InnerY, InnerWidth and InnerHeight properties.For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

### getYPixel() {#getypixel}

### getYRatioToChart() {#getyratiotochart}

### isAutomaticSize() {#isautomaticsize}

Indicates whether the plot area is automatic sized.

### isDefaultPosBeSet() {#isdefaultposbeset}

Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set.

### isInnerMode() {#isinnermode}

Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. Only for Xlsx file.

### setAutoScaleFont() {#setautoscalefont}

True if the text in the object changes font size when the object size changes. The default value is True.

### setAutomaticSize() {#setautomaticsize}

Indicates whether the plot area is automatic sized.

### setBackground() {#setbackground}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant.NOTE: This member is now obsolete. Instead, please use ChartFrame.BackgroundMode property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

### setBackgroundMode() {#setbackgroundmode}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant.

### setHeight() {#setheight}

Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X, Y, Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX, InnerY, InnerWidth and InnerHeight properties.For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

### setHeightPixel() {#setheightpixel}

Represents height

### setHeightRatioToChart() {#setheightratiotochart}

### setInnerHeight() {#setinnerheight}

Gets or sets the height of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X, Y, Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX, InnerY, InnerWidth and InnerHeight properties.For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

### setInnerHeightRatioToChart() {#setinnerheightratiotochart}

### setInnerMode() {#setinnermode}

Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. Only for Xlsx file.

### setInnerWidth() {#setinnerwidth}

Gets or sets the width of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X, Y, Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX, InnerY, InnerWidth and InnerHeight properties.For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

### setInnerWidthRatioToChart() {#setinnerwidthratiotochart}

### setInnerX() {#setinnerx}

Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X, Y, Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX, InnerY, InnerWidth and InnerHeight properties.For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

### setInnerXRatioToChart() {#setinnerxratiotochart}

### setInnerY() {#setinnery}

Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X, Y, Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX, InnerY, InnerWidth and InnerHeight properties.For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

### setInnerYRatioToChart() {#setinneryratiotochart}

### setPositionAuto() {#setpositionauto}

Set position of the plot area to automatic

### setShadow() {#setshadow}

True if the frame has a shadow.

### setWidth() {#setwidth}

Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X, Y, Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX, InnerY, InnerWidth and InnerHeight properties.For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

### setWidthPixel() {#setwidthpixel}

Represents width

### setWidthRatioToChart() {#setwidthratiotochart}

### setX() {#setx}

Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X, Y, Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX, InnerY, InnerWidth and InnerHeight properties.For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

### setXPixel() {#setxpixel}

### setXRatioToChart() {#setxratiotochart}

### setY() {#sety}

Gets or gets the y coordinate of the upper top corner of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X, Y, Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX, InnerY, InnerWidth and InnerHeight properties.For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

### setYPixel() {#setypixel}

### setYRatioToChart() {#setyratiotochart}
