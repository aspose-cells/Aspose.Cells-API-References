---
title: Series.Values
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents the Y values of this chart series
type: docs
url: /net/aspose.cells.charts/series/values/
---
## Series.Values property

Represents the Y values of this chart series.

```csharp
public string Values { get; set; }
```

### Examples

```csharp
// Called: testAreEqual("=Sheet1!$B$2:$B$4", chart.NSeries[0].Values, caseName);
private void Series_Property_Values(Workbook workbook)
        {
            Chart chart = workbook.Worksheets[0].Charts[0];
            testAreEqual("=Sheet1!$B$2:$B$4", chart.NSeries[0].Values, caseName);
            testAreEqual("=Sheet1!$C$2:$C$4", chart.NSeries[1].Values, caseName);
        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


