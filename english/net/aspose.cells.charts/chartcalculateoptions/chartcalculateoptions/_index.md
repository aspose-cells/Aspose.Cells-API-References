---
title: ChartCalculateOptions.ChartCalculateOptions
second_title: Aspose.Cells for .NET API Reference
description: ChartCalculateOptions constructor. Creates the options for calculating chart
type: docs
url: /net/aspose.cells.charts/chartcalculateoptions/chartcalculateoptions/
---
## ChartCalculateOptions constructor

Creates the options for calculating chart.

```csharp
public ChartCalculateOptions()
```

### Examples

```csharp
// Called: ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
public void ChartCalculateOptions_Constructor()
{
    var workbook = new Workbook(Path.Combine(Constants.sourcePath, "example.xlsx"));
    ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
    calculateOptions.UpdateAllPoints = true;

    Chart chart1 = workbook.Worksheets[0].Charts[0];
    chart1.Calculate(calculateOptions);
    // Assert.AreEqual(0, chart1.FirstSliceAngle);
    workbook.Save(Constants.destPath + "example.ods");
    workbook = new Workbook(Constants.destPath + "example.ods");
    Chart chart = workbook.Worksheets[0].Charts[0];
    //Color [A=255, R=68, G=114, B=196]
    Assert.IsTrue(Util.CompareColor(Color.FromArgb(68,114,196), chart.NSeries[0].Points[0].Area.ForegroundColor));
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ChartCalculateOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


