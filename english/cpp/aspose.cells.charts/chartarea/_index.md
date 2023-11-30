---
title: Aspose::Cells::Charts::ChartArea class
linktitle: ChartArea
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::ChartArea class. Encapsulates the object that represents the chart area in the worksheet in C++.'
type: docs
weight: 400
url: /cpp/aspose.cells.charts/chartarea/
---
## ChartArea class


Encapsulates the object that represents the chart area in the worksheet.

```cpp
class ChartArea : public Aspose::Cells::Charts::ChartFrame
```

## Methods

| Method | Description |
| --- | --- |
| [ChartArea(ChartArea_Impl* impl)](./chartarea/) | Constructs from an implementation object. |
| [ChartArea(const ChartArea\& src)](./chartarea/) | Copy constructor. |
| [ChartArea(const ChartFrame\& src)](./chartarea/) | Constructs from a parent object. |
| [ChartFrame(ChartFrame_Impl* impl)](../chartframe/chartframe/) | Constructs from an implementation object. |
| [ChartFrame(const ChartFrame\& src)](../chartframe/chartframe/) | Copy constructor. |
| [GetArea()](../chartframe/getarea/) | Gets the [area](../). |
| [GetAutoScaleFont()](../chartframe/getautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
| [GetBackgroundMode()](../chartframe/getbackgroundmode/) | Gets and sets the display mode of the background. |
| [GetBorder()](../chartframe/getborder/) | Gets the [border](../). |
| [GetDefaultHeight()](../chartframe/getdefaultheight/) | Represents height of default position. |
| [GetDefaultWidth()](../chartframe/getdefaultwidth/) | Represents width of default position. |
| [GetDefaultX()](../chartframe/getdefaultx/) | Represents x of default position. |
| [GetDefaultY()](../chartframe/getdefaulty/) | Represents y of default position. |
| [GetFont()](./getfont/) | Gets a [Font](../../aspose.cells/font/) object of the specified chartarea object. |
| [GetHeight()](./getheight/) | Gets or sets the vertical offset from its lower right corner row. |
| [GetShadow()](../chartframe/getshadow/) | True if the frame has a shadow. |
| [GetShapeProperties()](../chartframe/getshapeproperties/) | Gets the ShapeProperties object. |
| [GetTextOptions()](../chartframe/gettextoptions/) | Gets and sets the options of the text. |
| [GetWidth()](./getwidth/) | Gets or sets the horizontal offset from its lower right corner column. |
| [GetX()](./getx/) | Gets or gets the horizontal offset from its upper left corner column. |
| [GetY()](./gety/) | Gets or gets the vertical offset from its upper left corner row. |
| [IsAutomaticSize()](../chartframe/isautomaticsize/) | Indicates whether the chart frame is automatic sized. |
| [IsDefaultPosBeSet()](../chartframe/isdefaultposbeset/) | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [IsInnerMode()](../chartframe/isinnermode/) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ChartArea\& src)](./operator_asm/) | operator= |
| [operator=(const ChartFrame\& src)](../chartframe/operator_asm/) | operator= |
| [SetAutoScaleFont(bool value)](../chartframe/setautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
| [SetBackgroundMode(BackgroundMode value)](../chartframe/setbackgroundmode/) | Gets and sets the display mode of the background. |
| [SetHeight(int32_t value)](./setheight/) | Gets or sets the vertical offset from its lower right corner row. |
| [SetIsAutomaticSize(bool value)](../chartframe/setisautomaticsize/) | Indicates whether the chart frame is automatic sized. |
| [SetIsInnerMode(bool value)](../chartframe/setisinnermode/) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [SetPositionAuto()](../chartframe/setpositionauto/) | Set position of the frame to automatic. |
| [SetShadow(bool value)](../chartframe/setshadow/) | True if the frame has a shadow. |
| [SetWidth(int32_t value)](./setwidth/) | Gets or sets the horizontal offset from its lower right corner column. |
| [SetX(int32_t value)](./setx/) | Gets or gets the horizontal offset from its upper left corner column. |
| [SetY(int32_t value)](./sety/) | Gets or gets the vertical offset from its upper left corner row. |
| [~ChartArea()](./~chartarea/) | Destructor. |
| [~ChartFrame()](../chartframe/~chartframe/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;

//Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.GetWorksheets().Get(0);

//Adding a sample value to "A1" cell
worksheet.GetCells().Get(u"A1").PutValue(50);

//Adding a sample value to "A2" cell
worksheet.GetCells().Get(u"A2").PutValue(100);

//Adding a sample value to "A3" cell
worksheet.GetCells().Get(u"A3").PutValue(150);

//Adding a sample value to "B1" cell
worksheet.GetCells().Get(u"B1").PutValue(60);

//Adding a sample value to "B2" cell
worksheet.GetCells().Get(u"B2").PutValue(32);

//Adding a sample value to "B3" cell
worksheet.GetCells().Get(u"B3").PutValue(50);

//Adding a chart to the worksheet
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);

//Accessing the instance of the newly added chart
Chart chart = worksheet.GetCharts().Get(chartIndex);

//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.GetNSeries().Add(u"A1:B3", true);

//Getting Chart Area
ChartArea chartArea = chart.GetChartArea();

//Setting the foreground color of the chart area
chartArea.GetArea().SetForegroundColor(Color{ 0xff, 0xff, 0xff, 0 });

//Setting Chart Area Shadow
chartArea.SetShadow(true);

//Saving the Excel file
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Class [ChartFrame](../chartframe/)
* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
