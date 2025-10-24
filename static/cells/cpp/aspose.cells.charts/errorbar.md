##Aspose::Cells::Charts::ErrorBar class
'Aspose::Cells::Charts::ErrorBar class. Represents error bar of data series in C++.'
## ErrorBar class
Represents error bar of data series.
```cpp
class ErrorBar : public Aspose::Cells::Drawing::Line
```
## Methods
| Method | Description |
| --- | --- |
| [ErrorBar(ErrorBar_Impl* impl)](./errorbar/) | Constructs from an implementation object. |
| [ErrorBar(const ErrorBar\& src)](./errorbar/) | Copy constructor. |
| [ErrorBar(const Line\& src)](./errorbar/) | Constructs from a parent object. |
| [GetAmount()](./getamount/) | Represents amount of error bar. |
| [GetBeginArrowLength()](../../aspose.cells.drawing/line/getbeginarrowlength/) | Specifies the length of the arrowhead for the begin of a line. |
| [GetBeginArrowWidth()](../../aspose.cells.drawing/line/getbeginarrowwidth/) | Specifies the width of the arrowhead for the begin of a line. |
| [GetBeginType()](../../aspose.cells.drawing/line/getbegintype/) | Specifies an arrowhead for the begin of a line. |
| [GetCapType()](../../aspose.cells.drawing/line/getcaptype/) | Specifies the ending caps. |
| [GetColor()](../../aspose.cells.drawing/line/getcolor/) | Represents the [Color](../../aspose.cells/color/) of the line. |
| [GetCompoundType()](../../aspose.cells.drawing/line/getcompoundtype/) | Specifies the compound line type. |
| [GetDashType()](../../aspose.cells.drawing/line/getdashtype/) | Specifies the dash line type. |
| [GetDisplayType()](./getdisplaytype/) | Represents the display type of error bar. |
| [GetEndArrowLength()](../../aspose.cells.drawing/line/getendarrowlength/) | Specifies the length of the arrowhead for the end of a line. |
| [GetEndArrowWidth()](../../aspose.cells.drawing/line/getendarrowwidth/) | Specifies the width of the arrowhead for the end of a line. |
| [GetEndType()](../../aspose.cells.drawing/line/getendtype/) | Specifies an arrowhead for the end of a line. |
| [GetFormattingType()](../../aspose.cells.drawing/line/getformattingtype/) | Gets or sets format type. |
| [GetGradientFill()](../../aspose.cells.drawing/line/getgradientfill/) | Represents gradient fill. |
| [GetJoinType()](../../aspose.cells.drawing/line/getjointype/) | Specifies the joining caps. |
| [GetMinusValue()](./getminusvalue/) | Represents negative error amount when error bar type is Custom. |
| [GetPlusValue()](./getplusvalue/) | Represents positive error amount when error bar type is Custom. |
| [GetShowMarkerTTop()](./getshowmarkerttop/) | Indicates if formatting error bars with a T-top. |
| [GetStyle()](../../aspose.cells.drawing/line/getstyle/) | Represents the style of the line. |
| [GetThemeColor()](../../aspose.cells.drawing/line/getthemecolor/) | Gets and sets the theme color. |
| [GetTransparency()](../../aspose.cells.drawing/line/gettransparency/) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [GetType()](./gettype/) | Represents error bar amount type. |
| [GetWeight()](../../aspose.cells.drawing/line/getweight/) | Gets or sets the [WeightType](../../aspose.cells.drawing/weighttype/) of the line. |
| [GetWeightPt()](../../aspose.cells.drawing/line/getweightpt/) | Gets or sets the weight of the line in unit of points. |
| [GetWeightPx()](../../aspose.cells.drawing/line/getweightpx/) | Gets or sets the weight of the line in unit of pixels. |
| [IsAuto()](../../aspose.cells.drawing/line/isauto/) | Indicates whether this line style is auto assigned. |
| [IsAutomaticColor()](../../aspose.cells.drawing/line/isautomaticcolor/) | Indicates whether the color of line is automatic assigned. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsVisible()](../../aspose.cells.drawing/line/isvisible/) | Represents whether the line is visible. |
| [Line(Line_Impl* impl)](../../aspose.cells.drawing/line/line/) | Constructs from an implementation object. |
| [Line(const Line\& src)](../../aspose.cells.drawing/line/line/) | Copy constructor. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ErrorBar\& src)](./operator_asm/) | operator= |
| [operator=(const Line\& src)](../../aspose.cells.drawing/line/operator_asm/) | operator= |
| [SetAmount(double value)](./setamount/) | Represents amount of error bar. |
| [SetBeginArrowLength(MsoArrowheadLength value)](../../aspose.cells.drawing/line/setbeginarrowlength/) | Specifies the length of the arrowhead for the begin of a line. |
| [SetBeginArrowWidth(MsoArrowheadWidth value)](../../aspose.cells.drawing/line/setbeginarrowwidth/) | Specifies the width of the arrowhead for the begin of a line. |
| [SetBeginType(MsoArrowheadStyle value)](../../aspose.cells.drawing/line/setbegintype/) | Specifies an arrowhead for the begin of a line. |
| [SetCapType(LineCapType value)](../../aspose.cells.drawing/line/setcaptype/) | Specifies the ending caps. |
| [SetColor(const Aspose::Cells::Color\& value)](../../aspose.cells.drawing/line/setcolor/) | Represents the [Color](../../aspose.cells/color/) of the line. |
| [SetCompoundType(MsoLineStyle value)](../../aspose.cells.drawing/line/setcompoundtype/) | Specifies the compound line type. |
| [SetDashType(MsoLineDashStyle value)](../../aspose.cells.drawing/line/setdashtype/) | Specifies the dash line type. |
| [SetDisplayType(ErrorBarDisplayType value)](./setdisplaytype/) | Represents the display type of error bar. |
| [SetEndArrowLength(MsoArrowheadLength value)](../../aspose.cells.drawing/line/setendarrowlength/) | Specifies the length of the arrowhead for the end of a line. |
| [SetEndArrowWidth(MsoArrowheadWidth value)](../../aspose.cells.drawing/line/setendarrowwidth/) | Specifies the width of the arrowhead for the end of a line. |
| [SetEndType(MsoArrowheadStyle value)](../../aspose.cells.drawing/line/setendtype/) | Specifies an arrowhead for the end of a line. |
| [SetFormattingType(ChartLineFormattingType value)](../../aspose.cells.drawing/line/setformattingtype/) | Gets or sets format type. |
| [SetIsAuto(bool value)](../../aspose.cells.drawing/line/setisauto/) | Indicates whether this line style is auto assigned. |
| [SetIsVisible(bool value)](../../aspose.cells.drawing/line/setisvisible/) | Represents whether the line is visible. |
| [SetJoinType(LineJoinType value)](../../aspose.cells.drawing/line/setjointype/) | Specifies the joining caps. |
| [SetMinusValue(const U16String\& value)](./setminusvalue/) | Represents negative error amount when error bar type is Custom. |
| [SetMinusValue(const char16_t* value)](./setminusvalue/) | Represents negative error amount when error bar type is Custom. |
| [SetPlusValue(const U16String\& value)](./setplusvalue/) | Represents positive error amount when error bar type is Custom. |
| [SetPlusValue(const char16_t* value)](./setplusvalue/) | Represents positive error amount when error bar type is Custom. |
| [SetShowMarkerTTop(bool value)](./setshowmarkerttop/) | Indicates if formatting error bars with a T-top. |
| [SetStyle(LineType value)](../../aspose.cells.drawing/line/setstyle/) | Represents the style of the line. |
| [SetThemeColor(const ThemeColor\& value)](../../aspose.cells.drawing/line/setthemecolor/) | Gets and sets the theme color. |
| [SetTransparency(double value)](../../aspose.cells.drawing/line/settransparency/) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [SetType(ErrorBarType value)](./settype/) | Represents error bar amount type. |
| [SetWeight(WeightType value)](../../aspose.cells.drawing/line/setweight/) | Gets or sets the [WeightType](../../aspose.cells.drawing/weighttype/) of the line. |
| [SetWeightPt(double value)](../../aspose.cells.drawing/line/setweightpt/) | Gets or sets the weight of the line in unit of points. |
| [SetWeightPx(double value)](../../aspose.cells.drawing/line/setweightpx/) | Gets or sets the weight of the line in unit of pixels. |
| [~ErrorBar()](./~errorbar/) | Destructor. |
| [~Line()](../../aspose.cells.drawing/line/~line/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
cells.Get(u"a1").PutValue(2);
cells.Get(u"a2").PutValue(5);
cells.Get(u"a3").PutValue(3);
cells.Get(u"a4").PutValue(6);
cells.Get(u"b1").PutValue(4);
cells.Get(u"b2").PutValue(3);
cells.Get(u"b3").PutValue(6);
cells.Get(u"b4").PutValue(7);
cells.Get(u"C1").PutValue(u"Q1");
cells.Get(u"C2").PutValue(u"Q2");
cells.Get(u"C3").PutValue(u"Y1");
cells.Get(u"C4").PutValue(u"Y2");
int chartIndex = workbook.GetWorksheets().Get(0).GetCharts().Add(ChartType::Column, 11, 0, 27, 10);
Chart chart = workbook.GetWorksheets().Get(0).GetCharts().Get(chartIndex);
chart.GetNSeries().Add(u"A1:B4", true);
chart.GetNSeries().SetCategoryData(u"C1:C4");
for (int i = 0; i < chart.GetNSeries().GetCount(); i++)
{
Series aseries = chart.GetNSeries().Get(i);
aseries.GetYErrorBar().SetDisplayType(ErrorBarDisplayType::Minus);
aseries.GetYErrorBar().SetType(ErrorBarType::FixedValue);
aseries.GetYErrorBar().SetAmount(5);
}
Aspose::Cells::Cleanup();
```
## See Also
* Class [Line](../../aspose.cells.drawing/line/)
* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
