---
title: Chart.Calculate
second_title: Aspose.Cells for .NET API Reference
description: Chart method. Calculates the custom position of plot area axes if the position of them are auto assigned
type: docs
url: /net/aspose.cells.charts/chart/calculate/
---
## Calculate() {#calculate}

Calculates the custom position of plot area, axes if the position of them are auto assigned.

```csharp
public void Calculate()
```

### Examples

```csharp
// Called: charts[j].Calculate();
[Test]
        public void Method_Calculate()
        {
            String filePath = Constants.PivotTableSourcePath + @&quot;JAVA41968_&quot;;

            Workbook workbook = new Workbook(filePath + &quot;aspose.xlsx&quot;);
            ChartCollection charts = workbook.Worksheets[&quot;Tabelle2&quot;].Charts;
            for (int j = 0; j &lt; charts.Count; j++)
            {
                charts[j].RefreshPivotData();
                charts[j].Calculate();
            }

            workbook.Save(Constants.PivotTableDestPath + @&quot;JAVA41968_&quot; + &quot;out.pdf&quot;);
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Calculate(ChartCalculateOptions) {#calculate_1}

Calculates the custom position of plot area, axes if the position of them are auto assigned, with Chart Calculate Options.

```csharp
public void Calculate(ChartCalculateOptions calculateOptions)
```

### Examples

```csharp
// Called: chart.Calculate(calculateOptions);
[Test]
        public void Method_ChartCalculateOptions_()
        {
            String dataDir = Constants.destPath;
            // Create an instance of Workbook in XLSX format
            Workbook workbook = new Workbook(FileFormatType.Xlsx);

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add two columns of data
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Retail&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;Services&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Info &amp; Communication&quot;);
            worksheet.Cells[&quot;A4&quot;].PutValue(&quot;Transport Equip&quot;);
            worksheet.Cells[&quot;A5&quot;].PutValue(&quot;Construction&quot;);

            worksheet.Cells[&quot;B1&quot;].PutValue(98.0);
            worksheet.Cells[&quot;B2&quot;].PutValue(0.5);
            worksheet.Cells[&quot;B3&quot;].PutValue(0.5);
            worksheet.Cells[&quot;B4&quot;].PutValue(0.5);
            worksheet.Cells[&quot;B5&quot;].PutValue(0.5);

            // Create a pie chart and add it to the collection of charts
            int id = worksheet.Charts.Add(ChartType.Doughnut, 3, 3, 23, 10);
            // Access newly created Chart instance
            Chart chart = worksheet.Charts[id];

            // Set series data range
            chart.NSeries.Add(&quot;B1:B5&quot;, true);
            // Set category data range
            chart.NSeries.CategoryData = &quot;A1:A5&quot;;
            // Turn off legend
            chart.ShowLegend = false;

            // Access data labels
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            // Turn on percentage format
            dataLabels.ShowPercentage = true;
            // Set position
            dataLabels.Position = LabelPositionType.OutsideEnd;

            //Turn on leader lines
            chart.NSeries[0].HasLeaderLines = true;

            //chart.getChartArea().getFont().setName(&quot;Century Gothic&quot;);
            chart.ChartArea.Font.Name = &quot;Century Gothic&quot;;
            chart.ChartArea.Font.Size = 10;

            chart.ChartArea.Area.ForegroundColor = Color.FromArgb(0, 0, 0);
            chart.ChartArea.Area.Transparency = 1;
            chart.PlotArea.Area.ForegroundColor = Color.FromArgb(0, 0, 0);
            chart.PlotArea.Area.Transparency = 1;
            chart.ChartArea.Border.IsVisible = false;
            chart.PlotArea.Border.IsVisible = false;

            //Calculate chart
            ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
            calculateOptions.UpdateAllPoints = true;
            chart.Calculate(calculateOptions);

            //You need to move DataLabels a little leftward or rightward depending on their position
            //to show leader lines
            int delta = 0;
            float minAngle = 10;
            double totalValue = 0;
            for (int i = 0; i &lt; chart.NSeries[0].Points.Count; i++)
            {
                totalValue += Double.Parse(chart.NSeries[0].Points[i].YValue.ToString());
            }
            for (int i = chart.NSeries[0].Points.Count - 1; i &gt;= 0; i--)
            {
                ChartPoint point = chart.NSeries[0].Points[i];

                point.DataLabels.IsResizeShapeToFitText = (false);
                point.DataLabels.IsTextWrapped = (false);

                point.DataLabels.NumberFormat = (&quot;#0.00%&quot;);
                int X = point.DataLabels.X;
                int Y = point.DataLabels.Y;
                double val = Double.Parse(point.YValue.ToString());
                double angle = val / totalValue * 360;
                int deltaX = delta;
                int deltaY = -100;
                if (angle &lt; minAngle)
                {
                    int k = i + 1;
                    while (k &lt; chart.NSeries[0].Points.Count)
                    {
                        val += Double.Parse(chart.NSeries[0].Points[k].YValue.ToString());
                        if (val / totalValue * 360 &lt; minAngle)
                        {
                            deltaX += 350;
                        }
                        deltaY += 100;
                        k++;
                    }

                    // More offset is required for successive angles that are too small
                    delta += 100;
                }
                else
                {
                    delta = 0;
                    if (angle &gt; 2 * minAngle)
                        deltaX = 0;
                }

                if (deltaX == 0 &amp;&amp; angle &gt; minAngle)
                {
                    if (X &gt; 2000)
                    {
                        point.DataLabels.X = (X + 350);
                    }
                    else
                    {
                        point.DataLabels.X = (X - 350);
                    }
                }
                else if (deltaX &gt; 0)
                {
                    X -= deltaX;
                    Y += deltaY;
                    point.DataLabels.X = (X);
                    point.DataLabels.Y = (Y);
                }
                else if (Y &lt; 150)
                {
                    // set label further away from chart to make the leader line show
                    point.DataLabels.Y = (Y - 10);
                }
            }

            chart.Calculate();

            //In order to save the chart image, create an instance of ImageOrPrintOptions
            ImageOrPrintOptions anOption = new ImageOrPrintOptions();
            //Set image format
            anOption.ImageType = ImageType.Png;
            //Set resolution
            anOption.HorizontalResolution = 500;
            anOption.VerticalResolution = 500;

            //Render chart to image
            chart.ToImage(dataDir + &quot;CELLSJAVA44130.png&quot;, anOption);

            //Judging values
            Assert.AreEqual(chart.NSeries[0].Points.Count, 5);
            Assert.True(chart.NSeries[0].Points[0].DataLabels.Width &gt; 350); //wrong:268, correct:429
            Assert.True(chart.NSeries[0].Points[1].DataLabels.Width &gt; 280); //wrong:196, correct:366

            //Save the workbook to see chart inside the Excel
            workbook.Save(dataDir + &quot;CELLSJAVA44130.xlsx&quot;);
        }
```

### See Also

* class [ChartCalculateOptions](../../chartcalculateoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


