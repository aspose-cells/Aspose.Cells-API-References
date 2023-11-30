---
title: Aspose::Cells::Charts::ChartTextFrame class
linktitle: ChartTextFrame
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::ChartTextFrame class. Encapsulates the object that represents the frame object which contains text in C++.'
type: docs
weight: 1100
url: /cpp/aspose.cells.charts/charttextframe/
---
## ChartTextFrame class


Encapsulates the object that represents the frame object which contains text.

```cpp
class ChartTextFrame : public Aspose::Cells::Charts::ChartFrame
```

## Methods

| Method | Description |
| --- | --- |
| [Characters(int32_t startIndex, int32_t length)](./characters/) | Returns a Characters object that represents a range of characters within the text. |
| [ChartFrame(ChartFrame_Impl* impl)](../chartframe/chartframe/) | Constructs from an implementation object. |
| [ChartFrame(const ChartFrame\& src)](../chartframe/chartframe/) | Copy constructor. |
| [ChartTextFrame(ChartTextFrame_Impl* impl)](./charttextframe/) | Constructs from an implementation object. |
| [ChartTextFrame(const ChartTextFrame\& src)](./charttextframe/) | Copy constructor. |
| [ChartTextFrame(const ChartFrame\& src)](./charttextframe/) | Constructs from a parent object. |
| [GetArea()](../chartframe/getarea/) | Gets the [area](../). |
| [GetAutoScaleFont()](../chartframe/getautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
| [GetBackgroundMode()](../chartframe/getbackgroundmode/) | Gets and sets the display mode of the background. |
| [GetBorder()](../chartframe/getborder/) | Gets the [border](../). |
| [GetDefaultHeight()](../chartframe/getdefaultheight/) | Represents height of default position. |
| [GetDefaultWidth()](../chartframe/getdefaultwidth/) | Represents width of default position. |
| [GetDefaultX()](../chartframe/getdefaultx/) | Represents x of default position. |
| [GetDefaultY()](../chartframe/getdefaulty/) | Represents y of default position. |
| [GetDirectionType()](./getdirectiontype/) | Gets and sets the direction of text. |
| [GetFont()](../chartframe/getfont/) | Gets a [Font](../../aspose.cells/font/) object of the specified [ChartFrame](../chartframe/) object. |
| [GetHeight()](../chartframe/getheight/) | Gets or sets the height of frame in units of 1/4000 of the chart area. |
| [GetLinkedSource()](./getlinkedsource/) | Gets and sets a reference to the worksheet. |
| [GetReadingOrder()](./getreadingorder/) | Represents text reading order. |
| [GetRotationAngle()](./getrotationangle/) | Represents text rotation angle. |
| [GetShadow()](../chartframe/getshadow/) | True if the frame has a shadow. |
| [GetShapeProperties()](../chartframe/getshapeproperties/) | Gets the ShapeProperties object. |
| [GetText()](./gettext/) | Gets or sets the text of a frame's title. |
| [GetTextHorizontalAlignment()](./gettexthorizontalalignment/) | Gets and sets the text horizontal alignment. |
| [GetTextOptions()](../chartframe/gettextoptions/) | Gets and sets the options of the text. |
| [GetTextVerticalAlignment()](./gettextverticalalignment/) | Gets or sets the text vertical alignment of text. |
| [GetWidth()](../chartframe/getwidth/) | Gets or sets the width of frame in units of 1/4000 of the chart area. |
| [GetX()](../chartframe/getx/) | Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [GetY()](../chartframe/gety/) | Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [IsAutomaticRotation()](./isautomaticrotation/) | Indicates whether the text of the chart is automatically rotated. |
| [IsAutomaticSize()](../chartframe/isautomaticsize/) | Indicates whether the chart frame is automatic sized. |
| [IsAutoText()](./isautotext/) | Indicates the text is auto generated. |
| [IsDefaultPosBeSet()](../chartframe/isdefaultposbeset/) | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [IsDeleted()](./isdeleted/) | Indicates whether this data labels is deleted. |
| [IsInnerMode()](../chartframe/isinnermode/) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsResizeShapeToFitText()](./isresizeshapetofittext/) | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside. |
| [IsTextWrapped()](./istextwrapped/) | Gets or sets a value indicating whether the text is wrapped. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ChartTextFrame\& src)](./operator_asm/) | operator= |
| [operator=(const ChartFrame\& src)](../chartframe/operator_asm/) | operator= |
| [SetAutoScaleFont(bool value)](../chartframe/setautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
| [SetBackgroundMode(BackgroundMode value)](../chartframe/setbackgroundmode/) | Gets and sets the display mode of the background. |
| [SetDirectionType(ChartTextDirectionType value)](./setdirectiontype/) | Gets and sets the direction of text. |
| [SetHeight(int32_t value)](../chartframe/setheight/) | Gets or sets the height of frame in units of 1/4000 of the chart area. |
| [SetIsAutomaticSize(bool value)](../chartframe/setisautomaticsize/) | Indicates whether the chart frame is automatic sized. |
| [SetIsAutoText(bool value)](./setisautotext/) | Indicates the text is auto generated. |
| [SetIsDeleted(bool value)](./setisdeleted/) | Indicates whether this data labels is deleted. |
| [SetIsInnerMode(bool value)](../chartframe/setisinnermode/) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [SetIsResizeShapeToFitText(bool value)](./setisresizeshapetofittext/) | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside. |
| [SetIsTextWrapped(bool value)](./setistextwrapped/) | Gets or sets a value indicating whether the text is wrapped. |
| [SetLinkedSource(const U16String\& value)](./setlinkedsource/) | Gets and sets a reference to the worksheet. |
| [SetLinkedSource(const char16_t* value)](./setlinkedsource/) | Gets and sets a reference to the worksheet. |
| [SetPositionAuto()](../chartframe/setpositionauto/) | Set position of the frame to automatic. |
| [SetReadingOrder(TextDirectionType value)](./setreadingorder/) | Represents text reading order. |
| [SetRotationAngle(int32_t value)](./setrotationangle/) | Represents text rotation angle. |
| [SetShadow(bool value)](../chartframe/setshadow/) | True if the frame has a shadow. |
| [SetText(const U16String\& value)](./settext/) | Gets or sets the text of a frame's title. |
| [SetText(const char16_t* value)](./settext/) | Gets or sets the text of a frame's title. |
| [SetTextHorizontalAlignment(TextAlignmentType value)](./settexthorizontalalignment/) | Gets and sets the text horizontal alignment. |
| [SetTextVerticalAlignment(TextAlignmentType value)](./settextverticalalignment/) | Gets or sets the text vertical alignment of text. |
| [SetWidth(int32_t value)](../chartframe/setwidth/) | Gets or sets the width of frame in units of 1/4000 of the chart area. |
| [SetX(int32_t value)](../chartframe/setx/) | Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [SetY(int32_t value)](../chartframe/sety/) | Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [~ChartFrame()](../chartframe/~chartframe/) | Destructor. |
| [~ChartTextFrame()](./~charttextframe/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Class [ChartFrame](../chartframe/)
* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
