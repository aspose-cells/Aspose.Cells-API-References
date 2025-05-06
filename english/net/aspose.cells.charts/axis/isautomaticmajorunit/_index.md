---
title: Axis.IsAutomaticMajorUnit
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Indicates whether the major unit of the axis is automatically assigned
type: docs
url: /net/aspose.cells.charts/axis/isautomaticmajorunit/
---
## Axis.IsAutomaticMajorUnit property

Indicates whether the major unit of the axis is automatically assigned.

```csharp
public bool IsAutomaticMajorUnit { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(!chart.CategoryAxis.IsAutomaticMajorUnit, &amp;quot;Is Automatic Major Unit&amp;quot;);
[Test]
        public void Property_IsAutomaticMajorUnit()
        {
            var workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET-51016.xlsx&quot;);
            workbook.Save(Constants.destPath + &quot;CELLSNET-51016_Resave.xlsx&quot;);
            workbook = new Workbook(workbook.FileName);
            var chart = workbook.Worksheets[0].Charts[0];
            Assert.IsTrue(!chart.CategoryAxis.IsAutomaticMajorUnit, &quot;Is Automatic Major Unit&quot;);
            Assert.AreEqual(chart.CategoryAxis.MajorUnitScale, TimeUnit.Days, &quot;Major Unit Scale&quot;);
        }
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


