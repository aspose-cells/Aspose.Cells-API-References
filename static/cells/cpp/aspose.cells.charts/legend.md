##Aspose::Cells::Charts::Legend class
'Aspose::Cells::Charts::Legend class. Encapsulates the object that represents the chart legend in C++.'
## Legend class
Encapsulates the object that represents the chart legend.
```cpp
class Legend : public Aspose::Cells::Charts::ChartTextFrame
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
| [GetDirectionType()](../charttextframe/getdirectiontype/) | Gets and sets the direction of text. |
| [GetFont()](../chartframe/getfont/) | Gets a [Font](../../aspose.cells/font/) object of the specified [ChartFrame](../chartframe/) object. |
| [GetHeight()](../chartframe/getheight/) |  **(Deprecated)** Gets or sets the height of frame in units of 1/4000 of the chart area. |
| [GetHeightPixel()](../chartframe/getheightpixel/) | Gets or sets the height of frame in units of Pixel. |
| [GetHeightRatioToChart()](../chartframe/getheightratiotochart/) | Gets or sets the height of frame in units of ratio of the chart area. |
| [GetLegendEntries()](./getlegendentries/) | Gets a collection of all the [LegendEntry](../legendentry/) objects in the specified chart legend. Setting the legend entries of the surface chart is not supported. So it will return null if the chart type is surface chart type. |
| [GetLegendLabels()](./getlegendlabels/) | Gets the labels of the legend entries after call [Chart.Calculate()](../chart/calculate/) method. |
| [GetLinkedSource()](../charttextframe/getlinkedsource/) | Gets and sets a reference to the worksheet. |
| [GetPosition()](./getposition/) | Gets or sets the legend position type. |
| [GetReadingOrder()](../charttextframe/getreadingorder/) | Represents text reading order. |
| [GetRotationAngle()](../charttextframe/getrotationangle/) | Represents text rotation angle. |
| [GetShadow()](../chartframe/getshadow/) | True if the frame has a shadow. |
| [GetShapeProperties()](../chartframe/getshapeproperties/) | Gets the ShapeProperties object. |
| [GetText()](../charttextframe/gettext/) | Gets or sets the text of a frame's title. |
| [GetTextHorizontalAlignment()](../charttextframe/gettexthorizontalalignment/) | Gets and sets the text horizontal alignment. |
| [GetTextOptions()](../chartframe/gettextoptions/) | Gets and sets the options of the text. |
| [GetTextVerticalAlignment()](../charttextframe/gettextverticalalignment/) | Gets or sets the text vertical alignment of text. |
| [GetWidth()](../chartframe/getwidth/) |  **(Deprecated)** Gets or sets the width of frame in units of 1/4000 of the chart area. |
| [GetWidthPixel()](../chartframe/getwidthpixel/) | Gets or sets the width of frame in units of Pixel. |
| [GetWidthRatioToChart()](../chartframe/getwidthratiotochart/) | Gets or sets the width of frame in units of ratio of the chart area. |
| [GetX()](../chartframe/getx/) |  **(Deprecated)** Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [GetXPixel()](../chartframe/getxpixel/) | Gets or sets the x coordinate of the upper left corner in units of Pixel. |
| [GetXRatioToChart()](../chartframe/getxratiotochart/) | Gets or sets the x coordinate of the upper left corner in units of ratio of the chart area. |
| [GetY()](../chartframe/gety/) |  **(Deprecated)** Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [GetYPixel()](../chartframe/getypixel/) | Gets or sets the y coordinate of the upper left corner in units of Pixel. |
| [GetYRatioToChart()](../chartframe/getyratiotochart/) | Gets or sets the y coordinate of the upper left corner in units of ratio of the chart area. |
| [IsAutomaticRotation()](../charttextframe/isautomaticrotation/) | Indicates whether the text of the chart is automatically rotated. |
| [IsAutomaticSize()](../chartframe/isautomaticsize/) | Indicates whether the chart frame is automatic sized. |
| [IsAutoText()](../charttextframe/isautotext/) | Indicates the text is auto generated. |
| [IsDefaultPosBeSet()](../chartframe/isdefaultposbeset/) | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [IsDeleted()](../charttextframe/isdeleted/) | Indicates whether this data labels is deleted. |
| [IsInnerMode()](../chartframe/isinnermode/) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsOverLay()](./isoverlay/) | Gets or sets whether showing the legend without overlapping the chart. |
| [IsResizeShapeToFitText()](../charttextframe/isresizeshapetofittext/) | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside. |
| [IsTextWrapped()](../charttextframe/istextwrapped/) | Gets or sets a value indicating whether the text is wrapped. |
| [Legend(Legend_Impl* impl)](./legend/) | Constructs from an implementation object. |
| [Legend(const Legend\& src)](./legend/) | Copy constructor. |
| [Legend(const ChartTextFrame\& src)](./legend/) | Constructs from a parent object. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Legend\& src)](./operator_asm/) | operator= |
| [operator=(const ChartTextFrame\& src)](../charttextframe/operator_asm/) | operator= |
| [operator=(const ChartFrame\& src)](../chartframe/operator_asm/) | operator= |
| [SetAutoScaleFont(bool value)](../chartframe/setautoscalefont/) | True if the text in the object changes font size when the object size changes. The default value is True. |
| [SetBackgroundMode(BackgroundMode value)](../chartframe/setbackgroundmode/) | Gets and sets the display mode of the background. |
| [SetDirectionType(ChartTextDirectionType value)](../charttextframe/setdirectiontype/) | Gets and sets the direction of text. |
| [SetHeight(int32_t value)](../chartframe/setheight/) |  **(Deprecated)** Gets or sets the height of frame in units of 1/4000 of the chart area. |
| [SetHeightPixel(int32_t value)](../chartframe/setheightpixel/) | Gets or sets the height of frame in units of Pixel. |
| [SetHeightRatioToChart(double value)](../chartframe/setheightratiotochart/) | Gets or sets the height of frame in units of ratio of the chart area. |
| [SetIsAutomaticSize(bool value)](../chartframe/setisautomaticsize/) | Indicates whether the chart frame is automatic sized. |
| [SetIsAutoText(bool value)](../charttextframe/setisautotext/) | Indicates the text is auto generated. |
| [SetIsDeleted(bool value)](../charttextframe/setisdeleted/) | Indicates whether this data labels is deleted. |
| [SetIsInnerMode(bool value)](../chartframe/setisinnermode/) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels. |
| [SetIsOverLay(bool value)](./setisoverlay/) | Gets or sets whether showing the legend without overlapping the chart. |
| [SetIsResizeShapeToFitText(bool value)](../charttextframe/setisresizeshapetofittext/) | Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside. |
| [SetIsTextWrapped(bool value)](../charttextframe/setistextwrapped/) | Gets or sets a value indicating whether the text is wrapped. |
| [SetLinkedSource(const U16String\& value)](../charttextframe/setlinkedsource/) | Gets and sets a reference to the worksheet. |
| [SetLinkedSource(const char16_t* value)](../charttextframe/setlinkedsource/) | Gets and sets a reference to the worksheet. |
| [SetPosition(LegendPositionType value)](./setposition/) | Gets or sets the legend position type. |
| [SetPositionAuto()](../chartframe/setpositionauto/) | Set position of the frame to automatic. |
| [SetReadingOrder(TextDirectionType value)](../charttextframe/setreadingorder/) | Represents text reading order. |
| [SetRotationAngle(int32_t value)](../charttextframe/setrotationangle/) | Represents text rotation angle. |
| [SetShadow(bool value)](../chartframe/setshadow/) | True if the frame has a shadow. |
| [SetText(const U16String\& value)](../charttextframe/settext/) | Gets or sets the text of a frame's title. |
| [SetText(const char16_t* value)](../charttextframe/settext/) | Gets or sets the text of a frame's title. |
| [SetTextHorizontalAlignment(TextAlignmentType value)](../charttextframe/settexthorizontalalignment/) | Gets and sets the text horizontal alignment. |
| [SetTextVerticalAlignment(TextAlignmentType value)](../charttextframe/settextverticalalignment/) | Gets or sets the text vertical alignment of text. |
| [SetWidth(int32_t value)](../chartframe/setwidth/) |  **(Deprecated)** Gets or sets the width of frame in units of 1/4000 of the chart area. |
| [SetWidthPixel(int32_t value)](../chartframe/setwidthpixel/) | Gets or sets the width of frame in units of Pixel. |
| [SetWidthRatioToChart(double value)](../chartframe/setwidthratiotochart/) | Gets or sets the width of frame in units of ratio of the chart area. |
| [SetX(int32_t value)](../chartframe/setx/) |  **(Deprecated)** Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [SetXPixel(int32_t value)](../chartframe/setxpixel/) | Gets or sets the x coordinate of the upper left corner in units of Pixel. |
| [SetXRatioToChart(double value)](../chartframe/setxratiotochart/) | Gets or sets the x coordinate of the upper left corner in units of ratio of the chart area. |
| [SetY(int32_t value)](../chartframe/sety/) |  **(Deprecated)** Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area. |
| [SetYPixel(int32_t value)](../chartframe/setypixel/) | Gets or sets the y coordinate of the upper left corner in units of Pixel. |
| [SetYRatioToChart(double value)](../chartframe/setyratiotochart/) | Gets or sets the y coordinate of the upper left corner in units of ratio of the chart area. |
| [~ChartFrame()](../chartframe/~chartframe/) | Destructor. |
| [~ChartTextFrame()](../charttextframe/~charttextframe/) | Destructor. |
| [~Legend()](./~legend/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
Worksheet sheet = workbook.GetWorksheets().Get(0);
Cells cells = sheet.GetCells();
cells.Get(0, 1).PutValue(u"Income");
cells.Get(1, 0).PutValue(u"Company A");
cells.Get(2, 0).PutValue(u"Company B");
cells.Get(3, 0).PutValue(u"Company C");
cells.Get(1, 1).PutValue(10000);
cells.Get(2, 1).PutValue(20000);
cells.Get(3, 1).PutValue(30000);
int chartIndex = sheet.GetCharts().Add(ChartType::Column, 9, 9, 21, 15);
Chart chart = sheet.GetCharts().Get(chartIndex);
chart.SetChartDataRange(u"A1:B4", true);
//Set Legend's width and height
Legend legend = chart.GetLegend();
//Legend is at right side of chart by default.
//If the legend is at left or right side of the chart, setting Legend.X property will not take effect.
//If the legend is at top or bottom side of the chart, setting Legend.Y property will not take effect.
legend.SetY(1500);
legend.SetWidth(50);
legend.SetHeight(50);
//Set legend's position
legend.SetPosition(LegendPositionType::Left);
Aspose::Cells::Cleanup();
```
## See Also
* Class [ChartTextFrame](../charttextframe/)
* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
