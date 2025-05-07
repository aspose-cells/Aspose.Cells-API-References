---
title: DataLabels.Font
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets the font of the DataLabels
type: docs
url: /net/aspose.cells.charts/datalabels/font/
---
## DataLabels.Font property

Gets the font of the DataLabels;

```csharp
public override Font Font { get; }
```

### Examples

```csharp
// Called: Color c1 = d1.Font.Color;
[Test]
        public void Property_Font()
        {
            Workbook book = new Workbook(Constants.sourcePath + "Charts/BarChart_WhiteAndBlackLabels.xlsx");
            Chart chart1 = book.Worksheets[0].Charts[0];
            DataLabels d1 = chart1.NSeries[0].Points[0].DataLabels;
            Color c1 = d1.Font.Color;
            //book.Save(Constants.destPath + "BarChart_WhiteAndBlackLabels2.xlsx");
            //Workbook book2 = new Workbook(Constants.destPath + "BarChart_WhiteAndBlackLabels2.xlsx");
            Workbook book2 = Util.ReSave(book, SaveFormat.Xlsx);
            Chart chart2 = book2.Worksheets[0].Charts[0];
            DataLabels d2 = chart2.NSeries[0].Points[0].DataLabels;
            Color c2 = d2.Font.Color;
            Assert.AreEqual(c1, c2);
            //book2.Save(Constants.destPath + "BarChart_WhiteAndBlackLabels3.xlsx");
        }
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


