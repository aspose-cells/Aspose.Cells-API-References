---
title: Series.Values
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents the Y values of this chart series
type: docs
url: /net/aspose.cells.charts/series/values/
---
## Series.Values property

Represents the Y values of this chart series.

```csharp
public string Values { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("='Tableau et graphique'!$E$17:$E$30", chart.NSeries[3].Values);
[Test]
        public void Property_Values()
        {
            LoadOptions options = new LoadOptions();
            options.WarningCallback = new NumbersWarningCallback();
            Workbook wb = new Workbook(Constants.sourcePath + "Numbers13/ods.numbers", options);
            //wb.Save(Constants.destPath + @"Numbers13\ods.ods");
            wb = Util.ReSave(wb, SaveFormat.Ods);
            Cells cell = wb.Worksheets[0].Cells;
            Assert.AreEqual("kWh= 0.1712 €", cell["A31"].StringValue);
            Assert.AreEqual("13,710", cell["B32"].StringValue);
            Assert.AreEqual("=SUM(B17:B31)", cell["B32"].Formula);
            Assert.AreEqual("11 165 kWh.", cell["B35"].StringValue);
            Assert.AreEqual("=SUM(H17:H32)", cell["H33"].Formula);
            Assert.AreEqual("227", cell["H33"].StringValue);
            Chart chart = wb.Worksheets[0].Charts[0];
            Assert.AreEqual(4, chart.NSeries.Count);
            Assert.AreEqual("='Tableau et graphique'!$B$16", chart.NSeries[0].Name);
            Assert.AreEqual("='Tableau et graphique'!$B$17:$B$30", chart.NSeries[0].Values);
            Assert.AreEqual("='Tableau et graphique'!$C$16", chart.NSeries[1].Name);
            Assert.AreEqual("='Tableau et graphique'!$C$17:$C$30", chart.NSeries[1].Values);
            Assert.AreEqual("='Tableau et graphique'!$D$16", chart.NSeries[2].Name);
            Assert.AreEqual("='Tableau et graphique'!$D$17:$D$30", chart.NSeries[2].Values);
            Assert.AreEqual("='Tableau et graphique'!$E$16", chart.NSeries[3].Name);
            Assert.AreEqual("='Tableau et graphique'!$E$17:$E$30", chart.NSeries[3].Values);
        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


