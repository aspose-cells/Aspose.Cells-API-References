---
title: ChartTextFrame
second_title: Aspose.Cells for .NET API Reference
description: Encapsulates the object that represents the frame object which contains text.
type: docs
url: /net/aspose.cells.charts/charttextframe/
---
## ChartTextFrame class

Encapsulates the object that represents the frame object which contains text.

```csharp
public class ChartTextFrame : ChartFrame
```

## Properties

| Name | Description |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | Gets the [`area`](../chartframe/area).(Inherited from [`ChartFrame`](../chartframe).) |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | True if the text in the object changes font size when the object size changes. The default value is True.(Inherited from [`ChartFrame`](../chartframe).) |
| [Background](../../aspose.cells.charts/chartframe/background) { get; set; } | (**Obsolete.**) Gets and sets the display mode of the background(Inherited from [`ChartFrame`](../chartframe).) |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | Gets and sets the display mode of the background(Inherited from [`ChartFrame`](../chartframe).) |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | Gets the [`border`](../../aspose.cells.drawing/line).(Inherited from [`ChartFrame`](../chartframe).) |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Represents height of default position(Inherited from [`ChartFrame`](../chartframe).) |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Represents width of default position(Inherited from [`ChartFrame`](../chartframe).) |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Represents x of default position(Inherited from [`ChartFrame`](../chartframe).) |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Represents y of default position(Inherited from [`ChartFrame`](../chartframe).) |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | Gets and sets the direction of text. |
| virtual [Font](../../aspose.cells.charts/chartframe/font) { get; } | Gets a [`Font`](../chartframe/font) object of the specified ChartFrame object.(Inherited from [`ChartFrame`](../chartframe).) |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | Gets or sets the height of frame in units of 1/4000 of the chart area.(Inherited from [`ChartFrame`](../chartframe).) |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Indicates whether the chart frame is automatic sized.(Inherited from [`ChartFrame`](../chartframe).) |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | Indicates the text is auto generated. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set.(Inherited from [`ChartFrame`](../chartframe).) |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | Indicates whether this data labels is deleted. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels.(Inherited from [`ChartFrame`](../chartframe).) |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | Gets or sets a value indicating whether the text is wrapped. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | Gets and sets a reference to the worksheet. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | Represents text reading order. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | Represents text rotation angle. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | True if the frame has a shadow.(Inherited from [`ChartFrame`](../chartframe).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Gets the [`ShapeProperties`](../chartframe/shapeproperties) object.(Inherited from [`ChartFrame`](../chartframe).) |
| virtual [Text](../../aspose.cells.charts/charttextframe/text) { get; set; } | Gets or sets the text of a frame's title. |
| [TextDirection](../../aspose.cells.charts/charttextframe/textdirection) { get; set; } | (**Obsolete.**) Represents text reading order. |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont) { get; } | (**Obsolete.**) Gets a [`Font`](../chartframe/font) object of the specified ChartFrame object.(Inherited from [`ChartFrame`](../chartframe).) |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | Gets and sets the text horizontal alignment. |
| virtual [TextOptions](../../aspose.cells.charts/chartframe/textoptions) { get; } | Gets and sets the options of the text.(Inherited from [`ChartFrame`](../chartframe).) |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | Gets or sets the text vertical alignment of text. |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | Gets or sets the width of frame in units of 1/4000 of the chart area.(Inherited from [`ChartFrame`](../chartframe).) |
| virtual [X](../../aspose.cells.charts/chartframe/x) { get; set; } | Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area.(Inherited from [`ChartFrame`](../chartframe).) |
| virtual [Y](../../aspose.cells.charts/chartframe/y) { get; set; } | Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area.(Inherited from [`ChartFrame`](../chartframe).) |

## Methods

| Name | Description |
| --- | --- |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | Returns a Characters object that represents a range of characters within the text. |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Set position of the frame to automatic(Inherited from [`ChartFrame`](../chartframe).) |

### See Also

* class [ChartFrame](../chartframe)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
