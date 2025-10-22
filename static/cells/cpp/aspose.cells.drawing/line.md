##Aspose::Cells::Drawing::Line class
'Aspose::Cells::Drawing::Line class. Encapsulates the object that represents the line format in C++.'
## Line class
Encapsulates the object that represents the line format.
```cpp
class Line
```
## Methods
| Method | Description |
| --- | --- |
| [GetBeginArrowLength()](./getbeginarrowlength/) | Specifies the length of the arrowhead for the begin of a line. |
| [GetBeginArrowWidth()](./getbeginarrowwidth/) | Specifies the width of the arrowhead for the begin of a line. |
| [GetBeginType()](./getbegintype/) | Specifies an arrowhead for the begin of a line. |
| [GetCapType()](./getcaptype/) | Specifies the ending caps. |
| [GetColor()](./getcolor/) | Represents the [Color](../../aspose.cells/color/) of the line. |
| [GetCompoundType()](./getcompoundtype/) | Specifies the compound line type. |
| [GetDashType()](./getdashtype/) | Specifies the dash line type. |
| [GetEndArrowLength()](./getendarrowlength/) | Specifies the length of the arrowhead for the end of a line. |
| [GetEndArrowWidth()](./getendarrowwidth/) | Specifies the width of the arrowhead for the end of a line. |
| [GetEndType()](./getendtype/) | Specifies an arrowhead for the end of a line. |
| [GetFormattingType()](./getformattingtype/) | Gets or sets format type. |
| [GetGradientFill()](./getgradientfill/) | Represents gradient fill. |
| [GetJoinType()](./getjointype/) | Specifies the joining caps. |
| [GetStyle()](./getstyle/) | Represents the style of the line. |
| [GetThemeColor()](./getthemecolor/) | Gets and sets the theme color. |
| [GetTransparency()](./gettransparency/) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [GetWeight()](./getweight/) | Gets or sets the [WeightType](../weighttype/) of the line. |
| [GetWeightPt()](./getweightpt/) | Gets or sets the weight of the line in unit of points. |
| [GetWeightPx()](./getweightpx/) | Gets or sets the weight of the line in unit of pixels. |
| [IsAuto()](./isauto/) | Indicates whether this line style is auto assigned. |
| [IsAutomaticColor()](./isautomaticcolor/) | Indicates whether the color of line is automatic assigned. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsVisible()](./isvisible/) | Represents whether the line is visible. |
| [Line(Line_Impl* impl)](./line/) | Constructs from an implementation object. |
| [Line(const Line\& src)](./line/) | Copy constructor. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Line\& src)](./operator_asm/) | operator= |
| [SetBeginArrowLength(MsoArrowheadLength value)](./setbeginarrowlength/) | Specifies the length of the arrowhead for the begin of a line. |
| [SetBeginArrowWidth(MsoArrowheadWidth value)](./setbeginarrowwidth/) | Specifies the width of the arrowhead for the begin of a line. |
| [SetBeginType(MsoArrowheadStyle value)](./setbegintype/) | Specifies an arrowhead for the begin of a line. |
| [SetCapType(LineCapType value)](./setcaptype/) | Specifies the ending caps. |
| [SetColor(const Aspose::Cells::Color\& value)](./setcolor/) | Represents the [Color](../../aspose.cells/color/) of the line. |
| [SetCompoundType(MsoLineStyle value)](./setcompoundtype/) | Specifies the compound line type. |
| [SetDashType(MsoLineDashStyle value)](./setdashtype/) | Specifies the dash line type. |
| [SetEndArrowLength(MsoArrowheadLength value)](./setendarrowlength/) | Specifies the length of the arrowhead for the end of a line. |
| [SetEndArrowWidth(MsoArrowheadWidth value)](./setendarrowwidth/) | Specifies the width of the arrowhead for the end of a line. |
| [SetEndType(MsoArrowheadStyle value)](./setendtype/) | Specifies an arrowhead for the end of a line. |
| [SetFormattingType(ChartLineFormattingType value)](./setformattingtype/) | Gets or sets format type. |
| [SetIsAuto(bool value)](./setisauto/) | Indicates whether this line style is auto assigned. |
| [SetIsVisible(bool value)](./setisvisible/) | Represents whether the line is visible. |
| [SetJoinType(LineJoinType value)](./setjointype/) | Specifies the joining caps. |
| [SetStyle(LineType value)](./setstyle/) | Represents the style of the line. |
| [SetThemeColor(const ThemeColor\& value)](./setthemecolor/) | Gets and sets the theme color. |
| [SetTransparency(double value)](./settransparency/) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [SetWeight(WeightType value)](./setweight/) | Gets or sets the [WeightType](../weighttype/) of the line. |
| [SetWeightPt(double value)](./setweightpt/) | Gets or sets the weight of the line in unit of points. |
| [SetWeightPx(double value)](./setweightpx/) | Gets or sets the weight of the line in unit of pixels. |
| [~Line()](./~line/) | Destructor. |
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
int chartIndex = sheet.GetCharts().Add(ChartType::Line, 9, 9, 21, 15);
Chart chart = sheet.GetCharts().Get(chartIndex);
//Add series
chart.GetNSeries().Add(u"A2:B4", true);
//Set category data
chart.GetNSeries().SetCategoryData(u"=Sheet1!$A$2:$A$4");
//Applying a dotted line style on the lines of an NSeries
chart.GetNSeries().Get(0).GetBorder().SetStyle(LineType::Dot);
chart.GetNSeries().Get(0).GetBorder().SetColor(Color{ 0xff, 0xff, 0, 0 });
//Applying a triangular marker style on the data markers of an NSeries
chart.GetNSeries().Get(0).GetMarker().SetMarkerStyle(ChartMarkerType::Triangle);
//Setting the weight of all lines in an NSeries to medium
chart.GetNSeries().Get(0).GetBorder().SetWeight(WeightType::MediumLine);
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
