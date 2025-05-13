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
public void Axis_Method_GetAxisTexts()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Chart chart = workbook.Worksheets[0].Charts[0];
    chart.Calculate();
    var labels = chart.ValueAxis.GetAxisTexts();
    Assert.AreEqual(9, labels.Length, "ValueAxis Labels Count");
    Assert.AreEqual(labels[0], "8000", "Max axis label");
    Assert.AreEqual(labels[8], "-8000", "Min axis label");
}
```

### See Also

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


