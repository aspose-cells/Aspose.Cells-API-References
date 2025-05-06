---
title: ChartCalculateOptions.ChartCalculateOptions
second_title: Aspose.Cells for .NET API Reference
description: ChartCalculateOptions constructor. Creates the options for calculating chart
type: docs
url: /net/aspose.cells.charts/chartcalculateoptions/chartcalculateoptions/
---
## ChartCalculateOptions constructor

Creates the options for calculating chart.

```csharp
public ChartCalculateOptions()
```

### Examples

```csharp
// Called: ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
[Test]
        public void ChartCalculateOptions_Constructor()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;LATAM&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;JAPAN/APAC&quot;);

            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Q3:17&quot;);
            worksheet.Cells[&quot;C1&quot;].PutValue(&quot;Q3:18&quot;);
            worksheet.Cells[&quot;D1&quot;].PutValue(&quot;Q3:19&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(35);
            worksheet.Cells[&quot;C2&quot;].PutValue(32);
            worksheet.Cells[&quot;D2&quot;].PutValue(31);
            worksheet.Cells[&quot;B3&quot;].PutValue(185);
            worksheet.Cells[&quot;C3&quot;].PutValue(202);
            worksheet.Cells[&quot;D3&quot;].PutValue(224);

            worksheet.Cells[&quot;B4&quot;].Formula = &quot;=SUM(B2:B3)&quot;;
            worksheet.Cells[&quot;C4&quot;].Formula = &quot;=SUM(C2:C3)&quot;;
            worksheet.Cells[&quot;D4&quot;].Formula = &quot;=SUM(D2:D3)&quot;;

            worksheet.Cells[&quot;F2&quot;].Formula = &quot;=B2/B$4&quot;;
            worksheet.Cells[&quot;F3&quot;].Formula = &quot;=B3/B$4&quot;;
            worksheet.Cells[&quot;G2&quot;].Formula = &quot;=C2/C$4&quot;;
            worksheet.Cells[&quot;G3&quot;].Formula = &quot;=C3/C$4&quot;;
            worksheet.Cells[&quot;H2&quot;].Formula = &quot;=D2/D$4&quot;;
            worksheet.Cells[&quot;H3&quot;].Formula = &quot;=D3/D$4&quot;;

            //Format cell B2 with $ formatting
            Style st = worksheet.Cells[&quot;B2&quot;].GetStyle();
            st.Custom = &quot;$#,##0;$-#,##0&quot;;
            worksheet.Cells[&quot;B2&quot;].SetStyle(st);

            //Make the entire column with $ formatting
            StyleFlag flg = new StyleFlag();
            flg.NumberFormat = true;
            worksheet.Cells.Columns[1].ApplyStyle(st, flg);
            worksheet.Cells.Columns[2].ApplyStyle(st, flg);
            worksheet.Cells.Columns[3].ApplyStyle(st, flg);

            workbook.CalculateFormula();
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.ColumnStacked, 7, 1, 25, 5);
            // Accessing the instance of the newly added chart
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.Title.Text = &quot;Sales by segment&quot;;
            chart.NSeries.Add(&quot;B2:D2&quot;, false);
            chart.NSeries.Add(&quot;B3:D3&quot;, false);
            chart.NSeries.Add(&quot;B4:D4&quot;, false);
            chart.NSeries.CategoryData = &quot;B1:D1&quot;;

            for (int i = 0; i &lt; chart.NSeries.Count; i++)
            {
                DataLabels dataLabels = chart.NSeries[i].DataLabels;
                dataLabels.ShowValue = true;
            }

            DataLabels dataLabels0 = chart.NSeries[0].DataLabels;
            dataLabels0.ShowCellRange = true;
            dataLabels0.ShowPercentage = true;
            dataLabels0.LinkedSource = &quot;=Sheet1!$F$2:$H$2&quot;;
            DataLabels dataLabels1 = chart.NSeries[1].DataLabels;
            dataLabels1.ShowCellRange = true;
            dataLabels1.ShowPercentage = true;
            dataLabels1.LinkedSource = &quot;=Sheet1!$F$3:$H$3&quot;;

            Style style = workbook.CreateStyle();
            StyleFlag flag = new StyleFlag { NumberFormat = true };
            style.Custom = &quot;0%&quot;;
            //Apply style to complete column
            worksheet.Cells.Columns[5].ApplyStyle(style, flag);
            worksheet.Cells.Columns[6].ApplyStyle(style, flag);
            worksheet.Cells.Columns[7].ApplyStyle(style, flag);

            workbook.Save(Constants.destPath + &quot;CELLSNET49191.xlsx&quot;);

            workbook = new Workbook(workbook.FileName);
            chart = workbook.Worksheets[0].Charts[chartIndex];
            ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
            calculateOptions.UpdateAllPoints = true;
            chart.Calculate(calculateOptions);
            //chart.ToImage(Constants.destPath + &quot;CELLSNET49191.png&quot;);
            var points = chart.NSeries[0].Points;
            Assert.AreEqual(&quot;16%, $35&quot;, points[0].DataLabels.Text, &quot;DataLabel Text&quot;);
            Assert.AreEqual(&quot;14%, $32&quot;, points[1].DataLabels.Text, &quot;DataLabel Text&quot;);
            Assert.AreEqual(&quot;12%, $31&quot;, points[2].DataLabels.Text, &quot;DataLabel Text&quot;);
            points = chart.NSeries[1].Points;
            Assert.AreEqual(&quot;84%, $185&quot;, points[0].DataLabels.Text, &quot;DataLabel Text&quot;);
            Assert.AreEqual(&quot;86%, $202&quot;, points[1].DataLabels.Text, &quot;DataLabel Text&quot;);
            Assert.AreEqual(&quot;88%, $224&quot;, points[2].DataLabels.Text, &quot;DataLabel Text&quot;);

            
        }
```

### See Also

* class [ChartCalculateOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


