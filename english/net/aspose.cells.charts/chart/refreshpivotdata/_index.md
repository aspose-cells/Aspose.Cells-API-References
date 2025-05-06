---
title: Chart.RefreshPivotData
second_title: Aspose.Cells for .NET API Reference
description: Chart method. Refreshes charts data from pivot table
type: docs
url: /net/aspose.cells.charts/chart/refreshpivotdata/
---
## Chart.RefreshPivotData method

Refreshes chart's data from pivot table.

```csharp
public void RefreshPivotData()
```

### Remarks

We will gather data from pivot data source to the pivot table report. This method is only used to gather all data to a pivot chart.

### Examples

```csharp
// Called: chart.RefreshPivotData();
[Test]
        public void Method_RefreshPivotData()
        {
            string filePath = Constants.PivotTableSourcePath + &quot;NET49385_&quot;;
            string savePath = CreateFolder(filePath);

            Workbook wb = new Workbook(filePath + &quot;Input.xlsx&quot;);

            for (int i = 0; i &lt; wb.Worksheets.Count; i++)
            {
                foreach (Chart chart in wb.Worksheets[i].Charts)
                    chart.RefreshPivotData();

                foreach (PivotTable pivotTable in wb.Worksheets[i].PivotTables)
                {
                    pivotTable.RefreshData();
                    pivotTable.CalculateData();
                }
            }

            Assert.AreEqual(wb.Worksheets[&quot;TCD&quot;].Cells[&quot;G7&quot;].StringValue, &quot;-80.83%&quot;);
            Assert.AreEqual(wb.Worksheets[&quot;TCD&quot;].Cells[&quot;H10&quot;].StringValue, &quot;-75.00%&quot;);
            Assert.AreEqual(wb.Worksheets[&quot;TCD&quot;].Cells[&quot;G12&quot;].StringValue, &quot;-100.00%&quot;);

            PdfSaveOptions options = new PdfSaveOptions();
            options.OnePagePerSheet = true;
            wb.Save(savePath + &quot;Input_out.pdf&quot;, options);

            wb.Save(savePath + &quot;Input_out.xlsx&quot;, SaveFormat.Xlsx);

            wb = new Workbook(filePath + &quot;a.xlsx&quot;);

            for (int i = 0; i &lt; wb.Worksheets.Count; i++)
            {
                foreach (PivotTable pivotTable in wb.Worksheets[i].PivotTables)
                {
                    pivotTable.RefreshData();
                    pivotTable.CalculateData();
                }
            }

            Assert.AreEqual(wb.Worksheets[&quot;Sheet1&quot;].Cells[&quot;B14&quot;].StringValue, &quot;33.33%&quot;);
            Assert.AreEqual(wb.Worksheets[&quot;Sheet1&quot;].Cells[&quot;D14&quot;].StringValue, &quot;50.00%&quot;);

            Assert.AreEqual(wb.Worksheets[&quot;Sheet1&quot;].Cells[&quot;C22&quot;].StringValue, &quot;-33.33%&quot;);
            Assert.AreEqual(wb.Worksheets[&quot;Sheet1&quot;].Cells[&quot;G22&quot;].StringValue, &quot;-20.00%&quot;);

            Assert.AreEqual(wb.Worksheets[&quot;Sheet1&quot;].Cells[&quot;B30&quot;].StringValue, &quot;-50.00%&quot;);
            Assert.AreEqual(wb.Worksheets[&quot;Sheet1&quot;].Cells[&quot;D30&quot;].StringValue, &quot;-25.00%&quot;);

            wb.Save(savePath + &quot;a_out.pdf&quot;, options);
            wb.Save(savePath + &quot;a_out.xlsx&quot;, SaveFormat.Xlsx);
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


