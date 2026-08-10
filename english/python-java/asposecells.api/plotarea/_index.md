---
title: "PlotArea Class"
linktitle: "PlotArea"
articleTitle: "PlotArea"
second_title: "Aspose.Cells for Python via Java"
description: "Encapsulates the object that represents the plot area in a chart."
type: docs
weight: 4930
url: /python-java/asposecells.api/plotarea/
---

## PlotArea class

Encapsulates the object that represents the plot area in a chart.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [X](#x) | int | Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of 1/4000 of the chart area. T |
| [Y](#y) | int | Gets or gets the y coordinate of the upper top corner of plot-area bounding box in units of 1/4000 of the chart area. Th |
| [Height](#height) | int | Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box inclu |
| [Width](#width) | int | Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includ |
| [InnerX](#innerx) | int | Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. The plot-area b |
| [InnerY](#innery) | int | Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. The plot-area b |
| [InnerHeight](#innerheight) | int | Gets or sets the height of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot  |
| [InnerWidth](#innerwidth) | int | Gets or sets the width of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot a |
| [XRatioToChart](#xratiotochart) | float |  |
| [YRatioToChart](#yratiotochart) | float |  |
| [HeightRatioToChart](#heightratiotochart) | float |  |
| [WidthRatioToChart](#widthratiotochart) | float |  |
| [InnerXRatioToChart](#innerxratiotochart) | float |  |
| [InnerYRatioToChart](#inneryratiotochart) | float |  |
| [InnerHeightRatioToChart](#innerheightratiotochart) | float |  |
| [InnerWidthRatioToChart](#innerwidthratiotochart) | float |  |
| [IsAutomaticSize](#isautomaticsize) | boolean | Indicates whether the plot area is automatic sized. |
| [IsInnerMode](#isinnermode) | boolean | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the  |
| [Chart](#chart) | Chart | Gets the chart to which this object belongs. |
| [Border](#border) | Line | Gets the Line . |
| [Area](#area) | Area | Gets the area . |
| [TextFont](#textfont) | Font | Gets a Font object of the specified ChartFrame object. NOTE: This member is now obsolete. Instead, please use ChartFrame |
| [TextOptions](#textoptions) | TextOptions | Gets and sets the options of the text. |
| [Font](#font) | Font | Gets a Font object of the specified ChartFrame object. |
| [AutoScaleFont](#autoscalefont) | boolean | True if the text in the object changes font size when the object size changes. The default value is True. |
| [BackgroundMode](#backgroundmode) | int | Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. |
| [Background](#background) | int | Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. NOTE: Thi |
| [Shadow](#shadow) | boolean | True if the frame has a shadow. |
| [ShapeProperties](#shapeproperties) | ShapePropertyCollection | Gets the ShapeProperties object. |
| [IsDefaultPosBeSet](#isdefaultposbeset) | boolean | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [DefaultX](#defaultx) | int | Represents x of default position |
| [DefaultY](#defaulty) | int | Represents y of default position |
| [DefaultWidth](#defaultwidth) | int | Represents width of default position |
| [DefaultHeight](#defaultheight) | int | Represents height of default position |
| [DefaultXRatioToChart](#defaultxratiotochart) | float |  |
| [DefaultYRatioToChart](#defaultyratiotochart) | float |  |
| [DefaultWidthRatioToChart](#defaultwidthratiotochart) | float |  |
| [DefaultHeightRatioToChart](#defaultheightratiotochart) | float |  |
| [XPixel](#xpixel) | int |  |
| [YPixel](#ypixel) | int |  |
| [WidthPixel](#widthpixel) | int | Represents width |
| [HeightPixel](#heightpixel) | int | Represents height |

## Methods

| Name | Description |
| --- | --- |
| [setPositionAuto](#setpositionauto) | Set position of the plot area to automatic |

### PlotArea.X property {#x}

Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X , Y , Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX , InnerY , InnerWidth and InnerHeight properties. For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

**Type:** int

### PlotArea.Y property {#y}

Gets or gets the y coordinate of the upper top corner of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X , Y , Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX , InnerY , InnerWidth and InnerHeight properties. For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

**Type:** int

### PlotArea.Height property {#height}

Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X , Y , Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX , InnerY , InnerWidth and InnerHeight properties. For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

**Type:** int

### PlotArea.Width property {#width}

Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X , Y , Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX , InnerY , InnerWidth and InnerHeight properties. For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

**Type:** int

### PlotArea.InnerX property {#innerx}

Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X , Y , Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX , InnerY , InnerWidth and InnerHeight properties. For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

**Type:** int

### PlotArea.InnerY property {#innery}

Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X , Y , Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX , InnerY , InnerWidth and InnerHeight properties. For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

**Type:** int

### PlotArea.InnerHeight property {#innerheight}

Gets or sets the height of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X , Y , Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX , InnerY , InnerWidth and InnerHeight properties. For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

**Type:** int

### PlotArea.InnerWidth property {#innerwidth}

Gets or sets the width of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X , Y , Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX , InnerY , InnerWidth and InnerHeight properties. For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

**Type:** int

### PlotArea.XRatioToChart property {#xratiotochart}

**Type:** float

### PlotArea.YRatioToChart property {#yratiotochart}

**Type:** float

### PlotArea.HeightRatioToChart property {#heightratiotochart}

**Type:** float

### PlotArea.WidthRatioToChart property {#widthratiotochart}

**Type:** float

### PlotArea.InnerXRatioToChart property {#innerxratiotochart}

**Type:** float

### PlotArea.InnerYRatioToChart property {#inneryratiotochart}

**Type:** float

### PlotArea.InnerHeightRatioToChart property {#innerheightratiotochart}

**Type:** float

### PlotArea.InnerWidthRatioToChart property {#innerwidthratiotochart}

**Type:** float

### PlotArea.IsAutomaticSize property {#isautomaticsize}

Indicates whether the plot area is automatic sized.

**Type:** boolean

### PlotArea.IsInnerMode property {#isinnermode}

Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. Only for Xlsx file.

**Type:** boolean

### PlotArea.Chart property {#chart}

Gets the chart to which this object belongs.

**Type:** Chart

### PlotArea.Border property {#border}

Gets the Line .

**Type:** Line

### PlotArea.Area property {#area}

Gets the area .

**Type:** Area

### PlotArea.TextFont property {#textfont}

Gets a Font object of the specified ChartFrame object. NOTE: This member is now obsolete. Instead, please use ChartFrame.Font property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Type:** Font

### PlotArea.TextOptions property {#textoptions}

Gets and sets the options of the text.

**Type:** TextOptions

### PlotArea.Font property {#font}

Gets a Font object of the specified ChartFrame object.

**Type:** Font

### PlotArea.AutoScaleFont property {#autoscalefont}

True if the text in the object changes font size when the object size changes. The default value is True.

**Type:** boolean

### PlotArea.BackgroundMode property {#backgroundmode}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant.

**Type:** int

### PlotArea.Background property {#background}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. NOTE: This member is now obsolete. Instead, please use ChartFrame.BackgroundMode property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Type:** int

### PlotArea.Shadow property {#shadow}

True if the frame has a shadow.

**Type:** boolean

### PlotArea.ShapeProperties property {#shapeproperties}

Gets the ShapeProperties object.

**Type:** ShapePropertyCollection

### PlotArea.IsDefaultPosBeSet property {#isdefaultposbeset}

Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set.

**Type:** boolean

### PlotArea.DefaultX property {#defaultx}

Represents x of default position

**Type:** int

### PlotArea.DefaultY property {#defaulty}

Represents y of default position

**Type:** int

### PlotArea.DefaultWidth property {#defaultwidth}

Represents width of default position

**Type:** int

### PlotArea.DefaultHeight property {#defaultheight}

Represents height of default position

**Type:** int

### PlotArea.DefaultXRatioToChart property {#defaultxratiotochart}

**Type:** float

### PlotArea.DefaultYRatioToChart property {#defaultyratiotochart}

**Type:** float

### PlotArea.DefaultWidthRatioToChart property {#defaultwidthratiotochart}

**Type:** float

### PlotArea.DefaultHeightRatioToChart property {#defaultheightratiotochart}

**Type:** float

### PlotArea.XPixel property {#xpixel}

**Type:** int

### PlotArea.YPixel property {#ypixel}

**Type:** int

### PlotArea.WidthPixel property {#widthpixel}

Represents width

**Type:** int

### PlotArea.HeightPixel property {#heightpixel}

Represents height

**Type:** int

### setPositionAuto() {#setpositionauto}

Set position of the plot area to automatic
