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

            sheet.Cells["A2"].PutValue("カテゴリー1");
            sheet.Cells["A3"].PutValue("カテゴリー2");
            sheet.Cells["A4"].PutValue("カテゴリー3");
            sheet.Cells["B1"].PutValue("列 1");
            sheet.Cells["B2"].PutValue(4);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(50);
            sheet.Cells["C1"].PutValue("列 2");
            sheet.Cells["C2"].PutValue(50);
            sheet.Cells["C3"].PutValue(100);
            sheet.Cells["C4"].PutValue(150);

            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];

            chart.Title.Text = "マーケット";
            Aspose.Cells.Drawing.Texts.TextOptions textOptions = chart.Title.TextOptions;
            textOptions.LanguageCode = CountryCode.Japan;
            chart.SetChartDataRange("A1:C4", true);
            wb.Save(Constants.destPath + "CellsNet51924.xlsx");
            wb = new Workbook(Constants.destPath + "CellsNet51924.xlsx");
            Assert.AreEqual(CountryCode.Japan, wb.Worksheets[0].Charts[0].Title.TextOptions.LanguageCode);

        }
```

### See Also

* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


