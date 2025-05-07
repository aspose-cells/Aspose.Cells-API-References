---
title: Series.BubbleScale
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 zero to 300 corresponding to a percentage of the default size. Applies only to bubble charts
type: docs
url: /net/aspose.cells.charts/series/bubblescale/
---
## Series.BubbleScale property

Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts.

```csharp
public int BubbleScale { get; set; }
```

### Examples

```csharp
// Called: aChart.NSeries[K].BubbleScale = 50;
[Test]
        public void Property_BubbleScale()
        {
            Console.WriteLine("Property_BubbleScale()");
            string outfn = Constants.destPath + "Test_CustomDataLabels_out.xlsx";

            double[] nameSeries = {
                                      1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23,
                                      24, 25,
                                      26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46
                                      , 47, 48
                                  };

            double[] serieX = {
                                  0.26, 0.16, 0.17, 0.10, 0.09, 2.26, 0.29, 0.03, 0.41, 0.21, 0.02, 0.78, 1.27, 0.14, 0.09,
                                  0.03, 0.08, 0.01, 0.08, 0.01, 0.25, 0.01, 0.03, 0.05, 0.32, 0.10, 1.00, 0.01, 0.01, 0.13,
                                  0.01, 0.02, 0.02, 0.01, 0.01, 0.01, 1.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00, 0.00,
                                  0.00, 0.00, 0.00
                              };
            double[] serieY = {
                                  0.2448738660, 1.4350222984, 0.7494378276, 1.2662960239, 0.0321888145, 0.6654144719,
                                  0.3832439407, 2.0247917795, 0.2902760709, 0.2453112295, 1.1855630275, 0.5462327141,
                                  0.2164425057, 2.1368291791, 0.0721144532, 0.2737299286, -0.2611136147, -0.5593772169,
                                  0.0211079380, 0.5852872395, 11.0259958872, -0.4526565817, -0.0994308093, -0.0398313922,
                                  0.0592413388, 2.2906237362, 0.0654417550, 0.2776674300, 0.6535332288, -0.2545607830,
                                  -0.0824537234, 0.7478201753, -0.1016664447, -0.0049290272, -0.1494419256, 31.7089290623,
                                  -0.0502815542, -0.0002826367, -0.0498523772, 0.5242816831, 4.8477334608, 20.5787261718,
                                  0.3688442066, 0.3428454022, -0.9626397863, -0.9247876376, 0.0000000000, 0.0000000000
                              };
            double[] serieZ = {
                                  24.48738660, 143.50222984, 74.94378276, 126.62960239, 3.21888145, 66.54144719,
                                  38.32439407, 202.47917795, 29.02760709, 24.53112295, 118.55630275, 54.62327141,
                                  21.64425057, 213.68291791, 7.21144532, 27.37299286, -26.11136147, -55.93772169,
                                  2.11079380, 58.52872395, 1102.59958872, -45.26565817, -9.94308093, -3.98313922,
                                  5.92413388, 229.06237362, 6.54417550, 27.76674300, 65.35332288, -25.45607830, -8.24537234
                                  , 74.78201753, -10.16664447, -0.49290272, -14.94419256, 3170.89290623, -5.02815542,
                                  -0.02826367, -4.98523772, 52.42816831, 484.77334608, 2057.87261718, 36.88442066,
                                  34.28454022, -96.26397863, -92.47876376, 0.00000000, 0.00000000
                              };

            Workbook wb1 = new Workbook(FileFormatType.Xlsx);
            Worksheet ws0 = wb1.Worksheets[0];
            Cells c0 = ws0.Cells;

            c0[0, 0].PutValue("Serie Name");
            c0[0, 1].PutValue("X");
            c0[0, 2].PutValue("Y");
            c0[0, 3].PutValue("Z");
            Style style1 = wb1.CreateStyle();
            style1.Custom = "0.00%";
            for (int i = 0; i < nameSeries.Length; ++i)
            {
                c0[i + 1, 0].PutValue(nameSeries[i]);
                c0[i + 1, 1].PutValue(serieX[i]);
                c0[i + 1, 2].PutValue(serieY[i]);
                c0[i + 1, 2].SetStyle(style1);
                c0[i + 1, 3].PutValue(serieZ[i]);
            }

            int chartIndex = ws0.Charts.Add(ChartType.Bubble, 0, 6, 25, 15);
            Chart aChart = ws0.Charts[chartIndex];

            for (int row = 2; row <= 49; ++row)
            {
                int indexSerie = aChart.NSeries.Add("Sheet1!" + IndexToR1C1(row, 2), true);
                aChart.NSeries[indexSerie].Name = "=Sheet1!" + IndexToR1C1(row, 0);
                aChart.NSeries[indexSerie].XValues = "=Sheet1!" + IndexToR1C1(row, 1);
                aChart.NSeries[indexSerie].BubbleSizes = "=Sheet1!" + IndexToR1C1(row + 1, 3);
            }

            for (int K = 0; K < aChart.NSeries.Count; ++K)
            {
                aChart.NSeries[K].IsColorVaried = false;
                aChart.NSeries[K].Area.FillFormat.SetOneColorGradient(Color.FromArgb(0, 236, 102, 102), 0.9, GradientStyleType.DiagonalDown, 2);
                aChart.NSeries[K].BubbleScale = 50;
            }

            aChart.CategoryAxis.MajorTickMark = TickMarkType.None;
            aChart.CategoryAxis.TickLabelSpacing = 2;
            aChart.CategoryAxis.TickLabelPosition = TickLabelPositionType.Low;
            aChart.CategoryAxis.Title.Text = "Title X";
            aChart.CategoryAxis.IsLogarithmic = true;
            aChart.CategoryAxis.LogBase = 2;
            aChart.CategoryAxis.CrossAt = 1;
            aChart.CategoryAxis.IsPlotOrderReversed = true;
            aChart.CategoryAxis.TickLabelPosition = TickLabelPositionType.Low;
            aChart.CategoryAxis.MinValue = 0.125;
            aChart.CategoryAxis.MaxValue = 8.0;

            aChart.ValueAxis.MinValue = -1.76;
            aChart.ValueAxis.MaxValue = 1.760;
            aChart.ValueAxis.TickLabelPosition = TickLabelPositionType.High;
            aChart.ValueAxis.MajorTickMark = TickMarkType.None;
            aChart.ValueAxis.MajorGridLines.IsVisible = false;
            aChart.ValueAxis.Title.Text = "Title Y";
            aChart.ValueAxis.CrossAt = 0.19;
            aChart.ValueAxis.TickLabelPosition = TickLabelPositionType.High;

            // All the object
            aChart.ChartArea.Area.ForegroundColor = Color.Transparent;
            //// Only the chart
            aChart.PlotArea.Area.ForegroundColor = Color.Transparent;
            aChart.PlotArea.Border.IsVisible = true;
            aChart.PlotArea.Border.Color = Color.Gray;
            aChart.PlotArea.Border.Style = LineType.Solid;

            aChart.ShowLegend = false;

            //#region Test 1
            //for (int i = 0; i < aChart.NSeries[0].Points.Count; i++)
            //{
            //  aChart.NSeries[0].Points[i].DataLabels.Text = "SR" + i.ToString();
            //}
            //#endregion

            #region Test 2
            for (int j = 0; j < aChart.NSeries.Count; ++j)
            {
                Series series = aChart.NSeries[j];
                series.DataLabels.ShowSeriesName = true;
                for (int i = 0; i < series.Points.Count; i++)
                {
                    series.Points[i].DataLabels.Text = "SR" + j.ToString() + ":" + i.ToString();
                }
            }
            #endregion

            //Saving the Excel file
            wb1.Save(outfn);

        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


