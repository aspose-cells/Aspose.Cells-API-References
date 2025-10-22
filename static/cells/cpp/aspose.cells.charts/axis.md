##Aspose::Cells::Charts::Axis class
'Aspose::Cells::Charts::Axis class. Encapsulates the object that represents an axis of chart in C++.'
## Axis class
Encapsulates the object that represents an axis of chart.
```cpp
class Axis
```
## Methods
| Method | Description |
| --- | --- |
| [Axis(Axis_Impl* impl)](./axis/) | Constructs from an implementation object. |
| [Axis(const Axis\& src)](./axis/) | Copy constructor. |
| [GetArea()](./getarea/) | Gets the Area. |
| [GetAxisBetweenCategories()](./getaxisbetweencategories/) | Represents if the value axis crosses the category axis between categories. |
| [GetAxisLine()](./getaxisline/) | Gets the appearance of an [Axis](./). |
| [GetAxisTexts()](./getaxistexts/) | Gets the labels of the axis after call [Chart.Calculate()](../chart/calculate/) method. |
| [GetBaseUnitScale()](./getbaseunitscale/) | Represents the base unit scale for the category axis. |
| [GetBins()](./getbins/) | Represents bins on a chart(Histogram/Pareto) axis. |
| [GetCategoryType()](./getcategorytype/) | Represents the category axis type. |
| [GetCrossAt()](./getcrossat/) | Represents the point on the value axis where the category axis crosses it. |
| [GetCrossType()](./getcrosstype/) | Represents the [CrossType](../crosstype/) on the specified axis where the other axis crosses. |
| [GetCustomDisplayUnit()](./getcustomdisplayunit/) | Specifies a custom value for the display unit. |
| [GetCustomUnit()](./getcustomunit/) |  **(Deprecated)** Specifies a custom value for the display unit. |
| [GetDisplayUnit()](./getdisplayunit/) | Represents the unit label for the specified axis. |
| [GetDisplayUnitLabel()](./getdisplayunitlabel/) | Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values— for example, in the millions or billions. |
| [GetHasMultiLevelLabels()](./gethasmultilevellabels/) | Indicates whether the labels shall be shown as multi level. |
| [GetLogBase()](./getlogbase/) | Represents the logarithmic base. Default value is 10.Only applies for Excel2007. |
| [GetMajorGridLines()](./getmajorgridlines/) | Represents major gridlines on a chart axis. |
| [GetMajorTickMark()](./getmajortickmark/) | Represents the type of major tick mark for the specified axis. |
| [GetMajorUnit()](./getmajorunit/) | Represents the major units for the axis. |
| [GetMajorUnitScale()](./getmajorunitscale/) | Represents the major unit scale for the category axis. |
| [GetMaxValue()](./getmaxvalue/) | Represents the maximum value on the value axis. |
| [GetMinorGridLines()](./getminorgridlines/) | Represents minor gridlines on a chart axis. |
| [GetMinorTickMark()](./getminortickmark/) | Represents the type of minor tick mark for the specified axis. |
| [GetMinorUnit()](./getminorunit/) | Represents the minor units for the axis. |
| [GetMinorUnitScale()](./getminorunitscale/) | Represents the major unit scale for the category axis. |
| [GetMinValue()](./getminvalue/) | Represents the minimum value on the value axis. |
| [GetTickLabelPosition()](./getticklabelposition/) | Represents the position of tick-mark labels on the specified axis. |
| [GetTickLabels()](./getticklabels/) | Returns a [TickLabels](../ticklabels/) object that represents the tick-mark labels for the specified axis. |
| [GetTickLabelSpacing()](./getticklabelspacing/) | Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. |
| [GetTickMarkSpacing()](./gettickmarkspacing/) | Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. |
| [GetTitle()](./gettitle/) | Gets the axis' title. |
| [IsAutomaticMajorUnit()](./isautomaticmajorunit/) | Indicates whether the major unit of the axis is automatically assigned. |
| [IsAutomaticMaxValue()](./isautomaticmaxvalue/) | Indicates whether the max value is automatically assigned. |
| [IsAutomaticMinorUnit()](./isautomaticminorunit/) | Indicates whether the minor unit of the axis is automatically assigned. |
| [IsAutomaticMinValue()](./isautomaticminvalue/) | Indicates whether the min value is automatically assigned. |
| [IsAutoTickLabelSpacing()](./isautoticklabelspacing/) | Indicates whether the spacing of tick label is automatic. |
| [IsDisplayUnitLabelShown()](./isdisplayunitlabelshown/) | Represents if the display unit label is shown on the specified axis. |
| [IsLogarithmic()](./islogarithmic/) | Represents if the value axis scale type is logarithmic or not. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsPlotOrderReversed()](./isplotorderreversed/) | Represents if Microsoft Excel plots data points from last to first. |
| [IsVisible()](./isvisible/) | Represents if the axis is visible. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Axis\& src)](./operator_asm/) | operator= |
| [SetAxisBetweenCategories(bool value)](./setaxisbetweencategories/) | Represents if the value axis crosses the category axis between categories. |
| [SetBaseUnitScale(TimeUnit value)](./setbaseunitscale/) | Represents the base unit scale for the category axis. |
| [SetCategoryType(CategoryType value)](./setcategorytype/) | Represents the category axis type. |
| [SetCrossAt(double value)](./setcrossat/) | Represents the point on the value axis where the category axis crosses it. |
| [SetCrossType(CrossType value)](./setcrosstype/) | Represents the [CrossType](../crosstype/) on the specified axis where the other axis crosses. |
| [SetCustomDisplayUnit(double value)](./setcustomdisplayunit/) | Specifies a custom value for the display unit. |
| [SetCustomUnit(int32_t value)](./setcustomunit/) |  **(Deprecated)** Specifies a custom value for the display unit. |
| [SetDisplayUnit(DisplayUnitType value)](./setdisplayunit/) | Represents the unit label for the specified axis. |
| [SetHasMultiLevelLabels(bool value)](./sethasmultilevellabels/) | Indicates whether the labels shall be shown as multi level. |
| [SetIsAutomaticMajorUnit(bool value)](./setisautomaticmajorunit/) | Indicates whether the major unit of the axis is automatically assigned. |
| [SetIsAutomaticMaxValue(bool value)](./setisautomaticmaxvalue/) | Indicates whether the max value is automatically assigned. |
| [SetIsAutomaticMinorUnit(bool value)](./setisautomaticminorunit/) | Indicates whether the minor unit of the axis is automatically assigned. |
| [SetIsAutomaticMinValue(bool value)](./setisautomaticminvalue/) | Indicates whether the min value is automatically assigned. |
| [SetIsAutoTickLabelSpacing(bool value)](./setisautoticklabelspacing/) | Indicates whether the spacing of tick label is automatic. |
| [SetIsDisplayUnitLabelShown(bool value)](./setisdisplayunitlabelshown/) | Represents if the display unit label is shown on the specified axis. |
| [SetIsLogarithmic(bool value)](./setislogarithmic/) | Represents if the value axis scale type is logarithmic or not. |
| [SetIsPlotOrderReversed(bool value)](./setisplotorderreversed/) | Represents if Microsoft Excel plots data points from last to first. |
| [SetIsVisible(bool value)](./setisvisible/) | Represents if the axis is visible. |
| [SetLogBase(double value)](./setlogbase/) | Represents the logarithmic base. Default value is 10.Only applies for Excel2007. |
| [SetMajorTickMark(TickMarkType value)](./setmajortickmark/) | Represents the type of major tick mark for the specified axis. |
| [SetMajorUnit(double value)](./setmajorunit/) | Represents the major units for the axis. |
| [SetMajorUnitScale(TimeUnit value)](./setmajorunitscale/) | Represents the major unit scale for the category axis. |
| [SetMaxValue(const Aspose::Cells::Object\& value)](./setmaxvalue/) | Represents the maximum value on the value axis. |
| [SetMinorTickMark(TickMarkType value)](./setminortickmark/) | Represents the type of minor tick mark for the specified axis. |
| [SetMinorUnit(double value)](./setminorunit/) | Represents the minor units for the axis. |
| [SetMinorUnitScale(TimeUnit value)](./setminorunitscale/) | Represents the major unit scale for the category axis. |
| [SetMinValue(const Aspose::Cells::Object\& value)](./setminvalue/) | Represents the minimum value on the value axis. |
| [SetTickLabelPosition(TickLabelPositionType value)](./setticklabelposition/) | Represents the position of tick-mark labels on the specified axis. |
| [SetTickLabelSpacing(int32_t value)](./setticklabelspacing/) | Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. |
| [SetTickMarkSpacing(int32_t value)](./settickmarkspacing/) | Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. |
| [~Axis()](./~axis/) | Destructor. |
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
//Adding a sample value to "B1" cell
worksheet.GetCells().Get(u"B1").PutValue(4);
//Adding a sample value to "B2" cell
worksheet.GetCells().Get(u"B2").PutValue(20);
//Adding a sample value to "B3" cell
worksheet.GetCells().Get(u"B3").PutValue(50);
//Adding a chart to the worksheet
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 25, 5);
//Accessing the instance of the newly added chart
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.GetNSeries().Add(u"A1:B3", true);
//Set the major unit
chart.GetValueAxis().SetMajorUnit(25);
//Category(X) axis crosses at the maxinum value.
chart.GetValueAxis().SetCrossType(CrossType::Maximum);
//Set he number of categories or series between tick-mark labels.
chart.GetCategoryAxis().SetTickLabelSpacing(2);
//Saving the Excel file
workbook.Save(u"book1.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
