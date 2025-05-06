---
title: Chart.PlotVisibleCells
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Indicates whether only plot visible cells
type: docs
url: /net/aspose.cells.charts/chart/plotvisiblecells/
---
## Chart.PlotVisibleCells property

Indicates whether only plot visible cells.

```csharp
[Obsolete("Use PlotVisibleCellsOnly property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool PlotVisibleCells { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use PlotVisibleCellsOnly property. This method will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: Assert.IsFalse(wb.Worksheets[0].Charts[0].PlotVisibleCells);
[Test]
        public void Property_PlotVisibleCells()
        {
            Workbook wb = new Workbook();

            wb.Worksheets.Clear();

            Worksheet ws = wb.Worksheets[wb.Worksheets.Add()];

            ws.Name = &quot;Sheet&quot;;

            Cells cells = ws.Cells;

            cells[0, 1].PutValue(&quot;Person&quot;);
            Style style = wb.CreateStyle();
            style.Font.IsBold = true;
            cells[0, 1].SetStyle(style);

            cells[1, 1].PutValue(&quot;Alice&quot;);

            cells[2, 1].PutValue(&quot;Bob&quot;);

            cells[3, 1].PutValue(&quot;Eve&quot;);

            cells[4, 1].PutValue(&quot;Jenny&quot;);

            cells[0, 2].PutValue(&quot;Values&quot;);

            cells[0, 2].SetStyle(style);

            cells[1, 2].PutValue(88.0);

            cells[2, 2].PutValue(34.2);

            cells[3, 2].PutValue(34.5);

            cells[4, 2].PutValue(52.0);

            cells.GroupRows(0, 5, true);

            Chart chart = ws.Charts[ws.Charts.Add(ChartType.Column, 15, 1, 30, 8)];

            chart.Title.Text = &quot;Chart Title&quot;;

            chart.Legend.Position = LegendPositionType.Bottom;

            chart.ValueAxis.Title.Text = &quot;Values&quot;;

            chart.PlotVisibleCells = false;

            chart.Placement = PlacementType.FreeFloating;

            Series s1 = chart.NSeries[chart.NSeries.Add(String.Format(&quot;{0}!{1}&quot;, ws.Name, &quot;C1&quot;), true)];

            s1.Values = String.Format(&quot;{0}!{1}{2}:{1}{3}&quot;, ws.Name, &quot;C&quot;, 2, 5);

            s1.Name = ws.Cells[&quot;C1&quot;].Value.ToString();

            chart.NSeries.CategoryData = String.Format(&quot;{0}!{1}{2}:{1}{3}&quot;, ws.Name, &quot;C&quot;, 2, 5);

            wb.Save(Constants.destPath + &quot;HiddenChartData.xlsx&quot;);
            wb = new Workbook(Constants.destPath + &quot;HiddenChartData.xlsx&quot;);

            Assert.IsFalse(wb.Worksheets[0].Charts[0].PlotVisibleCells);
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


