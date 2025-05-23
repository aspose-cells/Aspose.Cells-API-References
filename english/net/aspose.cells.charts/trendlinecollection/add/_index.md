---
title: TrendlineCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: TrendlineCollection method. Adds a Trendline object to this collection with specified type
type: docs
url: /net/aspose.cells.charts/trendlinecollection/add/
---
## Add(TrendlineType) {#add}

Adds a [`Trendline`](../../trendline/) object to this collection with specified type.

```csharp
public int Add(TrendlineType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | TrendlineType | Trendline type. |

### Return Value

[`Trendline`](../../trendline/) object index.

### Examples

```csharp
// Called: chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);
public void TrendlineCollection_Method_Add()
{
    Workbook workbook = new Workbook();
    workbook = TestColumn.CreateChart(workbook);
    Chart chart = workbook.Worksheets[0].Charts[0];
    chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);

    checkTrendlineType_Exponential(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    checkTrendlineType_Exponential(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    checkTrendlineType_Exponential(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
}
```

### See Also

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(TrendlineType, string) {#add_1}

Adds a [`Trendline`](../../trendline/) object to this collection with specified type and name.

```csharp
public int Add(TrendlineType type, string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | TrendlineType | Trendline type. |
| name | String | Trendline name. |

### Return Value

[`Trendline`](../../trendline/) object index.

### Examples

```csharp
// Called: chart.NSeries[1].TrendLines.Add(TrendlineType.Logarithmic, "Logarithmic");
public void TrendlineCollection_Method_Add(Workbook workbook)
        {
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet sheet = workbook.Worksheets[sheetIndex];
            //Set the name of worksheet
            sheet.Name = "Chart";

            //Create chart
            int chartIndex = 0;
            chartIndex = sheet.Charts.Add(ChartType.ScatterConnectedByLinesWithDataMarker, 1, 1, 25, 10);
            Chart chart = sheet.Charts[chartIndex];

            //Set properties of chart
            chart.CategoryAxis.MajorGridLines.IsVisible = false;
            chart.Legend.Position = LegendPositionType.Top;

            //Set properties of chart title
            chart.Title.Text = "Scatter Chart:Particulate Levels in Rainfall";
            chart.Title.Font.Color = Color.Black;
            chart.Title.Font.IsBold = true;
            chart.Title.Font.Size = 12;

            //Set properties of nseries
            chart.NSeries.Add("Data!B2:B10", true);
            chart.NSeries[0].XValues = "Data!A2:A10";

            for (int i = 0; i <= chart.NSeries.Count - 1; i++)
            {
                chart.NSeries[i].Name = "Particulate";
            }

            //Trend Lines
            chart.NSeries.Add("Data!B2:B10", true);
            chart.NSeries[1].XValues = "Data!A2:A10";
            chart.NSeries[1].Type = ChartType.Scatter;
            chart.NSeries[1].TrendLines.Add(TrendlineType.Logarithmic, "Logarithmic");
            chart.NSeries[1].TrendLines[0].Order = 2;
            chart.NSeries[1].TrendLines[0].Style = Aspose.Cells.Drawing.LineType.Solid;
            chart.NSeries[1].TrendLines[0].DisplayRSquared = true;
            chart.NSeries[1].TrendLines[0].DataLabels.Border.IsVisible = true;
            chart.NSeries[1].TrendLines[0].DataLabels.Border.Style = Aspose.Cells.Drawing.LineType.Solid;
            chart.NSeries[1].TrendLines[0].DataLabels.Border.Weight = Aspose.Cells.Drawing.WeightType.SingleLine;
            chart.NSeries[1].TrendLines[0].DataLabels.Border.Color = Color.Black;
            chart.NSeries[1].TrendLines[0].DataLabels.Font.Color = Color.Blue;
            //chart.NSeries[1].DataLabels.ShowCategoryName = true;
            //chart.NSeries[1].DataLabels.ShowSeriesName = true;
            //chart.NSeries[1].DataLabels.ShowValue = true;
            //chart.NSeries[1].DataLabels.Position = LabelPositionType.Left;
            chart.NSeries[1].TrendLines[0].DataLabels.X = -1608;
            chart.NSeries[1].TrendLines[0].DataLabels.Y = -694;

            Cells cells = workbook.Worksheets[0].Cells;
            //Set properties of categoryaxis title
            chart.CategoryAxis.Title.Text = cells["A1"].Value.ToString();
            chart.CategoryAxis.Title.Font.Color = Color.Black;
            chart.CategoryAxis.Title.Font.IsBold = true;
            chart.CategoryAxis.Title.Font.Size = 10;

            //Set properties of valueaxis title
            chart.ValueAxis.Title.Text = cells["B1"].Value.ToString();
            chart.ValueAxis.Title.Font.Color = Color.Black;
            chart.ValueAxis.Title.Font.IsBold = true;
            chart.ValueAxis.Title.Font.Size = 10;
            chart.ValueAxis.Title.RotationAngle = 90;
        }
```

### See Also

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


