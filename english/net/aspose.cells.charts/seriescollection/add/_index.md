---
title: SeriesCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: SeriesCollection method. Adds the SeriesCollection collection to a chart
type: docs
url: /net/aspose.cells.charts/seriescollection/add/
---
## Add(string, bool) {#add}

Adds the [`SeriesCollection`](../) collection to a chart.

```csharp
public int Add(string area, bool isVertical)
```

| Parameter | Type | Description |
| --- | --- | --- |
| area | String | Specifies values from which to plot the data series |
| isVertical | Boolean | Specifies whether to plot the series from a range of cell values by row or by column. |

### Return Value

Return the first index of the added ASeries in the NSeries.

### Remarks

If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.If set data on non contiguous cells, use comma to seperate them.For example: ($C$2,$D$5).

### See Also

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool, bool) {#add_1}

Adds the [`SeriesCollection`](../) collection to a chart.

```csharp
public int Add(string area, bool isVertical, bool checkLabels)
```

| Parameter | Type | Description |
| --- | --- | --- |
| area | String | Specifies values from which to plot the data series |
| isVertical | Boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| checkLabels | Boolean | Indicates whether the range contains series's name |

### Return Value

Return the first index of the added ASeries in the NSeries.

### Remarks

If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.If set data on non contiguous cells, use comma to seperate them.For example, ($C$2,$D$5).

### See Also

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


