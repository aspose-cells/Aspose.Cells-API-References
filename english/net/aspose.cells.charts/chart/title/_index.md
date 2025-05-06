---
title: Chart.Title
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the charts title
type: docs
url: /net/aspose.cells.charts/chart/title/
---
## Chart.Title property

Gets the chart's title.

```csharp
public Title Title { get; }
```

### Examples

```csharp
// Called: chChart.Title.Font.Color = System.Drawing.Color.Blue;
[Test]
        public void Property_Title()
        {

            //Create a new Workbook.
            Workbook workbook = new Workbook();
            //Get the first worksheet.
            Worksheet sheet = workbook.Worksheets[0];

            //Set the name of worksheet


            sheet.Cells[0, 1].PutValue(&quot;column 1&quot;);
            sheet.Cells[0, 2].PutValue(&quot;column 2&quot;);
            sheet.Cells[1, 0].PutValue(&quot;alternative 1&quot;);
            sheet.Cells[2, 0].PutValue(&quot;alternative 2&quot;);
            sheet.Cells[3, 0].PutValue(&quot;alternative 3&quot;);

            sheet.Cells[1, 1].PutValue(0.25);
            sheet.Cells[2, 1].PutValue(0.5);
            sheet.Cells[3, 1].PutValue(0.25);
            sheet.Cells[1, 2].PutValue(0.33);
            sheet.Cells[2, 2].PutValue(0.33);
            sheet.Cells[3, 2].PutValue(0.33);
            int index = workbook.Worksheets.Add(SheetType.Chart);
            sheet = workbook.Worksheets[index];

            sheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chChart = sheet.Charts[sheet.Charts.Count - 1];
            chChart.ChartArea.Area.Formatting = FormattingType.None;
            chChart.NSeries.Add(&quot;Sheet1!B2:C4&quot;, true);

            chChart.ChartObject.Name = &quot;Chart1&quot;;
            chChart.Title.Text = &quot;Test&quot;;
            chChart.Title.Font.Color = System.Drawing.Color.Blue;
            chChart.Title.Font.IsBold = true;
            chChart.ValueAxis.MajorGridLines.Color = Color.Red;
            workbook.Save(Constants.destPath + &quot;TestChartSheetFont_001.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;TestChartSheetFont_001.xls&quot;);

            chChart = workbook.Worksheets[1].Charts[0];

            Assert.IsTrue(chChart.Title.Font.IsBold);
            Assert.AreEqual(chChart.Title.Font.Color.ToArgb() &amp; 0xFFFFFF, System.Drawing.Color.Blue.ToArgb() &amp; 0xFFFFFF);
            Assert.AreEqual(chChart.ValueAxis.MajorGridLines.Color.ToArgb() &amp; 0xFFFFFF, Color.Red.ToArgb() &amp; 0xFFFFFF);
        }
```

### See Also

* class [Title](../../title/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


