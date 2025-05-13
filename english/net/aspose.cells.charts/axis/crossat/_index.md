---
title: Axis.CrossAt
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents the point on the value axis where the category axis crosses it
type: docs
url: /net/aspose.cells.charts/axis/crossat/
---
## Axis.CrossAt property

Represents the point on the value axis where the category axis crosses it.

```csharp
public double CrossAt { get; set; }
```

### Remarks

The number should be a integer when it applies to category axis. And the value must be between 1 and 31999.

### Examples

```csharp
// Called: ActualChart.CategoryAxis.CrossAt = 1.5;
//http://www.aspose.com/community/forums/thread/223664.aspx
public void Axis_Property_CrossAt()
{
    Console.WriteLine("Axis_Property_CrossAt()");
    string outfn = Constants.destPath + "Test_BubbleChartAxCrossAt_out.xlsx";

    Workbook AsposeBook = new Workbook();
    int SheetIndex = AsposeBook.Worksheets.Add();
    Worksheet ActualChartSheet = AsposeBook.Worksheets[SheetIndex];
    SheetIndex = AsposeBook.Worksheets.Add();
    Worksheet DataSheet = AsposeBook.Worksheets[SheetIndex];
    DataSheet.IsVisible = false;
    DataSheet.Name = "DataSheet";


    int ChartIndex = ActualChartSheet.Charts.Add(ChartType.Line, 0, 0, 30, 10);
    Chart ActualChart = ActualChartSheet.Charts[ChartIndex];


    double[] XValues = { 2.4, 0.3, 0.2, 1.1, 2.3, 2.1, 0.3, 0.2, 0.128, 0.4, 0.2, 1.2, 0.7, 0.13, 0.13 };
    double[] Yvalues = { 0.867, -0.00141, 0.113, 0.028, 0.399, -0.18, 0.072, -0.237, 0.420, -0.132, -0.0125, 0.0405, -0.0479, -0.112, -0.1441 };
    double[] ZValues = { 1991446, 1416791, 1266904, 942250, 803036, 731421, 344330, 333208, 261988, 260854, 252742, 193094, 180512, 158543, 145193 };


    ActualChart.Title.Text = "Example Bubble Chart";
    SeriesCollection AspSeries = ActualChart.NSeries;
    int SerieCount = AspSeries.Add("DataSheet!A1:A15", true);
    Series MySerie = AspSeries[SerieCount];
    MySerie.Type = ChartType.Bubble3D;
    MySerie.PlotOnSecondAxis = false;
    MySerie.Name = "Example Column Chart";


    DataSheet.Cells.ImportArray(XValues, 0, 0, true);
    MySerie.XValues = "DataSheet!$A$1:$A$15";
    DataSheet.Cells.ImportArray(Yvalues, 0, 1, true);
    MySerie.Values = "DataSheet!$B$1:$B$15";
    DataSheet.Cells.ImportArray(ZValues, 0, 2, true);
    MySerie.BubbleSizes = "DataSheet!$C$1:$C$15";


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
    AsposeBook.Save(outfn);
}
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


