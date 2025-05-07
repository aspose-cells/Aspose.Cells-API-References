---
title: ChartCollection.RemoveAt
second_title: Aspose.Cells for .NET API Reference
description: ChartCollection method. Remove a chart at the specific index
type: docs
url: /net/aspose.cells.charts/chartcollection/removeat/
---
## ChartCollection.RemoveAt method

Remove a chart at the specific index.

```csharp
public void RemoveAt(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The chart index. |

### Examples

```csharp
// Called: sheet.Charts.RemoveAt(0);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "TestGridline_001.xls");
            Worksheet sheet = workbook.Worksheets[0];
            int chartCount = sheet.Charts.Count;
            int shapesCount = sheet.Shapes.Count;
            sheet.Charts.RemoveAt(0);
            Assert.AreEqual(chartCount, sheet.Charts.Count + 1);
            Assert.AreEqual(shapesCount, sheet.Shapes.Count + 1);
        }
```

### See Also

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


