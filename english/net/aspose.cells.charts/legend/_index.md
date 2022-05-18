---
title: Legend
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 680
url: /net/aspose.cells.charts/legend/
---
## Legend class

Encapsulates the object that represents the chart legend.

```csharp
public class Legend : ChartTextFrame
```

## Properties

| Name | Description |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | Gets the [`area`](../chartframe/area). |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | True if the text in the object changes font size when the object size changes. The default value is True. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | Gets and sets the display mode of the background |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | Gets the [`border`](../../aspose.cells.drawing/line). |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Represents height of default position |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Represents width of default position |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Represents x of default position |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Represents y of default position |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | Gets and sets the direction of text. |
| virtual [Font](../../aspose.cells.charts/chartframe/font) { get; } | Gets a [`Font`](../chartframe/font) object of the specified ChartFrame object. |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Gets or sets the height of frame in units of 1/4000 of the chart area. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Indicates whether the chart frame is automatic sized. |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | Indicates the text is auto generated. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Indicates whether this data labels is deleted. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [IsOverLay](../../aspose.cells.charts/legend/isoverlay) { get; set; } | Gets or sets whether other chart elements shall be allowed to overlap this chart element. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Gets or sets a value indicating whether the text is wrapped. |
| [LegendEntries](../../aspose.cells.charts/legend/legendentries) { get; } | Gets a collection of all the LegendEntry objects in the specified chart legend. Setting the legend entries of the surface chart is not supported. So it will return null if the chart type is surface chart type. |
| [LegendEntriesLabels](../../aspose.cells.charts/legend/legendentrieslabels) { get; } | Gets the labels of the legend entries after call Chart.Calculate() method. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Gets and sets a reference to the worksheet. |
| [Position](../../aspose.cells.charts/legend/position) { get; set; } | Gets or sets the legend position type. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Represents text reading order. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Represents text rotation angle. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | True if the frame has a shadow. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Gets the [`ShapeProperties`](../chartframe/shapeproperties) object. |
| virtual [Text](../../aspose.cells.charts/charttextframe/text) { get; set; } | Gets or sets the text of a frame's title. |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | Gets and sets the text horizontal alignment. |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | Gets or sets the text vertical alignment of text. |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | Gets or sets the width of frame in units of 1/4000 of the chart area. |
| virtual [X](../../aspose.cells.charts/chartframe/x) { get; set; } | Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. |
| virtual [Y](../../aspose.cells.charts/chartframe/y) { get; set; } | Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. |

## Methods

| Name | Description |
| --- | --- |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | Returns a Characters object that represents a range of characters within the text. |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Set position of the frame to automatic |

### Examples

```csharp
[C#]
   
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];

Cells cells = sheet.Cells;
cells[0,1].PutValue("Income");
cells[1,0].PutValue("Company A");
cells[2,0].PutValue("Company B");
cells[3,0].PutValue("Company C");
cells[1,1].PutValue(10000);
cells[2,1].PutValue(20000);
cells[3,1].PutValue(30000);
		
int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
//Set Legend's width and height
Legend legend = chart.Legend;

//Legend is at right side of chart by default.
//If the legend is at left or right side of the chart, setting Legend.X property will not take effect.
//If the legend is at top or bottom side of the chart, setting Legend.Y property will not take effect.
legend.Y = 1500;
legend.Width = 50;
legend.Height = 50; 
//Set legend's position
legend.Position = LegendPositionType.Left;

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim sheet as Worksheet = workbook.Worksheets(0)

Dim cells as Cells = sheet.Cells
cells(0,1).PutValue("Income")
cells(1,0).PutValue("Company A")
cells(2,0).PutValue("Company B")
cells(3,0).PutValue("Company C")
cells(1,1).PutValue(10000)
cells(2,1).PutValue(20000)
cells(3,1).PutValue(30000)
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)

Dim chart as Chart = sheet.Charts(chartIndex)
chart.SetChartDataRange("A1:B4", True);
 
'Set Legend's width and height
Dim legend as Legend = chart.Legend

'Legend is at right side of chart by default.
'If the legend is at left or right side of the chart, setting Legend.X property will not take effect.
'If the legend is at top or bottom side of the chart, setting Legend.Y property will not take effect.
legend.Y = 1500
legend.Width = 50
legend.Height = 50
'Set legend's position
legend.Position = LegendPositionType.Left
```

### See Also

* class [ChartTextFrame](../charttextframe)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
