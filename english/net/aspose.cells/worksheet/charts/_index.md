---
title: Worksheet.Charts
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets a Chart collection
type: docs
url: /net/aspose.cells/worksheet/charts/
---
## Worksheet.Charts property

Gets a [`Chart`](../../../aspose.cells.charts/chart/) collection

```csharp
public ChartCollection Charts { get; }
```

### Examples

```csharp
// Called: chart = workbook.Worksheets["Sheet2"].Charts[0];
private void Property_Charts(Workbook workbook)
        {
            Chart chart = workbook.Worksheets["Sheet1"].Charts[0];
            testAreEqual("=Sheet1!$E$3:$E$19", chart.NSeries[0].Values, caseName);
            testAreEqual("=Sheet1!$D$3:$D$19", chart.NSeries.CategoryData, caseName);

            chart = workbook.Worksheets["Chart1"].Charts[0];
            testAreEqual("=Sheet1!$B$1:$B$17", chart.NSeries[0].Values, caseName);
            testAreEqual("=Sheet1!$A$1:$A$17", chart.NSeries.CategoryData, caseName);

            chart = workbook.Worksheets["Sheet2"].Charts[0];
            testAreEqual("=Sheet1!$B$1:$B$17", chart.NSeries[0].Values, caseName);
            testAreEqual("=Sheet1!$A$1:$A$17", chart.NSeries.CategoryData, caseName);
        }
```

### See Also

* class [ChartCollection](../../../aspose.cells.charts/chartcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


