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
// Called: Assert.AreEqual(chart.NSeries[0].Points[3].DataLabels.ShowPercentage, true);
[Test]
        public void Property_ShowPercentage()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;test_176617.xlt&quot;);
            Chart chart = workbook.Worksheets[0].Charts[1];
            Aspose.Cells.Cells cells = workbook.Worksheets[0].Cells;
            cells[&quot;C32&quot;].PutValue(1);
            cells[&quot;C33&quot;].PutValue(1);
            Assert.AreEqual(chart.NSeries[0].Points[3].DataLabels.ShowPercentage, true);
            workbook.Save(Constants.destPath + &quot;Test_176617.xls&quot;);
        }
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


