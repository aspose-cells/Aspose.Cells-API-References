##Aspose::Cells::Drawing::Area::GetInvertIfNegative method
'Aspose::Cells::Drawing::Area::GetInvertIfNegative method. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged in C++.'
## Area::GetInvertIfNegative method
If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.
```cpp
bool Aspose::Cells::Drawing::Area::GetInvertIfNegative()
```
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
//Adding a new worksheet to the Workbook object
int sheetIndex = workbook.GetWorksheets().Add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.GetWorksheets().Get(sheetIndex);
//Adding a sample value to "A1" cell
worksheet.GetCells().Get(u"A1").PutValue(50);
//Adding a sample value to "A2" cell
worksheet.GetCells().Get(u"A2").PutValue(-100);
//Adding a sample value to "A3" cell
worksheet.GetCells().Get(u"A3").PutValue(150);
//Adding a chart to the worksheet
int chartIndex = worksheet.GetCharts().Add(ChartType::Column, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
Chart chart = worksheet.GetCharts().Get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "A3"
chart.GetNSeries().Add(u"A1:A3", true);
bool isNegative = chart.GetNSeries().Get(0).GetArea().GetInvertIfNegative();
Aspose::Cells::Cleanup();
```
## See Also
* Class [Area](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
