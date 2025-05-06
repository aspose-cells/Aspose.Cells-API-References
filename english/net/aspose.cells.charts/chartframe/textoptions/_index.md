---
title: ChartFrame.TextOptions
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets and sets the options of the text
type: docs
url: /net/aspose.cells.charts/chartframe/textoptions/
---
## ChartFrame.TextOptions property

Gets and sets the options of the text.

```csharp
public virtual TextOptions TextOptions { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(CountryCode.Japan, wb.Worksheets[0].Charts[0].Title.TextOptions.LanguageCode);
[Test]
        public void Property_TextOptions()
        {
            var wb = new Workbook();
            //  wb.Settings.Region = CountryCode.Japan;
            Worksheet sheet = wb.Worksheets[0];

            sheet.Cells[&quot;A2&quot;].PutValue(&quot;カテゴリー1&quot;);
            sheet.Cells[&quot;A3&quot;].PutValue(&quot;カテゴリー2&quot;);
            sheet.Cells[&quot;A4&quot;].PutValue(&quot;カテゴリー3&quot;);
            sheet.Cells[&quot;B1&quot;].PutValue(&quot;列 1&quot;);
            sheet.Cells[&quot;B2&quot;].PutValue(4);
            sheet.Cells[&quot;B3&quot;].PutValue(20);
            sheet.Cells[&quot;B4&quot;].PutValue(50);
            sheet.Cells[&quot;C1&quot;].PutValue(&quot;列 2&quot;);
            sheet.Cells[&quot;C2&quot;].PutValue(50);
            sheet.Cells[&quot;C3&quot;].PutValue(100);
            sheet.Cells[&quot;C4&quot;].PutValue(150);

            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];

            chart.Title.Text = &quot;マーケット&quot;;
            Aspose.Cells.Drawing.Texts.TextOptions textOptions = chart.Title.TextOptions;
            textOptions.LanguageCode = CountryCode.Japan;
            chart.SetChartDataRange(&quot;A1:C4&quot;, true);
            wb.Save(Constants.destPath + &quot;CellsNet51924.xlsx&quot;);
            wb = new Workbook(Constants.destPath + &quot;CellsNet51924.xlsx&quot;);
            Assert.AreEqual(CountryCode.Japan, wb.Worksheets[0].Charts[0].Title.TextOptions.LanguageCode);

        }
```

### See Also

* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


