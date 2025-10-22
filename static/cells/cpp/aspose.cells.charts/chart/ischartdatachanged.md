##Aspose::Cells::Charts::Chart::IsChartDataChanged method
'Aspose::Cells::Charts::Chart::IsChartDataChanged method. Detects if a chart''s data source has changed in C++.'
## Chart::IsChartDataChanged method
Detects if a chart's data source has changed.
```cpp
bool Aspose::Cells::Charts::Chart::IsChartDataChanged()
```
## ReturnValue
Returns true if the chart has changed otherwise returns false
## Remarks
The method detects the changes in the chart's data source before rendering the chart to image format. At first Chart.toImage call, the chart source data (e.g. XValuesParseData, ValuesParseData) will be recorded. Before calling the Chart.toImage method again, call IsChartDataChanged method to check if [Chart](../) needs re-rendering.
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [Chart](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
