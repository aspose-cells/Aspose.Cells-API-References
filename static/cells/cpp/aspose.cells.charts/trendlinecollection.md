##Aspose::Cells::Charts::TrendlineCollection class
'Aspose::Cells::Charts::TrendlineCollection class. Represents a collection of all the Trendline objects for the specified data series in C++.'
## TrendlineCollection class
Represents a collection of all the [Trendline](../trendline/) objects for the specified data series.
```cpp
class TrendlineCollection
```
## Methods
| Method | Description |
| --- | --- |
| [Add(TrendlineType type)](./add/) | Adds a [Trendline](../trendline/) object to this collection with specified type. |
| [Add(TrendlineType type, const U16String\& name)](./add/) | Adds a [Trendline](../trendline/) object to this collection with specified type and name. |
| [Add(TrendlineType type, const char16_t* name)](./add/) | Adds a [Trendline](../trendline/) object to this collection with specified type and name. |
| [Get(int32_t index)](./get/) | Gets a [Trendline](../trendline/) object by its index. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const TrendlineCollection\& src)](./operator_asm/) | operator= |
| [TrendlineCollection(TrendlineCollection_Impl* impl)](./trendlinecollection/) | Constructs from an implementation object. |
| [TrendlineCollection(const TrendlineCollection\& src)](./trendlinecollection/) | Copy constructor. |
| [~TrendlineCollection()](./~trendlinecollection/) | Destructor. |
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
worksheet.GetCells().Get(u"A1").PutValue(50);
worksheet.GetCells().Get(u"A2").PutValue(100);
worksheet.GetCells().Get(u"A3").PutValue(150);
worksheet.GetCells().Get(u"A4").PutValue(200);
worksheet.GetCells().Get(u"B1").PutValue(60);
worksheet.GetCells().Get(u"B2").PutValue(32);
worksheet.GetCells().Get(u"B3").PutValue(50);
worksheet.GetCells().Get(u"B4").PutValue(40);
//Adding a chart to the worksheet
int chartIndex = workbook.GetWorksheets().Get(0).GetCharts().Add(ChartType::Column, 3, 3, 15, 10);
Chart chart = workbook.GetWorksheets().Get(0).GetCharts().Get(chartIndex);
chart.GetNSeries().Add(u"A1:a3", true);
chart.GetNSeries().Get(0).GetTrendLines().Add(TrendlineType::Linear, u"MyTrendLine");
Trendline line = chart.GetNSeries().Get(0).GetTrendLines().Get(0);
line.SetDisplayEquation(true);
line.SetDisplayRSquared(true);
line.SetColor(Color{ 0xff, 0xff, 0, 0 });
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
