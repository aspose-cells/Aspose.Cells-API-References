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
// Called: chart.NSeries[0].SizeRepresents = BubbleSizeRepresents.SizeIsWidth;
[Test]
        public void Property_SizeRepresents()
        {
            Workbook workbook = new Workbook();
            workbook = TestBubble.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.NSeries[0].SizeRepresents = BubbleSizeRepresents.SizeIsWidth;

            checkBubbleSizeRepresents_SizeIsWidth(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkBubbleSizeRepresents_SizeIsWidth(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkBubbleSizeRepresents_SizeIsWidth(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* enum [BubbleSizeRepresents](../../bubblesizerepresents/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


