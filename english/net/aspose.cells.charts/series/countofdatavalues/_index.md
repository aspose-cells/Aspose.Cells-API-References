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
// Called: Assert.AreEqual(3, chart.NSeries[0].CountOfDataValues, "ChartDataCount");
public void Series_Property_CountOfDataValues()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    for (int i = 0; i < 4; i++)
    {
        cells[i, 1].PutValue(i);
    }
    Name name = wb.Worksheets.Names[wb.Worksheets.Names.Add("testname")];
    string fml = "IFERROR(Sheet1!$B$2:$B$4,-1)";
    name.RefersTo = fml;
    cells["C1"].Formula = "=testname";
    cells["D1"].Formula = "SUM(testname)";
    cells["E1"].Formula = fml;
    cells["F1"].Formula = "SUM(" + fml + ")";
    wb.CalculateFormula(false);
    Assert.AreEqual(-1.0, cells["E1"].DoubleValue, "E1");
    Assert.AreEqual(-1.0, cells["F1"].DoubleValue, "E1");
    Assert.AreEqual(1.0, cells["C1"].DoubleValue, "C1");
    Assert.AreEqual(6.0, cells["D1"].DoubleValue, "D1");
    Aspose.Cells.Range r = name.GetRange(true);
    if (r == null || r.FirstRow != 1 || r.FirstColumn != 1 || r.RowCount != 3 || r.ColumnCount != 1)
    {
        Assert.Fail("Name.GetRange should return B2:B4");
    }
    Chart chart = wb.Worksheets[0].Charts[wb.Worksheets[0].Charts.Add(ChartType.Column, 10, 1, 20, 5)];
    chart.NSeries.Add("testname", true);
    Assert.AreEqual(3, chart.NSeries[0].CountOfDataValues, "ChartDataCount");
}
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


