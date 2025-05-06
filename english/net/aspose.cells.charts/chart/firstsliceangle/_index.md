---
title: Chart.FirstSliceAngle
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets or sets the angle of the first piechart or doughnutchart slice in degrees clockwise from vertical. Applies only to pie 3D pie and doughnut charts 0 to 360
type: docs
url: /net/aspose.cells.charts/chart/firstsliceangle/
---
## Chart.FirstSliceAngle property

Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.

```csharp
public int FirstSliceAngle { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(0, chart.FirstSliceAngle);
[Test]
        public void Property_FirstSliceAngle()
        {
            var workbook = new Workbook(Path.Combine(Constants.sourcePath, &quot;CELLSJAVA45298_1.xlsx&quot;));
            Chart chart1 = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(0,chart1.FirstSliceAngle);
            workbook.Save(Constants.destPath + &quot;CELLSJAVA45298_1.ods&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSJAVA45298_1.ods&quot;);
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(0, chart.FirstSliceAngle);
            workbook.Save(Constants.destPath + &quot;CELLSJAVA45298_1.xlsx&quot;);
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


