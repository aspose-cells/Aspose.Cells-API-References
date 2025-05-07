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
// Called: Assert.AreEqual(workbook.Worksheets[0].Charts[0].Title.TextFont.Name,
[Test]
        // Mo Shujun Issue
        public void Property_Title()
        {
            Console.WriteLine("Property_Title()");
            string infn = path + @"ChartTitleFont\test.xlsx";
            string outfn = Constants.destPath + @"ChartTitleFont.xlsx";

            Workbook workbook = new Workbook(infn);
            Assert.AreEqual(workbook.Worksheets[0].Charts[0].Title.TextFont.Name,
                workbook.Worksheets[1].Charts[0].Title.TextFont.Name);
            workbook.Save(outfn);
        }
```

### See Also

* class [Title](../../title/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


