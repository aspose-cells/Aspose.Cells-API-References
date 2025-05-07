---
title: Axis.TickLabelSpacing
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents the number of categories or series between tickmark labels. Applies only to category and series axes
type: docs
url: /net/aspose.cells.charts/axis/ticklabelspacing/
---
## Axis.TickLabelSpacing property

Represents the number of categories or series between tick-mark labels. Applies only to category and series axes.

```csharp
public int TickLabelSpacing { get; set; }
```

### Remarks

The number must be between 1 and 31999.

### Examples

```csharp
// Called: chart.CategoryAxis.TickLabelSpacing = 1;
[Test]
        public void Property_TickLabelSpacing()
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
            chart.CategoryAxis.TickLabels.NumberFormat = "0000";
            chart.CategoryAxis.TickLabels.Font.Size = 8;
            chart.CategoryAxis.Title.Text = "Jahr";

            //settings for Y-Axis    
            chart.ValueAxis.Title.Text = "Beitrag, €";
            chart.ValueAxis.TickLabelPosition = TickLabelPositionType.Low;

            chart.Legend.Position = LegendPositionType.Bottom;

            //  chart.PlotArea.Area.ForegroundColor = System.Drawing.Color.White;

            Dictionary<int, PriceObj> btg1 = new Dictionary<int, PriceObj>();
            Dictionary<int, PriceObj> btg2 = new Dictionary<int, PriceObj>();

            Random rnd = new Random();
            StringBuilder xValues = new StringBuilder();
            xValues.Append("{");
            for (int i = MIN_YEAR; i <= MAX_YEAR; i++)
            {
                btg1[i] = new PriceObj(rnd.NextDouble() * 500);
                btg2[i] = new PriceObj(rnd.NextDouble() * 500);

                xValues.Append(i.ToString());
                if (i < MAX_YEAR)
                    xValues.Append(",");
            }
            xValues.Append("}");

            btg2[MIN_YEAR] = null;
            btg2[MIN_YEAR + 1] = null;
            btg2[MIN_YEAR + 2] = null;

            List<Dictionary<int, PriceObj>> currentPKVTarifs = new List<Dictionary<int, PriceObj>>();
            currentPKVTarifs.Add(btg1);
            currentPKVTarifs.Add(btg2);

            int iCounter = 0;
            foreach (Dictionary<int, PriceObj> pT in currentPKVTarifs)
            {
                strB = new StringBuilder();
                strB.Append("{");
                for (int i = MIN_YEAR; i <= MAX_YEAR; i++)
                {
                    //copy+past Jahr-Column for every year in history
                    PriceObj btgEl = pT[i];
                    strB.Append(btgEl == null ? String.Empty : btgEl.priceVal.ToString("#0.00").Replace(",", "."));
                    if (i < MAX_YEAR)
                        strB.Append(",");
                }
                strB.Append("}");

                aSerie = chart.NSeries[chart.NSeries.Add(strB.ToString(), true)];
                aSerie.Name = "Tarif" + (++iCounter).ToString();
                aSerie.XValues = xValues.ToString();

                //aSerie.Border.Color = System.Drawing.Color.Red;
                //aSerie.Border.Weight = Aspose.Cells.Drawing.WeightType.MediumLine;
            }

            string storedFileXlsx = Constants.destPath + "CellsNet47420.xlsx";
            if (System.IO.File.Exists(storedFileXlsx))
                System.IO.File.Delete(storedFileXlsx);
            wb.Save(storedFileXlsx, SaveFormat.Xlsx);
            Workbook workbook = new Workbook(storedFileXlsx);
            Assert.IsNull(workbook.Worksheets[0].Charts[0].CategoryAxis.MinValue);
        }
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


