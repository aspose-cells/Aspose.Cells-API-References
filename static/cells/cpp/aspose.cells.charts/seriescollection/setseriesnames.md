##Aspose::Cells::Charts::SeriesCollection::SetSeriesNames method
'Aspose::Cells::Charts::SeriesCollection::SetSeriesNames method. Sets the name of all the serieses in the chart in C++.'
## SeriesCollection::SetSeriesNames(int32_t, const U16String\&, bool) method
Sets the name of all the serieses in the chart.
```cpp
void Aspose::Cells::Charts::SeriesCollection::SetSeriesNames(int32_t startIndex, const U16String &area, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int32_t | The index of the first series which you want to set the name. |
| area | const U16String\& | Specifies the area for the series name. |
| isVertical | bool | >Specifies whether to plot the series from a range of cell values by row or by column. |
## Remarks
If the start index is larger than the count of the serieses, it will return and do nothing.
If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.
If set data on contiguous cells, use comma to seperate them.For example, ($C$2,$D$5).
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [SeriesCollection](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
## SeriesCollection::SetSeriesNames(int32_t, const char16_t*, bool) method
Sets the name of all the serieses in the chart.
```cpp
void Aspose::Cells::Charts::SeriesCollection::SetSeriesNames(int32_t startIndex, const char16_t *area, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int32_t | The index of the first series which you want to set the name. |
| area | const char16_t* | Specifies the area for the series name. |
| isVertical | bool | >Specifies whether to plot the series from a range of cell values by row or by column. |
## Remarks
If the start index is larger than the count of the serieses, it will return and do nothing.
If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.
If set data on contiguous cells, use comma to seperate them.For example, ($C$2,$D$5).
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [SeriesCollection](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
