---
title: ChartCollection.Clear
second_title: Aspose.Cells for .NET API Reference
description: ChartCollection method. Clear all charts
type: docs
url: /net/aspose.cells.charts/chartcollection/clear/
---
## ChartCollection.Clear method

Clear all charts.

```csharp
public void Clear()
```

### Examples

```csharp
// Called: workbook.Worksheets[0].Charts.Clear();
[Test]
        public void Method_Clear()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Test_145192.xls");
            workbook.Worksheets[0].Charts.Clear();
            workbook.Worksheets[0].Charts.Add(ChartType.Column, 5, 5, 15, 10);
        }
```

### See Also

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


