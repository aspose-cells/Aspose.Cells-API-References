---
title: Title.IsVisible
second_title: Aspose.Cells for .NET API Reference
description: Title property. Represents whether the title is visible
type: docs
url: /net/aspose.cells.charts/title/isvisible/
---
## Title.IsVisible property

Represents whether the title is visible.

```csharp
public bool IsVisible { get; set; }
```

### Examples

```csharp
// Called: chart.CategoryAxis.Title.IsVisible = true;
[Test]
        public void Property_IsVisible()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA-43449.xlsx&quot;);
            for (int chartIndex = 0; chartIndex &lt; workbook.Worksheets[0].Charts.Count; chartIndex++)
            {
                Chart chart = workbook.Worksheets[0].Charts[chartIndex];
                chart.Title.IsVisible = true;
                chart.CategoryAxis.Title.IsVisible = true;
                chart.ValueAxis.Title.IsVisible = true;
                chart.CategoryAxis.Title.Font.Name = &quot;Arial&quot;;
                chart.ValueAxis.Title.Font.Name = &quot;Aktiv Grotesk&quot;;
                chart.Title.Font.Name = &quot;Aktiv Grotesk&quot;;
            }

            workbook.Save(Constants.destPath + &quot;CELLSJAVA-43449_Resave.xlsx&quot;);
            workbook = new Workbook(workbook.FileName);
            for (int chartIndex = 0; chartIndex &lt; workbook.Worksheets[0].Charts.Count; chartIndex++)
            {
                Chart chart = workbook.Worksheets[0].Charts[chartIndex];
                Assert.AreEqual(&quot;Arial&quot;, chart.CategoryAxis.Title.Font.Name, &quot;CategoryAxis Title Font Name&quot;);
                Assert.AreEqual(&quot;Aktiv Grotesk&quot;, chart.ValueAxis.Title.Font.Name, &quot;ValueAxis Title Font Name&quot;);
                Assert.AreEqual(&quot;Aktiv Grotesk&quot;, chart.Title.Font.Name, &quot;Chart Title Font Name&quot;);
            }

        }
```

### See Also

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


