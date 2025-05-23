---
title: AxisBins.IsByCategory
second_title: Aspose.Cells for .NET API Reference
description: AxisBins property. Indicates whether grouping data by category
type: docs
url: /net/aspose.cells.charts/axisbins/isbycategory/
---
## AxisBins.IsByCategory property

Indicates whether grouping data by category

```csharp
public bool IsByCategory { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(false, bins.IsByCategory, "By Category");
public void AxisBins_Property_IsByCategory()
{
    // CELLSNET49316
    Workbook workbook = new Workbook();
    Worksheet worksheet = workbook.Worksheets[0];

    worksheet.Cells["B1"].PutValue(10);
    worksheet.Cells["C1"].PutValue(20);
    worksheet.Cells["D1"].PutValue(15);
    worksheet.Cells["B2"].PutValue(35);
    worksheet.Cells["C2"].PutValue(32);
    worksheet.Cells["D2"].PutValue(31);
    worksheet.Cells["B3"].PutValue(185);
    worksheet.Cells["C3"].PutValue(202);
    worksheet.Cells["D3"].PutValue(224);
    int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Histogram, 7, 1, 25, 5);
    Chart chart = worksheet.Charts[chartIndex];
    chart.NSeries.Add("B2:D2", false);
    chart.NSeries.Add("B3:D3", false);
    chart.NSeries.Add("B4:D4", false);
    chart.NSeries.CategoryData = "B1:D1";
    chart.CategoryAxis.Bins.Width = 12;
    workbook.Save(Constants.destPath + "example.xlsx");

    workbook = new Workbook(workbook.FileName);
    var bins = workbook.Worksheets[0].Charts[0].CategoryAxis.Bins;
    Assert.AreEqual(false, bins.IsByCategory, "By Category");
    Assert.AreEqual(12, bins.Width, "Bin Width");
    bins.Count = 3;
    bins.Overflow = 10;
    bins.Underflow = 0.5;
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(workbook.FileName);
    bins = workbook.Worksheets[0].Charts[0].CategoryAxis.Bins;
    Assert.AreEqual(false, bins.IsByCategory, "By Category");
    ;
    Assert.AreEqual(3, bins.Count, "Bins Count");
    Assert.AreEqual(10, bins.Overflow, "Bin Overflow");
    Assert.AreEqual(0.5, bins.Underflow, "Bin Underflow");
}
```

### See Also

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


