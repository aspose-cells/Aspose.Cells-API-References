---
title: Aspose::Cells::Charts::Trendline class
linktitle: Trendline
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Charts::Trendline class. Represents a trendline in a chart in C++.'
type: docs
weight: 3400
url: /de/cpp/aspose.cells.charts/trendline/
---
## Trendline class


Represents a trendline in a chart.

```cpp
class Trendline : public Aspose::Cells::Drawing::Line
```

## Methods

| Method | Description |
| --- | --- |
| [GetBackward()](./getbackward/) | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5. |
| [GetBeginArrowLength()](../../aspose.cells.drawing/line/getbeginarrowlength/) | Specifies the length of the arrowhead for the begin of a line. |
| [GetBeginArrowWidth()](../../aspose.cells.drawing/line/getbeginarrowwidth/) | Specifies the width of the arrowhead for the begin of a line. |
| [GetBeginType()](../../aspose.cells.drawing/line/getbegintype/) | Specifies an arrowhead for the begin of a line. |
| [GetCapType()](../../aspose.cells.drawing/line/getcaptype/) | Specifies the ending caps. |
| [GetColor()](../../aspose.cells.drawing/line/getcolor/) | Represents the [Color](../../aspose.cells/color/) of the line. |
| [GetCompoundType()](../../aspose.cells.drawing/line/getcompoundtype/) | Specifies the compound line type. |
| [GetDashType()](../../aspose.cells.drawing/line/getdashtype/) | Specifies the dash line type. |
| [GetDataLabels()](./getdatalabels/) | Represents the [DataLabels](../datalabels/) object for the specified series. |
| [GetDisplayEquation()](./getdisplayequation/) | Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels. |
| [GetDisplayRSquared()](./getdisplayrsquared/) | Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels. |
| [GetEndArrowLength()](../../aspose.cells.drawing/line/getendarrowlength/) | Specifies the length of the arrowhead for the end of a line. |
| [GetEndArrowWidth()](../../aspose.cells.drawing/line/getendarrowwidth/) | Specifies the width of the arrowhead for the end of a line. |
| [GetEndType()](../../aspose.cells.drawing/line/getendtype/) | Specifies an arrowhead for the end of a line. |
| [GetFormattingType()](../../aspose.cells.drawing/line/getformattingtype/) | Gets or sets format type. |
| [GetForward()](./getforward/) | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of periods must be greater than or equal to zero. |
| [GetGradientFill()](../../aspose.cells.drawing/line/getgradientfill/) | Represents gradient fill. |
| [GetIntercept()](./getintercept/) | Returns or sets the point where the trendline crosses the value axis. |
| [GetJoinType()](../../aspose.cells.drawing/line/getjointype/) | Specifies the joining caps. |
| [GetLegendEntry()](./getlegendentry/) | Gets the legend entry according to this trendline. |
| [GetName()](./getname/) | Returns the name of the trendline. |
| [GetOrder()](./getorder/) | Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be between 2 and 6. |
| [GetPeriod()](./getperiod/) | Returns or sets the period for the moving-average trendline. |
| [GetStyle()](../../aspose.cells.drawing/line/getstyle/) | Represents the style of the line. |
| [GetThemeColor()](../../aspose.cells.drawing/line/getthemecolor/) | Gets and sets the theme color. |
| [GetTransparency()](../../aspose.cells.drawing/line/gettransparency/) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [GetType()](./gettype/) | Returns the trendline type. |
| [GetWeight()](../../aspose.cells.drawing/line/getweight/) | Gets or sets the [WeightType](../../aspose.cells.drawing/weighttype/) of the line. |
| [GetWeightPt()](../../aspose.cells.drawing/line/getweightpt/) | Gets or sets the weight of the line in unit of points. |
| [GetWeightPx()](../../aspose.cells.drawing/line/getweightpx/) | Gets or sets the weight of the line in unit of pixels. |
| [IsAuto()](../../aspose.cells.drawing/line/isauto/) | Indicates whether this line style is auto assigned. |
| [IsAutomaticColor()](../../aspose.cells.drawing/line/isautomaticcolor/) | Indicates whether the color of line is automatic assigned. |
| [IsNameAuto()](./isnameauto/) | Returns if Microsoft Excel automatically determines the name of the trendline. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsVisible()](../../aspose.cells.drawing/line/isvisible/) | Represents whether the line is visible. |
| [Line(Line_Impl* impl)](../../aspose.cells.drawing/line/line/) | Constructs from an implementation object. |
| [Line(const Line\& src)](../../aspose.cells.drawing/line/line/) | Copy constructor. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Trendline\& src)](./operator_asm/) | operator= |
| [operator=(const Line\& src)](../../aspose.cells.drawing/line/operator_asm/) | operator= |
| [SetBackward(double value)](./setbackward/) | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward. The number of periods must be greater than or equal to zero. If the chart type is column ,the number of periods must be between 0 and 0.5. |
| [SetBeginArrowLength(MsoArrowheadLength value)](../../aspose.cells.drawing/line/setbeginarrowlength/) | Specifies the length of the arrowhead for the begin of a line. |
| [SetBeginArrowWidth(MsoArrowheadWidth value)](../../aspose.cells.drawing/line/setbeginarrowwidth/) | Specifies the width of the arrowhead for the begin of a line. |
| [SetBeginType(MsoArrowheadStyle value)](../../aspose.cells.drawing/line/setbegintype/) | Specifies an arrowhead for the begin of a line. |
| [SetCapType(LineCapType value)](../../aspose.cells.drawing/line/setcaptype/) | Specifies the ending caps. |
| [SetColor(const Aspose::Cells::Color\& value)](../../aspose.cells.drawing/line/setcolor/) | Represents the [Color](../../aspose.cells/color/) of the line. |
| [SetCompoundType(MsoLineStyle value)](../../aspose.cells.drawing/line/setcompoundtype/) | Specifies the compound line type. |
| [SetDashType(MsoLineDashStyle value)](../../aspose.cells.drawing/line/setdashtype/) | Specifies the dash line type. |
| [SetDisplayEquation(bool value)](./setdisplayequation/) | Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels. |
| [SetDisplayRSquared(bool value)](./setdisplayrsquared/) | Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels. |
| [SetEndArrowLength(MsoArrowheadLength value)](../../aspose.cells.drawing/line/setendarrowlength/) | Specifies the length of the arrowhead for the end of a line. |
| [SetEndArrowWidth(MsoArrowheadWidth value)](../../aspose.cells.drawing/line/setendarrowwidth/) | Specifies the width of the arrowhead for the end of a line. |
| [SetEndType(MsoArrowheadStyle value)](../../aspose.cells.drawing/line/setendtype/) | Specifies an arrowhead for the end of a line. |
| [SetFormattingType(ChartLineFormattingType value)](../../aspose.cells.drawing/line/setformattingtype/) | Gets or sets format type. |
| [SetForward(double value)](./setforward/) | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward. The number of periods must be greater than or equal to zero. |
| [SetIntercept(double value)](./setintercept/) | Returns or sets the point where the trendline crosses the value axis. |
| [SetIsAuto(bool value)](../../aspose.cells.drawing/line/setisauto/) | Indicates whether this line style is auto assigned. |
| [SetIsNameAuto(bool value)](./setisnameauto/) | Returns if Microsoft Excel automatically determines the name of the trendline. |
| [SetIsVisible(bool value)](../../aspose.cells.drawing/line/setisvisible/) | Represents whether the line is visible. |
| [SetJoinType(LineJoinType value)](../../aspose.cells.drawing/line/setjointype/) | Specifies the joining caps. |
| [SetName(const U16String\& value)](./setname/) | Returns the name of the trendline. |
| [SetName(const char16_t* value)](./setname/) | Returns the name of the trendline. |
| [SetOrder(int32_t value)](./setorder/) | Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial. The order must be between 2 and 6. |
| [SetPeriod(int32_t value)](./setperiod/) | Returns or sets the period for the moving-average trendline. |
| [SetStyle(LineType value)](../../aspose.cells.drawing/line/setstyle/) | Represents the style of the line. |
| [SetThemeColor(const ThemeColor\& value)](../../aspose.cells.drawing/line/setthemecolor/) | Gets and sets the theme color. |
| [SetTransparency(double value)](../../aspose.cells.drawing/line/settransparency/) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [SetWeight(WeightType value)](../../aspose.cells.drawing/line/setweight/) | Gets or sets the [WeightType](../../aspose.cells.drawing/weighttype/) of the line. |
| [SetWeightPt(double value)](../../aspose.cells.drawing/line/setweightpt/) | Gets or sets the weight of the line in unit of points. |
| [SetWeightPx(double value)](../../aspose.cells.drawing/line/setweightpx/) | Gets or sets the weight of the line in unit of pixels. |
| [Trendline(Trendline_Impl* impl)](./trendline/) | Constructs from an implementation object. |
| [Trendline(const Trendline\& src)](./trendline/) | Copy constructor. |
| [Trendline(const Line\& src)](./trendline/) | Constructs from a parent object. |
| [~Line()](../../aspose.cells.drawing/line/~line/) | Destructor. |
| [~Trendline()](./~trendline/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Instanziieren eines Workbook-Objekts
Workbook workbook;
//Hinzufügen eines neuen Arbeitsblatts zum Excel-Objekt
int sheetIndex = workbook.GetWorksheets().Add();
//Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergeben seines Blattindexes
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//Beispielwert zur Zelle "A1" hinzufügen
worksheet.GetCells().Get(u"A1").PutValue(50);
//Beispielwert zur Zelle "A2" hinzufügen
worksheet.GetCells().Get(u"A2").PutValue(100);
//Beispielwert zur Zelle "A3" hinzufügen
worksheet.GetCells().Get(u"A3").PutValue(150);
//Beispielwert zur Zelle "A4" hinzufügen
worksheet.GetCells().Get(u"A4").PutValue(200);
//Beispielwert zur Zelle "B1" hinzufügen
worksheet.GetCells().Get(u"B1").PutValue(60);
//Beispielwert zur Zelle "B2" hinzufügen
worksheet.GetCells().Get(u"B2").PutValue(32);
//Beispielwert zur Zelle "B3" hinzufügen
worksheet.GetCells().Get(u"B3").PutValue(50);
//Beispielwert zur Zelle "B4" hinzufügen
worksheet.GetCells().Get(u"B4").PutValue(40);
//Beispielwert zur Zelle "C1" als Kategoriedaten hinzufügen
worksheet.GetCells().Get(u"C1").PutValue(u"Q1");
//Beispielwert zur Zelle "C2" als Kategoriedaten hinzufügen
worksheet.GetCells().Get(u"C2").PutValue(u"Q2");
//Beispielwert zur Zelle "C3" als Kategoriedaten hinzufügen
worksheet.GetCells().Get(u"C3").PutValue(u"Y1");
//Beispielwert zur Zelle "C4" als Kategoriedaten hinzufügen
worksheet.GetCells().Get(u"C4").PutValue(u"Y2");
//Diagramm zum Arbeitsblatt hinzufügen
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Zugriff auf die Instanz des neu hinzugefügten Diagramms
Chart chart = worksheet.GetCharts().Get(chartIndex);
//NSeries (Diagrammdatenquelle) zum Diagramm hinzufügen, das von Zelle "A1" bis "B4" reicht
chart.GetNSeries().Add(u"A1:B4", true);
//Festlegen der Datenquelle für die Kategoriedaten von NSeries
chart.GetNSeries().SetCategoryData(u"C1:C4");
//eine lineare Trendlinie hinzufügen
int index = chart.GetNSeries().Get(0).GetTrendLines().Add(TrendlineType::Linear);
Trendline trendline = chart.GetNSeries().Get(0).GetTrendLines().Get(index);
//Benutzerdefinierten Namen der Trendlinie festlegen.
trendline.SetName(u"Linear");
//Gleichung im Diagramm anzeigen
trendline.SetDisplayEquation(true);
//R-Quadrat-Wert im Diagramm anzeigen
trendline.SetDisplayRSquared(true);
//Speichern der Excel-Datei
workbook.Save(u"book1.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Class [Line](../../aspose.cells.drawing/line/)
* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
