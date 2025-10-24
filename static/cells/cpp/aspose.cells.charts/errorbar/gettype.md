##Aspose::Cells::Charts::ErrorBar::GetType method
'Aspose::Cells::Charts::ErrorBar::GetType method. Represents error bar amount type in C++.'
## ErrorBar::GetType method
Represents error bar amount type.
```cpp
ErrorBarType Aspose::Cells::Charts::ErrorBar::GetType()
```
## Examples
```cpp
Aspose::Cells::Startup();
Workbook wb(u"chart.xlsx");
Chart chart = wb.GetWorksheets().Get(0).GetCharts().Get(0);
Series aseries = chart.GetNSeries().Get(0);
//Sets custom error bar type
ErrorBarType ty = aseries.GetYErrorBar().GetType();
Aspose::Cells::Cleanup();
```
## See Also
* Enum [ErrorBarType](../../errorbartype/)
* Class [ErrorBar](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
