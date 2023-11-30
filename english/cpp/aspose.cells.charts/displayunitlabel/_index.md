---
title: Aspose::Cells::Charts::DisplayUnitLabel class
linktitle: DisplayUnitLabel
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::DisplayUnitLabel class. Represents the display unit label in C++.'
type: docs
weight: 1300
url: /cpp/aspose.cells.charts/displayunitlabel/
---
## DisplayUnitLabel class


Represents the display unit label.

```cpp
class DisplayUnitLabel : public Aspose::Cells::Charts::ChartTextFrame
```

## Methods

| Method | Description |
| --- | --- |
| [Characters(int32_t startIndex, int32_t length)](../charttextframe/characters/) | Returns a Characters object that represents a range of characters within the text. |
| [ChartFrame(ChartFrame_Impl* impl)](../chartframe/chartframe/) | Constructs from an implementation object. |
| [ChartFrame(const ChartFrame\& src)](../chartframe/chartframe/) | Copy constructor. |
| [ChartTextFrame(ChartTextFrame_Impl* impl)](../charttextframe/charttextframe/) | Constructs from an implementation object. |
| [ChartTextFrame(const ChartTextFrame\& src)](../charttextframe/charttextframe/) | Copy constructor. |
| [ChartTextFrame(const ChartFrame\& src)](../charttextframe/charttextframe/) | Constructs from a parent object. |
| [DisplayUnitLabel(DisplayUnitLabel_Impl* impl)](./displayunitlabel/) | Constructs from an implementation object. |
| [DisplayUnitLabel(const DisplayUnitLabel\& src)](./displayunitlabel/) | Copy constructor. |
| [DisplayUnitLabel(const ChartTextFrame\& src)](./displayunitlabel/) | Constructs from a parent object. |
| [GetArea()](../chartframe/getarea/) | Gets the [area](../). |
| [GetAutoScaleFont()](./getautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
| [GetBackgroundMode()](../chartframe/getbackgroundmode/) | Gets and sets the display mode of the background. |
| [GetBorder()](../chartframe/getborder/) | Gets the [border](../). |
| [GetDefaultHeight()](../chartframe/getdefaultheight/) | Represents height of default position. |
| [GetDefaultWidth()](../chartframe/getdefaultwidth/) | Represents width of default position. |
| [GetDefaultX()](../chartframe/getdefaultx/) | Represents x of default position. |
| [GetDefaultY()](../chartframe/getdefaulty/) | Represents y of default position. |
| [GetDirectionType()](../charttextframe/getdirectiontype/) | Gets and sets the direction of text. |
| [GetFont()](./getfont/) | Gets a [Font](../../aspose.cells/font/) object of the specified [ChartFrame](../chartframe/) object. |
| [GetHeight()](../chartframe/getheight/) | Gets or sets the height of frame in units of 1/4000 of the chart area. |
| [GetLinkedSource()](../charttextframe/getlinkedsource/) | Gets and sets a reference to the worksheet. |
| [GetReadingOrder()](../charttextframe/getreadingorder/) | Represents text reading order. |
| [GetRotationAngle()](../charttextframe/getrotationangle/) | Represents text rotation angle. |
| [GetShadow()](../chartframe/getshadow/) | True if the frame has a shadow. |
| [GetShapeProperties()](../chartframe/getshapeproperties/) | Gets the ShapeProperties object. |
| [GetText()](./gettext/) | Gets or sets the text of display unit label. |
| [GetTextHorizontalAlignment()](../charttextframe/gettexthorizontalalignment/) | Gets and sets the text horizontal alignment. |
| [GetTextOptions()](../chartframe/gettextoptions/) | Gets and sets the options of the text. |
| [GetTextVerticalAlignment()](../charttextframe/gettextverticalalignment/) | Gets or sets the text vertical alignment of text. |
| [GetWidth()](../chartframe/getwidth/) | Gets or sets the width of frame in units of 1/4000 of the chart area. |
| [GetX()](../chartframe/getx/) | Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [GetY()](../chartframe/gety/) | Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [IsAutomaticRotation()](../charttextframe/isautomaticrotation/) | Indicates whether the text of the chart is automatically rotated. |
| [IsAutomaticSize()](../chartframe/isautomaticsize/) | Indicates whether the chart frame is automatic sized. |
| [IsAutoText()](../charttextframe/isautotext/) | Indicates the text is auto generated. |
| [IsDefaultPosBeSet()](../chartframe/isdefaultposbeset/) | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [IsDeleted()](../charttextframe/isdeleted/) | Indicates whether this data labels is deleted. |
| [IsInnerMode()](../chartframe/isinnermode/) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsResizeShapeToFitText()](../charttextframe/isresizeshapetofittext/) | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside. |
| [IsTextWrapped()](../charttextframe/istextwrapped/) | Gets or sets a value indicating whether the text is wrapped. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const DisplayUnitLabel\& src)](./operator_asm/) | operator= |
| [operator=(const ChartTextFrame\& src)](../charttextframe/operator_asm/) | operator= |
| [operator=(const ChartFrame\& src)](../chartframe/operator_asm/) | operator= |
| [SetAutoScaleFont(bool value)](./setautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
| [SetBackgroundMode(BackgroundMode value)](../chartframe/setbackgroundmode/) | Gets and sets the display mode of the background. |
| [SetDirectionType(ChartTextDirectionType value)](../charttextframe/setdirectiontype/) | Gets and sets the direction of text. |
| [SetHeight(int32_t value)](../chartframe/setheight/) | Gets or sets the height of frame in units of 1/4000 of the chart area. |
| [SetIsAutomaticSize(bool value)](../chartframe/setisautomaticsize/) | Indicates whether the chart frame is automatic sized. |
| [SetIsAutoText(bool value)](../charttextframe/setisautotext/) | Indicates the text is auto generated. |
| [SetIsDeleted(bool value)](../charttextframe/setisdeleted/) | Indicates whether this data labels is deleted. |
| [SetIsInnerMode(bool value)](../chartframe/setisinnermode/) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [SetIsResizeShapeToFitText(bool value)](../charttextframe/setisresizeshapetofittext/) | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside. |
| [SetIsTextWrapped(bool value)](../charttextframe/setistextwrapped/) | Gets or sets a value indicating whether the text is wrapped. |
| [SetLinkedSource(const U16String\& value)](../charttextframe/setlinkedsource/) | Gets and sets a reference to the worksheet. |
| [SetLinkedSource(const char16_t* value)](../charttextframe/setlinkedsource/) | Gets and sets a reference to the worksheet. |
| [SetPositionAuto()](../chartframe/setpositionauto/) | Set position of the frame to automatic. |
| [SetReadingOrder(TextDirectionType value)](../charttextframe/setreadingorder/) | Represents text reading order. |
| [SetRotationAngle(int32_t value)](../charttextframe/setrotationangle/) | Represents text rotation angle. |
| [SetShadow(bool value)](../chartframe/setshadow/) | True if the frame has a shadow. |
| [SetText(const U16String\& value)](./settext/) | Gets or sets the text of display unit label. |
| [SetText(const char16_t* value)](./settext/) | Gets or sets the text of display unit label. |
| [SetTextHorizontalAlignment(TextAlignmentType value)](../charttextframe/settexthorizontalalignment/) | Gets and sets the text horizontal alignment. |
| [SetTextVerticalAlignment(TextAlignmentType value)](../charttextframe/settextverticalalignment/) | Gets or sets the text vertical alignment of text. |
| [SetWidth(int32_t value)](../chartframe/setwidth/) | Gets or sets the width of frame in units of 1/4000 of the chart area. |
| [SetX(int32_t value)](../chartframe/setx/) | Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [SetY(int32_t value)](../chartframe/sety/) | Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [~ChartFrame()](../chartframe/~chartframe/) | Destructor. |
| [~ChartTextFrame()](../charttextframe/~charttextframe/) | Destructor. |
| [~DisplayUnitLabel()](./~displayunitlabel/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
//Adding a new worksheet to the Excel object
int sheetIndex = workbook.GetWorksheets().Add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//Adding a sample value to "A1" cell
worksheet.GetCells().Get(u"A1").PutValue(50);
//Adding a sample value to "A2" cell
worksheet.GetCells().Get(u"A2").PutValue(100);
//Adding a sample value to "A3" cell
worksheet.GetCells().Get(u"A3").PutValue(150);
//Adding a sample value to "A4" cell
worksheet.GetCells().Get(u"A4").PutValue(200);
//Adding a sample value to "B1" cell
worksheet.GetCells().Get(u"B1").PutValue(60);
//Adding a sample value to "B2" cell
worksheet.GetCells().Get(u"B2").PutValue(32);
//Adding a sample value to "B3" cell
worksheet.GetCells().Get(u"B3").PutValue(50);
//Adding a sample value to "B4" cell
worksheet.GetCells().Get(u"B4").PutValue(40);
//Adding a sample value to "C1" cell as category data
worksheet.GetCells().Get(u"C1").PutValue(u"Q1");
//Adding a sample value to "C2" cell as category data
worksheet.GetCells().Get(u"C2").PutValue(u"Q2");
//Adding a sample value to "C3" cell as category data
worksheet.GetCells().Get(u"C3").PutValue(u"Y1");
//Adding a sample value to "C4" cell as category data
worksheet.GetCells().Get(u"C4").PutValue(u"Y2");
//Adding a chart to the worksheet
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.GetNSeries().Add(u"A1:B4", true);
//Setting the data source for the category data of NSeries
chart.GetNSeries().SetCategoryData(u"C1:C4");
//Setting the display unit of value(Y) axis.
chart.GetValueAxis().SetDisplayUnit(DisplayUnitType::Hundreds);
DisplayUnitLabel displayUnitLabel = chart.GetValueAxis().GetDisplayUnitLabel();
//Setting the custom display unit label
displayUnitLabel.SetText(u"100");
//Saving the Excel file
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Class [ChartTextFrame](../charttextframe/)
* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
