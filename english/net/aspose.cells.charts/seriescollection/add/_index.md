---
title: SeriesCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: SeriesCollection method. Adds the Series collection to a chart
type: docs
url: /net/aspose.cells.charts/seriescollection/add/
---
## Add(string, bool) {#add}

Adds the [`Series`](../../series/) collection to a chart.

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

### Examples

```csharp
// Called: chart.NSeries.Add(&amp;quot;=Sheet1!$A$1:$F$11&amp;quot;, true);
public static Workbook Method_Boolean_(Workbook workbook)
        {
            workbook = new Workbook(Constants.sourcePath + &quot;Charts\\Surface\\Surface.xls&quot;);
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[sheet.Charts.Add(ChartType.SurfaceWireframe3D, 5, 2, 25, 11)];
            chart.NSeries.Add(&quot;=Sheet1!$A$1:$F$11&quot;, true);
            return workbook;
        }
```

### See Also

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool, bool) {#add_1}

Adds the [`Series`](../../series/) collection to a chart.

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

### Examples

```csharp
// Called: c.NSeries.Add(&amp;quot;=testname1&amp;quot;, true, false);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            NameCollection nc = wb.Worksheets.Names;
            nc[nc.Add(&quot;testname1&quot;)].RefersTo = &quot;=INDIRECT(\&quot;Sheet1!$A$10:$A$1\&quot;)&quot;;
            nc[nc.Add(&quot;testname2&quot;)].RefersTo = &quot;=INDIRECT(\&quot;Sheet1!$B$10:$B$1\&quot;)&quot;;
            Chart c = wb.Worksheets[0].Charts[wb.Worksheets[0].Charts.Add(ChartType.Column, 0, 0, 10, 10)];
            c.NSeries.Add(&quot;=testname1&quot;, true, false);
            c.NSeries.CategoryData = &quot;=testname2&quot;;
            c.Calculate(); //should be no exception
        }
```

### See Also

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


