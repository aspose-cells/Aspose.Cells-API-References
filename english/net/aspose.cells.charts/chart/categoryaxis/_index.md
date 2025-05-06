---
title: Chart.CategoryAxis
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the charts X axis
type: docs
url: /net/aspose.cells.charts/chart/categoryaxis/
---
## Chart.CategoryAxis property

Gets the chart's X axis.

```csharp
public Axis CategoryAxis { get; }
```

### Examples

```csharp
// Called: chart.CategoryAxis.TickLabels.NumberFormat = &amp;quot;0000&amp;quot;;
[Test]
        public void Property_CategoryAxis()
        {
            const int MIN_YEAR = 2010;
            const int MAX_YEAR = 2020;

            Workbook wb = new Workbook();

            // Obtaining the reference of the newly added worksheet by passing its sheet index
            Worksheet currentWS = wb.Worksheets[0];
            Series aSerie = null;
            StringBuilder strB = null;
            int chartIndex = currentWS.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 0, 0, 25, 10);
            Aspose.Cells.Charts.Chart chart = currentWS.Charts[chartIndex];
            //not show not defined values                
            //chart.PlotEmptyCellsType = PlotEmptyCellsType.NotPlotted;
            //chart.PlotVisibleCells = true;

            //settings for X-Axis    
            chart.CategoryAxis.MaxValue = MAX_YEAR;
            //Set the min value of value axis
            chart.CategoryAxis.MinValue = MIN_YEAR;
            //Set the major unit
            // chart.CategoryAxis.MajorUnit = 1;
            //Set the number of categories or series between tick-mark labels. 
            chart.CategoryAxis.TickLabelSpacing = 1;
            chart.CategoryAxis.TickLabels.NumberFormat = &quot;0000&quot;;
            chart.CategoryAxis.TickLabels.Font.Size = 8;
            chart.CategoryAxis.Title.Text = &quot;Jahr&quot;;

            //settings for Y-Axis    
            chart.ValueAxis.Title.Text = &quot;Beitrag, €&quot;;
            chart.ValueAxis.TickLabelPosition = TickLabelPositionType.Low;

            chart.Legend.Position = LegendPositionType.Bottom;

            //  chart.PlotArea.Area.ForegroundColor = System.Drawing.Color.White;

            Dictionary&lt;int, PriceObj&gt; btg1 = new Dictionary&lt;int, PriceObj&gt;();
            Dictionary&lt;int, PriceObj&gt; btg2 = new Dictionary&lt;int, PriceObj&gt;();

            Random rnd = new Random();
            StringBuilder xValues = new StringBuilder();
            xValues.Append(&quot;{&quot;);
            for (int i = MIN_YEAR; i &lt;= MAX_YEAR; i++)
            {
                btg1[i] = new PriceObj(rnd.NextDouble() * 500);
                btg2[i] = new PriceObj(rnd.NextDouble() * 500);

                xValues.Append(i.ToString());
                if (i &lt; MAX_YEAR)
                    xValues.Append(&quot;,&quot;);
            }
            xValues.Append(&quot;}&quot;);

            btg2[MIN_YEAR] = null;
            btg2[MIN_YEAR + 1] = null;
            btg2[MIN_YEAR + 2] = null;

            List&lt;Dictionary&lt;int, PriceObj&gt;&gt; currentPKVTarifs = new List&lt;Dictionary&lt;int, PriceObj&gt;&gt;();
            currentPKVTarifs.Add(btg1);
            currentPKVTarifs.Add(btg2);

            int iCounter = 0;
            foreach (Dictionary&lt;int, PriceObj&gt; pT in currentPKVTarifs)
            {
                strB = new StringBuilder();
                strB.Append(&quot;{&quot;);
                for (int i = MIN_YEAR; i &lt;= MAX_YEAR; i++)
                {
                    //copy+past Jahr-Column for every year in history
                    PriceObj btgEl = pT[i];
                    strB.Append(btgEl == null ? String.Empty : btgEl.priceVal.ToString(&quot;#0.00&quot;).Replace(&quot;,&quot;, &quot;.&quot;));
                    if (i &lt; MAX_YEAR)
                        strB.Append(&quot;,&quot;);
                }
                strB.Append(&quot;}&quot;);

                aSerie = chart.NSeries[chart.NSeries.Add(strB.ToString(), true)];
                aSerie.Name = &quot;Tarif&quot; + (++iCounter).ToString();
                aSerie.XValues = xValues.ToString();

                //aSerie.Border.Color = System.Drawing.Color.Red;
                //aSerie.Border.Weight = Aspose.Cells.Drawing.WeightType.MediumLine;
            }

            string storedFileXlsx = Constants.destPath + &quot;CellsNet47420.xlsx&quot;;
            if (System.IO.File.Exists(storedFileXlsx))
                System.IO.File.Delete(storedFileXlsx);
            wb.Save(storedFileXlsx, SaveFormat.Xlsx);
            Workbook workbook = new Workbook(storedFileXlsx);
            Assert.IsNull(workbook.Worksheets[0].Charts[0].CategoryAxis.MinValue);
        }
```

### See Also

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


