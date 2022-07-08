---
title: DataLabels
second_title: Aspose.Cells for .NET API Reference
description: Encapsulates a collection of all the DataLabel objects for the specified Series.
type: docs
weight: 580
url: /net/aspose.cells.charts/datalabels/
---
## DataLabels class

Encapsulates a collection of all the DataLabel objects for the specified Series.

```csharp
public class DataLabels : ChartTextFrame
```

## Properties

| Name | Description |
| --- | --- |
| override [Area](../../aspose.cells.charts/datalabels/area) { get; } | Gets the [`area`](./area). |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | True if the text in the object changes font size when the object size changes. The default value is True.(Inherited from [`ChartFrame`](../chartframe).) |
| [Background](../../aspose.cells.charts/chartframe/background) { get; set; } | (**Obsolete.**) Gets and sets the display mode of the background(Inherited from [`ChartFrame`](../chartframe).) |
| [BackgroundMode](../../aspose.cells.charts/datalabels/backgroundmode) { get; set; } | Gets and sets the display mode of the background |
| override [Border](../../aspose.cells.charts/datalabels/border) { get; } | Gets the [`border`](../../aspose.cells.drawing/line). |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Represents height of default position(Inherited from [`ChartFrame`](../chartframe).) |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Represents width of default position(Inherited from [`ChartFrame`](../chartframe).) |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Represents x of default position(Inherited from [`ChartFrame`](../chartframe).) |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Represents y of default position(Inherited from [`ChartFrame`](../chartframe).) |
| override [DirectionType](../../aspose.cells.charts/datalabels/directiontype) { get; set; } | Gets and sets the direction of text. |
| override [Font](../../aspose.cells.charts/datalabels/font) { get; } | Gets the font of the DataLabels; |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Gets or sets the height of frame in units of 1/4000 of the chart area.(Inherited from [`ChartFrame`](../chartframe).) |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Indicates whether the chart frame is automatic sized.(Inherited from [`ChartFrame`](../chartframe).) |
| override [IsAutoText](../../aspose.cells.charts/datalabels/isautotext) { get; set; } | Indicates the text is auto generated. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set.(Inherited from [`ChartFrame`](../chartframe).) |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Indicates whether this data labels is deleted.(Inherited from [`ChartTextFrame`](../charttextframe).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels.(Inherited from [`ChartFrame`](../chartframe).) |
| [IsNeverOverlap](../../aspose.cells.charts/datalabels/isneveroverlap) { get; set; } | Indicates whether the datalabels display never overlap. (For Pie chart) |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside.(Inherited from [`ChartTextFrame`](../charttextframe).) |
| override [IsTextWrapped](../../aspose.cells.charts/datalabels/istextwrapped) { get; set; } | Gets or sets a value indicating whether the text is wrapped. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Gets and sets a reference to the worksheet.(Inherited from [`ChartTextFrame`](../charttextframe).) |
| [Number](../../aspose.cells.charts/datalabels/number) { get; set; } | Gets and sets the built-in number format. |
| [NumberFormat](../../aspose.cells.charts/datalabels/numberformat) { get; set; } | Represents the format string for the DataLabels object. |
| [NumberFormatLinked](../../aspose.cells.charts/datalabels/numberformatlinked) { get; set; } | True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells). |
| [Position](../../aspose.cells.charts/datalabels/position) { get; set; } | Represents the position of the data label. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Represents text reading order.(Inherited from [`ChartTextFrame`](../charttextframe).) |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Represents text rotation angle.(Inherited from [`ChartTextFrame`](../charttextframe).) |
| [Separator](../../aspose.cells.charts/datalabels/separator) { get; set; } | (**Obsolete.**) Gets or sets the separator type used for the data labels on a chart. |
| [SeparatorType](../../aspose.cells.charts/datalabels/separatortype) { get; set; } | Gets or sets the separator type used for the data labels on a chart. |
| [SeparatorValue](../../aspose.cells.charts/datalabels/separatorvalue) { get; set; } | Gets or sets the separator value used for the data labels on a chart. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | True if the frame has a shadow.(Inherited from [`ChartFrame`](../chartframe).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Gets the [`ShapeProperties`](../chartframe/shapeproperties) object.(Inherited from [`ChartFrame`](../chartframe).) |
| [ShapeType](../../aspose.cells.charts/datalabels/shapetype) { get; set; } | Gets or sets shape type of data label. |
| [ShowBubbleSize](../../aspose.cells.charts/datalabels/showbubblesize) { get; set; } | Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide. |
| [ShowCategoryName](../../aspose.cells.charts/datalabels/showcategoryname) { get; set; } | Represents a specified chart's data label category name display behavior.True to display the category name for the data labels on a chart. False to hide. |
| [ShowCellRange](../../aspose.cells.charts/datalabels/showcellrange) { get; set; } | Indicates whether showing cell range as the data labels. |
| [ShowLegendKey](../../aspose.cells.charts/datalabels/showlegendkey) { get; set; } | Represents a specified chart's data label legend key display behavior. True if the data label legend key is visible. |
| [ShowPercentage](../../aspose.cells.charts/datalabels/showpercentage) { get; set; } | Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide. |
| [ShowSeriesName](../../aspose.cells.charts/datalabels/showseriesname) { get; set; } | Returns or sets a Boolean to indicate the series name display behavior for the data labels on a chart. True to show the series name. False to hide. |
| [ShowValue](../../aspose.cells.charts/datalabels/showvalue) { get; set; } | Represents a specified chart's data label values display behavior. True displays the values. False to hide. |
| override [Text](../../aspose.cells.charts/datalabels/text) { get; set; } | Gets or sets the text of data label. |
| [TextDirection](../../aspose.cells.charts/charttextframe/textdirection) { get; set; } | (**Obsolete.**) Represents text reading order.(Inherited from [`ChartTextFrame`](../charttextframe).) |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont) { get; } | (**Obsolete.**) Gets a [`Font`](../chartframe/font) object of the specified ChartFrame object.(Inherited from [`ChartFrame`](../chartframe).) |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | Gets and sets the text horizontal alignment.(Inherited from [`ChartTextFrame`](../charttextframe).) |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | Gets or sets the text vertical alignment of text.(Inherited from [`ChartTextFrame`](../charttextframe).) |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | Gets or sets the width of frame in units of 1/4000 of the chart area.(Inherited from [`ChartFrame`](../chartframe).) |
| virtual [X](../../aspose.cells.charts/chartframe/x) { get; set; } | Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area.(Inherited from [`ChartFrame`](../chartframe).) |
| virtual [Y](../../aspose.cells.charts/chartframe/y) { get; set; } | Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area.(Inherited from [`ChartFrame`](../chartframe).) |

## Methods

| Name | Description |
| --- | --- |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | Returns a Characters object that represents a range of characters within the text.(Inherited from [`ChartTextFrame`](../charttextframe).) |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Set position of the frame to automatic(Inherited from [`ChartFrame`](../chartframe).) |

### Examples

```csharp

[C#]

//Set the DataLabels in the chart
DataLabels datalabels;
for (int i = 0; i  <chart.NSeries.Count; i++)
{
    datalabels = chart.NSeries[i].DataLabels;
    //Set the position of DataLabels
    datalabels.Position = LabelPositionType.InsideBase;
    //Show the category name in the DataLabels
    datalabels.ShowCategoryName = true;
    //Show the value in the DataLabels
    datalabels.ShowValue = true;
    //Not show the percentage in the DataLabels
    datalabels.ShowPercentage = false;
    //Not show the legend key.
    datalabels.ShowLegendKey = false;
}

[Visual Basic]

'Set the DataLabels in the chart
Dim datalabels As DataLabels
Dim i As Integer
For i = 0 To chart.NSeries.Count - 1 Step 1
    datalabels = chart.NSeries(i).DataLabels
    'Set the position of DataLabels
    datalabels.Position = LabelPositionType.InsideBase
    'Show the category name in the DataLabels
    datalabels.ShowCategoryName= True
    'Show the value in the DataLabels
    datalabels.ShowValue = True
    'Not show the percentage in the DataLabels
    datalabels.ShowPercentage = False
    'Not show the legend key.
    datalabels.ShowLegendKey = False
Next
```

### See Also

* class [ChartTextFrame](../charttextframe)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
