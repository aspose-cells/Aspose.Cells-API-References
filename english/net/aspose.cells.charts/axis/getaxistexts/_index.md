---
title: Axis.GetAxisTexts
second_title: Aspose.Cells for .NET API Reference
description: Axis method. Gets the labels of the axis after call Chart.Calculate method
type: docs
url: /net/aspose.cells.charts/axis/getaxistexts/
---
## Axis.GetAxisTexts method

Gets the labels of the axis after call Chart.Calculate() method.

```csharp
public string[] GetAxisTexts()
```

### Examples

```csharp
// Called: var labels = chart.ValueAxis.GetAxisTexts();
[Test]
        public void Method_GetAxisTexts()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET-48049.xlsx");
            var chart = workbook.Worksheets[0].Charts[0];
            chart.Calculate();
            var labels = chart.ValueAxis.GetAxisTexts();
            Assert.AreEqual("15,000 ", labels[0], "ValueAxis max value");
        }
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


