---
title: DataLabels.SeparatorType
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets or sets the separator type used for the data labels on a chart
type: docs
url: /net/aspose.cells.charts/datalabels/separatortype/
---
## DataLabels.SeparatorType property

Gets or sets the separator type used for the data labels on a chart.

```csharp
public DataLabelsSeparatorType SeparatorType { get; set; }
```

### Remarks

To set custom separator, please set the property `SeparatorType` as Custom and then specify the expected value for [`SeparatorValue`](../separatorvalue/).

### Examples

```csharp
// Called: AssertHelper.AreEqual(DataLabelsSeparatorType.Auto, chart.NSeries[0].DataLabels.SeparatorType, &amp;quot;chart.NSeries[0].DataLabels.Separator&amp;quot;);
private void Property_SeparatorType(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(DataLabelsSeparatorType.Auto, chart.NSeries[0].DataLabels.SeparatorType, &quot;chart.NSeries[0].DataLabels.Separator&quot;);
        }
```

### See Also

* enum [DataLabelsSeparatorType](../../datalabelsseparatortype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


