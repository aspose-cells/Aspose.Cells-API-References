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
// Called: Assert.IsTrue(!chart.CategoryAxis.IsAutomaticMajorUnit, "Is Automatic Major Unit");
[Test]
        public void Property_IsAutomaticMajorUnit()
        {
            var workbook = new Workbook(Constants.sourcePath + "CELLSNET-51016.xlsx");
            workbook.Save(Constants.destPath + "CELLSNET-51016_Resave.xlsx");
            workbook = new Workbook(workbook.FileName);
            var chart = workbook.Worksheets[0].Charts[0];
            Assert.IsTrue(!chart.CategoryAxis.IsAutomaticMajorUnit, "Is Automatic Major Unit");
            Assert.AreEqual(chart.CategoryAxis.MajorUnitScale, TimeUnit.Days, "Major Unit Scale");
        }
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


