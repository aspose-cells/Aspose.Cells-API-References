---
title: Chart.Calculate
second_title: Aspose.Cells for .NET API Reference
description: Chart method. Calculates the custom position of plot area axes if the position of them are auto assigned
type: docs
url: /net/aspose.cells.charts/chart/calculate/
---
## Calculate() {#calculate}

Calculates the custom position of plot area, axes if the position of them are auto assigned.

```csharp
public void Calculate()
```

### Examples

```csharp
// Called: chart.Calculate();
public void Chart_Method_Calculate()
{
    //CELLSJAVA-42195.xlsx
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    Workbook chartBook = new Workbook();

    //Copy Workbook 
    chartBook.Copy(workbook);

    WorksheetCollection sheets = chartBook.Worksheets;
    //  clearNonChartData(sheets);

    Worksheet sheet1 = sheets[0];
    //sheet1.getCells().clear(); 

    ChartCollection charts = sheet1.Charts;
    for (int i = 0; i < charts.Count; i++)
    {

        Chart chart = sheet1.Charts[i];
        chart.Calculate();

        //Set chart ImageOrPrintOptions 
        ImageOrPrintOptions options = new ImageOrPrintOptions();
        chart.ToImage(Constants.destPath + "example.jpg", options);
    }
    Util.SaveManCheck(workbook, "Shape", "example.xlsx");
}
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Calculate(ChartCalculateOptions) {#calculate_1}

Calculates the custom position of plot area, axes if the position of them are auto assigned, with Chart Calculate Options.

```csharp
public void Calculate(ChartCalculateOptions calculateOptions)
```

### Examples

```csharp
// Called: chart.Calculate(calculateOptions);
public void Chart_Method_Calculate()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Chart chart = workbook.Worksheets[0].Charts[0];
    ChartPointCollection points = chart.NSeries[0].Points;
    Assert.AreEqual(string.Empty, points[0].DataLabels.Text, "DataLabel Text");
    Assert.AreEqual(null, points[1].DataLabels.Text, "DataLabel Text");
    ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
    calculateOptions.UpdateAllPoints = true;
    chart.Calculate(calculateOptions);
    Assert.AreEqual(string.Empty, points[0].DataLabels.Text, "DataLabel Text"); // rich has no chars
    Assert.AreEqual("200", points[1].DataLabels.Text, "DataLabel Text");
    Assert.AreEqual("150", points[2].DataLabels.Text, "DataLabel Text"); // rich contains chars
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    chart = workbook.Worksheets[0].Charts[0];
    Assert.AreEqual(string.Empty, points[0].DataLabels.Text, "DataLabel Text");
    Assert.AreEqual("200", points[1].DataLabels.Text, "DataLabel Text");
    Assert.AreEqual("150", points[2].DataLabels.Text, "DataLabel Text");
    chart.Calculate(calculateOptions);
    points = chart.NSeries[0].Points;
    Assert.AreEqual(string.Empty, points[0].DataLabels.Text, "DataLabel Text");
    Assert.AreEqual("200", points[1].DataLabels.Text, "DataLabel Text");
    Assert.AreEqual("150", points[2].DataLabels.Text, "DataLabel Text");
}
```

### See Also

* class [ChartCalculateOptions](../../chartcalculateoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


