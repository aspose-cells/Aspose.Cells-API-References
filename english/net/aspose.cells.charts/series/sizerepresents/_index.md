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
// Called: AssertHelper.AreEqual(BubbleSizeRepresents.SizeIsArea, chart.NSeries[0].SizeRepresents, "chart.NSeries[0].SizeRepresents");
private void Series_Property_SizeRepresents(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet1"];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(BubbleSizeRepresents.SizeIsArea, chart.NSeries[0].SizeRepresents, "chart.NSeries[0].SizeRepresents");
        }
```

### See Also

* enum [BubbleSizeRepresents](../../bubblesizerepresents/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


