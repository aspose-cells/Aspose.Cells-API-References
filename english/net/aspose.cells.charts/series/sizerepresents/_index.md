---
title: Series.SizeRepresents
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets or sets what the bubble size represents on a bubble chart
type: docs
url: /net/aspose.cells.charts/series/sizerepresents/
---
## Series.SizeRepresents property

Gets or sets what the bubble size represents on a bubble chart.

```csharp
public BubbleSizeRepresents SizeRepresents { get; set; }
```

### Remarks

BubbleSizeRepresents.SizeIsArea means the value [`BubbleSizes`](../bubblesizes/) is the area of the bubble. BubbleSizeRepresents.SizeIsWidth means the value [`BubbleSizes`](../bubblesizes/) is the width of the bubble.

### Examples

```csharp
// Called: AssertHelper.AreEqual(BubbleSizeRepresents.SizeIsArea, chart.NSeries[0].SizeRepresents, &amp;quot;chart.NSeries[0].SizeRepresents&amp;quot;);
private void Property_SizeRepresents(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(BubbleSizeRepresents.SizeIsArea, chart.NSeries[0].SizeRepresents, &quot;chart.NSeries[0].SizeRepresents&quot;);
        }
```

### See Also

* enum [BubbleSizeRepresents](../../bubblesizerepresents/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


