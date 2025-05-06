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
// Called: Assert.AreEqual(workbook.Worksheets[2].Charts[0].NSeries[0].Values, workbook.Worksheets[0].Charts[0].NSeries[0].Values);
[Test]
        public void Property_Values()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;ChartsUpdateOtherRef.xls&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            cells.InsertColumn(0, true);
            cells.InsertRows(0, 10, true);
            cells.DeleteColumn(0, true);
            cells.DeleteRows(0, 5, true);
           // 
            Assert.AreEqual(workbook.Worksheets[2].Charts[0].NSeries[0].Values, workbook.Worksheets[0].Charts[0].NSeries[0].Values);
            workbook.Save(Constants.destPath + &quot;ChartsUpdateOtherRef.xls&quot;);
        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


