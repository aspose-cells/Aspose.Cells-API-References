##Aspose::Cells::Charts::ChartFrame::SetX method
'Aspose::Cells::Charts::ChartFrame::SetX method. Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area in C++.'
## ChartFrame::SetX method
Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area.
>Deprecated
>
>Use ChartFrame.XRatioToChart property, instead.
```cpp
void Aspose::Cells::Charts::ChartFrame::SetX(int32_t value)
```
## Remarks
How to convert units of 1/4000 to pixels? X In Pixels = X * Chart.ChartObject.Width / 4000d;
NOTE: This member is now obsolete. Please use ChartFrame.XRatioToChart property, instead. X = XRatioToChart * 4000. This property will be removed 12 months later since February 2025. **Aspose** apologizes for any inconvenience you may have experienced.
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [ChartFrame](../)
* Namespace [Aspose::Cells::Charts](../../)
* Library [Aspose.Cells for C++](../../../)
