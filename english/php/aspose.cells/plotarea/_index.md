---
title: "PlotArea Class"
linktitle: "PlotArea"
articleTitle: "PlotArea"
second_title: "Aspose.Cells for PHP via Java"
description: "Encapsulates the object that represents the plot area in a chart."
type: docs
weight: 4930
url: /php/aspose.cells/plotarea/
---

## PlotArea class

Encapsulates the object that represents the plot area in a chart.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [X](#x) | Number | Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of 1/4000 of the chart area. T |
| [Y](#y) | Number | Gets or gets the y coordinate of the upper top corner of plot-area bounding box in units of 1/4000 of the chart area. Th |
| [Height](#height) | Number | Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box inclu |
| [Width](#width) | Number | Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includ |
| [InnerX](#innerx) | Number | Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. The plot-area b |
| [InnerY](#innery) | Number | Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. The plot-area b |
| [InnerHeight](#innerheight) | Number | Gets or sets the height of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot  |
| [InnerWidth](#innerwidth) | Number | Gets or sets the width of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot a |
| [XRatioToChart](#xratiotochart) | Number |  |
| [YRatioToChart](#yratiotochart) | Number |  |
| [HeightRatioToChart](#heightratiotochart) | Number |  |
| [WidthRatioToChart](#widthratiotochart) | Number |  |
| [InnerXRatioToChart](#innerxratiotochart) | Number |  |
| [InnerYRatioToChart](#inneryratiotochart) | Number |  |
| [InnerHeightRatioToChart](#innerheightratiotochart) | Number |  |
| [InnerWidthRatioToChart](#innerwidthratiotochart) | Number |  |
| [IsAutomaticSize](#isautomaticsize) | boolean | Indicates whether the plot area is automatic sized. |
| [IsInnerMode](#isinnermode) | boolean | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the  |
| [Chart](#chart) | Chart | Gets the chart to which this object belongs. |
| [Border](#border) | Line | Gets the Line . |
| [Area](#area) | Area | Gets the area . |
| [TextFont](#textfont) | Font | Gets a Font object of the specified ChartFrame object. NOTE: This member is now obsolete. Instead, please use ChartFrame |
| [TextOptions](#textoptions) | TextOptions | Gets and sets the options of the text. |
| [Font](#font) | Font | Gets a Font object of the specified ChartFrame object. |
| [AutoScaleFont](#autoscalefont) | boolean | True if the text in the object changes font size when the object size changes. The default value is True. |
| [BackgroundMode](#backgroundmode) | Number | Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. |
| [Background](#background) | Number | Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. NOTE: Thi |
| [Shadow](#shadow) | boolean | True if the frame has a shadow. |
| [ShapeProperties](#shapeproperties) | ShapePropertyCollection | Gets the ShapeProperties object. |
| [IsDefaultPosBeSet](#isdefaultposbeset) | boolean | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [DefaultX](#defaultx) | Number | Represents x of default position |
| [DefaultY](#defaulty) | Number | Represents y of default position |
| [DefaultWidth](#defaultwidth) | Number | Represents width of default position |
| [DefaultHeight](#defaultheight) | Number | Represents height of default position |
| [DefaultXRatioToChart](#defaultxratiotochart) | Number |  |
| [DefaultYRatioToChart](#defaultyratiotochart) | Number |  |
| [DefaultWidthRatioToChart](#defaultwidthratiotochart) | Number |  |
| [DefaultHeightRatioToChart](#defaultheightratiotochart) | Number |  |
| [XPixel](#xpixel) | Number |  |
| [YPixel](#ypixel) | Number |  |
| [WidthPixel](#widthpixel) | Number | Represents width |
| [HeightPixel](#heightpixel) | Number | Represents height |

## Methods

| Name | Description |
| --- | --- |
| [setPositionAuto](#setpositionauto) | Set position of the plot area to automatic |

### PlotArea.X property {#x}

Gets or gets the x coordinate of the upper left corner of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X , Y , Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX , InnerY , InnerWidth and InnerHeight properties. For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

**Type:** Number

### PlotArea.Y property {#y}

Gets or gets the y coordinate of the upper top corner of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X , Y , Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX , InnerY , InnerWidth and InnerHeight properties. For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

**Type:** Number

### PlotArea.Height property {#height}

Gets or sets the height of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X , Y , Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX , InnerY , InnerWidth and InnerHeight properties. For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

**Type:** Number

### PlotArea.Width property {#width}

Gets or sets the width of plot-area bounding box in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X , Y , Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX , InnerY , InnerWidth and InnerHeight properties. For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

**Type:** Number

### PlotArea.InnerX property {#innerx}

Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X , Y , Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX , InnerY , InnerWidth and InnerHeight properties. For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

**Type:** Number

### PlotArea.InnerY property {#innery}

Gets or gets the x coordinate of the upper top corner of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X , Y , Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX , InnerY , InnerWidth and InnerHeight properties. For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

**Type:** Number

### PlotArea.InnerHeight property {#innerheight}

Gets or sets the height of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X , Y , Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX , InnerY , InnerWidth and InnerHeight properties. For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

**Type:** Number

### PlotArea.InnerWidth property {#innerwidth}

Gets or sets the width of plot area in units of 1/4000 of the chart area. The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks. If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method. The X , Y , Width and Height of PlotArea represents the plot-area bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks. If you want to get actual size of plot area, you should call InnerX , InnerY , InnerWidth and InnerHeight properties. For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().

**Type:** Number

### PlotArea.XRatioToChart property {#xratiotochart}

**Type:** Number

### PlotArea.YRatioToChart property {#yratiotochart}

**Type:** Number

### PlotArea.HeightRatioToChart property {#heightratiotochart}

**Type:** Number

### PlotArea.WidthRatioToChart property {#widthratiotochart}

**Type:** Number

### PlotArea.InnerXRatioToChart property {#innerxratiotochart}

**Type:** Number

### PlotArea.InnerYRatioToChart property {#inneryratiotochart}

**Type:** Number

### PlotArea.InnerHeightRatioToChart property {#innerheightratiotochart}

**Type:** Number

### PlotArea.InnerWidthRatioToChart property {#innerwidthratiotochart}

**Type:** Number

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

**Type:** Number

### PlotArea.Background property {#background}

Gets and sets the display mode of the background The value of the property is BackgroundMode integer constant. NOTE: This member is now obsolete. Instead, please use ChartFrame.BackgroundMode property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Type:** Number

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

**Type:** Number

### PlotArea.DefaultY property {#defaulty}

Represents y of default position

**Type:** Number

### PlotArea.DefaultWidth property {#defaultwidth}

Represents width of default position

**Type:** Number

### PlotArea.DefaultHeight property {#defaultheight}

Represents height of default position

**Type:** Number

### PlotArea.DefaultXRatioToChart property {#defaultxratiotochart}

**Type:** Number

### PlotArea.DefaultYRatioToChart property {#defaultyratiotochart}

**Type:** Number

### PlotArea.DefaultWidthRatioToChart property {#defaultwidthratiotochart}

**Type:** Number

### PlotArea.DefaultHeightRatioToChart property {#defaultheightratiotochart}

**Type:** Number

### PlotArea.XPixel property {#xpixel}

**Type:** Number

### PlotArea.YPixel property {#ypixel}

**Type:** Number

### PlotArea.WidthPixel property {#widthpixel}

Represents width

**Type:** Number

### PlotArea.HeightPixel property {#heightpixel}

Represents height

**Type:** Number

### setPositionAuto() {#setpositionauto}

Set position of the plot area to automatic
