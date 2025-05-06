---
title: Series.CountOfDataValues
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets the number of the data values
type: docs
url: /net/aspose.cells.charts/series/countofdatavalues/
---
## Series.CountOfDataValues property

Gets the number of the data values.

```csharp
public int CountOfDataValues { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(3, chart.NSeries[0].CountOfDataValues, &amp;quot;ChartDataCount&amp;quot;);
[Test]
        public void Property_CountOfDataValues()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i &lt; 4; i++)
            {
                cells[i, 1].PutValue(i);
            }
            Name name = wb.Worksheets.Names[wb.Worksheets.Names.Add(&quot;testname&quot;)];
            string fml = &quot;IFERROR(Sheet1!$B$2:$B$4,-1)&quot;;
            name.RefersTo = fml;
            cells[&quot;C1&quot;].Formula = &quot;=testname&quot;;
            cells[&quot;D1&quot;].Formula = &quot;SUM(testname)&quot;;
            cells[&quot;E1&quot;].Formula = fml;
            cells[&quot;F1&quot;].Formula = &quot;SUM(&quot; + fml + &quot;)&quot;;
            wb.CalculateFormula(false);
            Assert.AreEqual(-1.0, cells[&quot;E1&quot;].DoubleValue, &quot;E1&quot;);
            Assert.AreEqual(-1.0, cells[&quot;F1&quot;].DoubleValue, &quot;E1&quot;);
            Assert.AreEqual(1.0, cells[&quot;C1&quot;].DoubleValue, &quot;C1&quot;);
            Assert.AreEqual(6.0, cells[&quot;D1&quot;].DoubleValue, &quot;D1&quot;);
            Aspose.Cells.Range r = name.GetRange(true);
            if (r == null || r.FirstRow != 1 || r.FirstColumn != 1 || r.RowCount != 3 || r.ColumnCount != 1)
            {
                Assert.Fail(&quot;Name.GetRange should return B2:B4&quot;);
            }
            Chart chart = wb.Worksheets[0].Charts[wb.Worksheets[0].Charts.Add(ChartType.Column, 10, 1, 20, 5)];
            chart.NSeries.Add(&quot;testname&quot;, true);
            Assert.AreEqual(3, chart.NSeries[0].CountOfDataValues, &quot;ChartDataCount&quot;);
        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


