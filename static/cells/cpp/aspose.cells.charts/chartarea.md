##Aspose::Cells::Charts::ChartArea class
'Aspose::Cells::Charts::ChartArea class. Encapsulates the object that represents the chart area in the worksheet in C++.'
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
| [GetDefaultHeight()](../chartframe/getdefaultheight/) |  **(Deprecated)** Represents height of default position in units of 1/4000 of the chart area. |
| [GetDefaultHeightRatioToChart()](../chartframe/getdefaultheightratiotochart/) | Represents height of default position in units of Fraction of the chart area. |
| [GetDefaultWidth()](../chartframe/getdefaultwidth/) |  **(Deprecated)** Represents width of default position in units of 1/4000 of the chart area. |
| [GetDefaultWidthRatioToChart()](../chartframe/getdefaultwidthratiotochart/) | Represents width of default position in units of Fraction of the chart area. |
| [GetDefaultX()](../chartframe/getdefaultx/) |  **(Deprecated)** Represents x of default position in units of 1/4000 of the chart area. |
| [GetDefaultXRatioToChart()](../chartframe/getdefaultxratiotochart/) | Represents x of default position in units of Fraction of the chart area. |
| [GetDefaultY()](../chartframe/getdefaulty/) |  **(Deprecated)** Represents y of default position in units of 1/4000 of the chart area. |
| [GetDefaultYRatioToChart()](../chartframe/getdefaultyratiotochart/) | Represents y of default position in units of Fraction of the chart area. |
| [GetFont()](./getfont/) | Gets a [Font](../../aspose.cells/font/) object of the specified chartarea object. |
| [GetHeight()](./getheight/) |  **(Deprecated)** Gets or sets the vertical offset from its lower right corner row, in units of 1/4000 of the chart area. |
| [GetHeightPixel()](../chartframe/getheightpixel/) | Gets or sets the height of frame in units of Pixel. |
| [GetHeightRatioToChart()](./getheightratiotochart/) | Gets or sets the vertical offset from its lower right corner row, in units of ratio of the chart area. |
| [GetShadow()](../chartframe/getshadow/) | True if the frame has a shadow. |
| [GetShapeProperties()](../chartframe/getshapeproperties/) | Gets the ShapeProperties object. |
| [GetTextOptions()](../chartframe/gettextoptions/) | Gets and sets the options of the text. |
| [GetWidth()](./getwidth/) |  **(Deprecated)** Gets or sets the horizontal offset from its lower right corner column, in units of 1/4000 of the chart area. |
| [GetWidthPixel()](../chartframe/getwidthpixel/) | Gets or sets the width of frame in units of Pixel. |
| [GetWidthRatioToChart()](./getwidthratiotochart/) | Gets or sets the horizontal offset from its lower right corner column, in units of ratio of the chart area. |
| [GetX()](./getx/) |  **(Deprecated)** Gets or gets the horizontal offset from its upper left corner column, in units of 1/4000 of the chart area. |
| [GetXPixel()](../chartframe/getxpixel/) | Gets or sets the x coordinate of the upper left corner in units of Pixel. |
| [GetXRatioToChart()](./getxratiotochart/) | Gets or gets the horizontal offset from its upper left corner column, in units of ratio of the chart area. |
| [GetY()](./gety/) |  **(Deprecated)** Gets or gets the vertical offset from its upper left corner row, in units of 1/4000 of the chart area. |
| [GetYPixel()](../chartframe/getypixel/) | Gets or sets the y coordinate of the upper left corner in units of Pixel. |
| [GetYRatioToChart()](./getyratiotochart/) | Gets or gets the vertical offset from its upper left corner row, in units of ratio of the chart area. |
| [IsAutomaticSize()](../chartframe/isautomaticsize/) | Indicates whether the chart frame is automatic sized. |
| [IsDefaultPosBeSet()](../chartframe/isdefaultposbeset/) | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [IsInnerMode()](../chartframe/isinnermode/) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ChartArea\& src)](./operator_asm/) | operator= |
| [operator=(const ChartFrame\& src)](../chartframe/operator_asm/) | operator= |
| [SetAutoScaleFont(bool value)](../chartframe/setautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
| [SetBackgroundMode(BackgroundMode value)](../chartframe/setbackgroundmode/) | Gets and sets the display mode of the background. |
| [SetHeight(int32_t value)](./setheight/) |  **(Deprecated)** Gets or sets the vertical offset from its lower right corner row, in units of 1/4000 of the chart area. |
| [SetHeightPixel(int32_t value)](../chartframe/setheightpixel/) | Gets or sets the height of frame in units of Pixel. |
| [SetHeightRatioToChart(double value)](./setheightratiotochart/) | Gets or sets the vertical offset from its lower right corner row, in units of ratio of the chart area. |
| [SetIsAutomaticSize(bool value)](../chartframe/setisautomaticsize/) | Indicates whether the chart frame is automatic sized. |
| [SetIsInnerMode(bool value)](../chartframe/setisinnermode/) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [SetPositionAuto()](../chartframe/setpositionauto/) | Set position of the frame to automatic. |
| [SetShadow(bool value)](../chartframe/setshadow/) | True if the frame has a shadow. |
| [SetWidth(int32_t value)](./setwidth/) |  **(Deprecated)** Gets or sets the horizontal offset from its lower right corner column, in units of 1/4000 of the chart area. |
| [SetWidthPixel(int32_t value)](../chartframe/setwidthpixel/) | Gets or sets the width of frame in units of Pixel. |
| [SetWidthRatioToChart(double value)](./setwidthratiotochart/) | Gets or sets the horizontal offset from its lower right corner column, in units of ratio of the chart area. |
| [SetX(int32_t value)](./setx/) |  **(Deprecated)** Gets or gets the horizontal offset from its upper left corner column, in units of 1/4000 of the chart area. |
| [SetXPixel(int32_t value)](../chartframe/setxpixel/) | Gets or sets the x coordinate of the upper left corner in units of Pixel. |
| [SetXRatioToChart(double value)](./setxratiotochart/) | Gets or gets the horizontal offset from its upper left corner column, in units of ratio of the chart area. |
| [SetY(int32_t value)](./sety/) |  **(Deprecated)** Gets or gets the vertical offset from its upper left corner row, in units of 1/4000 of the chart area. |
| [SetYPixel(int32_t value)](../chartframe/setypixel/) | Gets or sets the y coordinate of the upper left corner in units of Pixel. |
| [SetYRatioToChart(double value)](./setyratiotochart/) | Gets or gets the vertical offset from its upper left corner row, in units of ratio of the chart area. |
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
