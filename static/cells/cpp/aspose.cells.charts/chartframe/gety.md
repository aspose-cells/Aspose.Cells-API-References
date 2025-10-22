##Aspose::Cells::Charts::ChartFrame::GetY method
'Aspose::Cells::Charts::ChartFrame::GetY method. Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area in C++.'
## ChartFrame::GetY method
Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area.
>Deprecated
>
>Use ChartFrame.YRatioToChart property, instead.
```cpp
int32_t Aspose::Cells::Charts::ChartFrame::GetY()
```
## Remarks
How to convert units of 1/4000 to pixels? Y In Pixels = Y * Chart.ChartObject.Height / 4000d;
NOTE: This member is now obsolete. Please use ChartFrame.YRatioToChart property, instead. Y = YRatioToChart * 4000. This property will be removed 12 months later since February 2025. **Aspose** apologizes for any inconvenience you may have experienced.
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [ChartFrame](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
