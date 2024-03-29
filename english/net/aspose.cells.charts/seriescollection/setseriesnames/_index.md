---
title: SeriesCollection.SetSeriesNames
second_title: Aspose.Cells for .NET API Reference
description: SeriesCollection method. Sets the name of all the serieses in the chart
type: docs
url: /net/aspose.cells.charts/seriescollection/setseriesnames/
---
## SeriesCollection.SetSeriesNames method

Sets the name of all the serieses in the chart.

```csharp
public void SetSeriesNames(int startIndex, string area, bool isVertical)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | The index of the first series which you want to set the name. |
| area | String | Specifies the area for the series name. |
| isVertical | Boolean | &gt;Specifies whether to plot the series from a range of cell values by row or by column. |

### Remarks

If the start index is larger than the count of the serieses, it will return and do nothing.If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.If set data on contiguous cells, use comma to seperate them.For example, ($C$2,$D$5).

### See Also

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


