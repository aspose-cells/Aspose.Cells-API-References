---
title: DataLabels.ShowPercentage
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Represents a specified charts data label percentage value display behavior. True displays the percentage value. False to hide
type: docs
url: /net/aspose.cells.charts/datalabels/showpercentage/
---
## DataLabels.ShowPercentage property

Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide.

```csharp
public bool ShowPercentage { get; set; }
```

### Examples

```csharp
// Called: charts[0].NSeries[0].DataLabels.ShowPercentage = true;
[Test]
        public void Property_ShowPercentage()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "TestDoughnut_001.xls");
            ChartCollection charts = workbook.Worksheets[0].Charts;
            charts.Add(ChartType.Doughnut, 5, 5, 15, 10);
            charts[0].NSeries.Add("A1:B3", true);
            charts[0].NSeries[0].DataLabels.ShowPercentage = true;
            workbook.Save(Constants.destPath + "TestDoughnut_001.xls");
            workbook = new Workbook(Constants.destPath + "TestDoughnut_001.xls");
            Console.WriteLine(workbook.Worksheets[0].Charts[0].NSeries[0].DataLabels.ShowPercentage);
        }
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


