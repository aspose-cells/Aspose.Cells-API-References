---
title: Chart.Name
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets and sets the name of the chart
type: docs
url: /net/aspose.cells.charts/chart/name/
---
## Chart.Name property

Gets and sets the name of the chart.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: chart.ToImage(Constants.destPath + "Charts/BoxWhisker/Chart" + chart.Name + ".png");
[Test]
        public void Property_Name()
        {
            // for show inner/outlier points and datalabels
            Workbook workbook = new Workbook(Constants.sourcePath + "Charts/BoxWhisker/MyTest.xlsx");
            Worksheet worksheet = workbook.Worksheets["Sheet2"];
            foreach (Chart chart in worksheet.Charts)
            {
                chart.ToImage(Constants.destPath + "Charts/BoxWhisker/Chart" + chart.Name + ".png");
            }
            return;
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


