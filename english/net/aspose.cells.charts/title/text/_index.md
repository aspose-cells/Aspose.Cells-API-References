---
title: Title.Text
second_title: Aspose.Cells for .NET API Reference
description: Title property. Gets or sets the text of display unit label
type: docs
url: /net/aspose.cells.charts/title/text/
---
## Title.Text property

Gets or sets the text of display unit label.

```csharp
public override string Text { get; set; }
```

### Examples

```csharp
// Called: if (chart.Title.Text != null && chart.Title.Text == "<My Title>")
[Test]
        // SLIDESNET-25456 - After updating chart data cells it failed to edit chart in PowerPoint (related issue)
        // http://gemini.aspose.com:8042/issue/ViewIssue.aspx?ID=25953&PROJID=15
        public void Property_Text()
        {
            Console.WriteLine("Property_Text()");
            string infn = path + @"20110411\ChartTitle\ChartTitleTest.xlsx";

            Workbook workbook = new Workbook(infn);

            // worksheet has chart originally titled "<My Title>"
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];
            Assert.AreEqual("<My Title>", chart.Title.Text);
            // title should be "<My Title>" but it is null!
            if (chart.Title.Text != null && chart.Title.Text == "<My Title>")
            {
                chart.Title.Text = "New Title"; // never gets here!
            }
            Util.SaveManCheck(workbook, "ExcelUI", "BugChartTitleTest.xlsx");
            // saved chart will show "Chart Title"!
        }
```

### See Also

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


