---
title: Series.PlotOnSecondAxis
second_title: Aspose.Cells for .NET API Reference
description: Series property. Indicates if this series is plotted on second value axis
type: docs
url: /net/aspose.cells.charts/series/plotonsecondaxis/
---
## Series.PlotOnSecondAxis property

Indicates if this series is plotted on second value axis.

```csharp
public bool PlotOnSecondAxis { get; set; }
```

### Examples

```csharp
// Called: MySerie.PlotOnSecondAxis = false;
[Test]
        public void Property_PlotOnSecondAxis()
        {
            Console.WriteLine(&quot;Property_PlotOnSecondAxis()&quot;);
            string infn = path + &quot;TEST_ChartAxisLogBase.xlsx&quot;;
            string outfn = Constants.destPath + &quot;TEST_ChartAxisLogBase_out.xlsx&quot;;

            Workbook workbook = new Workbook(infn);
            workbook.Save(outfn);

            // test 2
            Workbook AsposeBook = new Workbook();
            int SheetIndex = AsposeBook.Worksheets.Add();
            Worksheet ActualChartSheet = AsposeBook.Worksheets[SheetIndex];
            SheetIndex = AsposeBook.Worksheets.Add();
            Worksheet DataSheet = AsposeBook.Worksheets[SheetIndex];
            DataSheet.IsVisible = false;
            DataSheet.Name = &quot;DataSheet&quot;;


            int ChartIndex = ActualChartSheet.Charts.Add(ChartType.Line, 0, 0, 30, 10);
            Chart ActualChart = ActualChartSheet.Charts[ChartIndex];

            double[] XValues = { 2.4, 0.3, 0.2, 1.1, 2.3, 2.1, 0.3, 0.2, 0.128, 0.4, 0.2, 1.2, 0.7, 0.13, 0.13 };
            double[] Yvalues = { 0.867, -0.00141, 0.113, 0.028, 0.399, -0.18, 0.072, -0.237, 0.420, -0.132, -0.0125, 0.0405, -0.0479, -0.112, -0.1441 };
            double[] ZValues = { 1991446, 1416791, 1266904, 942250, 803036, 731421, 344330, 333208, 261988, 260854, 252742, 193094, 180512, 158543, 145193 };

            ActualChart.Title.Text = &quot;Example Bubble Chart&quot;;
            SeriesCollection AspSeries = ActualChart.NSeries;
            int SerieCount = AspSeries.Add(&quot;DataSheet!A1:A15&quot;, true);
            Series MySerie = AspSeries[SerieCount];
            MySerie.Type = ChartType.Bubble3D;
            MySerie.PlotOnSecondAxis = false;
            MySerie.Name = &quot;Example Bubble Chart&quot;;


            DataSheet.Cells.ImportArray(XValues, 0, 0, true);
            MySerie.XValues = &quot;DataSheet!$A$1:$A$15&quot;;
            DataSheet.Cells.ImportArray(Yvalues, 0, 1, true);
            MySerie.Values = &quot;DataSheet!$B$1:$B$15&quot;;
            DataSheet.Cells.ImportArray(ZValues, 0, 2, true);
            MySerie.BubbleSizes = &quot;DataSheet!$C$1:$C$15&quot;;


            ActualChart.ValueAxis.MinorGridLines.IsVisible = false;
            ActualChart.ValueAxis.MajorGridLines.IsVisible = false;
            ActualChart.ValueAxis.MaxValue = 1.2;
            ActualChart.ValueAxis.MinValue = -0.6;
            ActualChart.ValueAxis.CrossAt = 0.31;
            ActualChart.ValueAxis.TickLabelPosition = TickLabelPositionType.High;


            ActualChart.CategoryAxis.MajorGridLines.IsVisible = false;
            ActualChart.CategoryAxis.MajorGridLines.IsVisible = false;
            ActualChart.CategoryAxis.IsLogarithmic = true;
            ActualChart.CategoryAxis.IsPlotOrderReversed = true;
            ActualChart.CategoryAxis.LogBase = 2;
            ActualChart.CategoryAxis.MaxValue = 8;
            ActualChart.CategoryAxis.MinValue = 0.125;
            ActualChart.CategoryAxis.CrossAt = 1.5;
            ActualChart.CategoryAxis.TickLabelPosition = TickLabelPositionType.Low;


            ActualChart.ShowLegend = false;
            AsposeBook.Save(Constants.destPath + &quot;TEST_ChartAxisLogBase_2.xlsx&quot;);

        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


