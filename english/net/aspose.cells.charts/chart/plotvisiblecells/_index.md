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
// Called: chart.PlotVisibleCells = false;
[Test]
        public void Property_PlotVisibleCells()
        {
            Console.WriteLine("Property_PlotVisibleCells()");
            Workbook wb = new Workbook();

            wb.Worksheets.Clear();

            Worksheet ws = wb.Worksheets[wb.Worksheets.Add()];

            ws.Name = "Sheet";

            Cells cells = ws.Cells;

            cells[0, 1].PutValue("Person");

            cells[0, 1].GetStyle().Font.IsBold = true;

            cells[1, 1].PutValue("Alice");

            cells[2, 1].PutValue("Bob");

            cells[3, 1].PutValue("Eve");

            cells[4, 1].PutValue("Jenny");

            cells[0, 2].PutValue("Values");

            cells[0, 2].GetStyle().Font.IsBold = true;

            cells[1, 2].PutValue(88.0);

            cells[2, 2].PutValue(34.2);

            cells[3, 2].PutValue(34.5);

            cells[4, 2].PutValue(52.0);

            cells.GroupRows(0, 5, true);

            Chart chart = ws.Charts[ws.Charts.Add(ChartType.Column, 15, 1, 30, 8)];

            chart.Title.Text = "Chart Title";

            chart.Legend.Position = LegendPositionType.Bottom;

            chart.ValueAxis.Title.Text = "Values";

            chart.PlotVisibleCells = false;

            chart.Placement = PlacementType.FreeFloating;

            Series s1 = chart.NSeries[chart.NSeries.Add(String.Format("{0}!{1}", ws.Name, "C1"), true)];

            s1.Values = String.Format("{0}!{1}{2}:{1}{3}", ws.Name, "C", 2, 5);

            s1.Name = ws.Cells["C1"].Value.ToString();

            chart.NSeries.CategoryData = String.Format("{0}!{1}{2}:{1}{3}", ws.Name, "C", 2, 5);

            wb.Save(Constants.destPath + "Test_ChartPlotVisOnlyAttr_2.xlsx");
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


