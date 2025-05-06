---
title: Axis.DisplayUnitLabel
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values for example in the millions or billions
type: docs
url: /net/aspose.cells.charts/axis/displayunitlabel/
---
## Axis.DisplayUnitLabel property

Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values— for example, in the millions or billions.

```csharp
public DisplayUnitLabel DisplayUnitLabel { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.ValueAxis.DisplayUnitLabel.RotationAngle, 0);
[Test]
        public void Property_DisplayUnitLabel()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET40620.xlsx&quot;);
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.ValueAxis.DisplayUnitLabel.RotationAngle, 0);
            
        }
```

### See Also

* class [DisplayUnitLabel](../../displayunitlabel/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


