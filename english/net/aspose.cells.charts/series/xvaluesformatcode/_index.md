---
title: Series.XValuesFormatCode
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents format code of X Valuess NumberList
type: docs
url: /net/aspose.cells.charts/series/xvaluesformatcode/
---
## Series.XValuesFormatCode property

Represents format code of X Values's NumberList.

```csharp
public string XValuesFormatCode { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;M/d/yyyy&amp;quot;,chart.NSeries[0].XValuesFormatCode);
[Test]
        public void Property_XValuesFormatCode()
        {
            Workbook wb = new Workbook(Constants.PivotTableSourcePath + &quot;CellsJava41156.xlsx&quot;);
            wb.Worksheets.RefreshAll();
            Chart chart = wb.Worksheets[0].Charts[0];
            
          //  chart = wb.Worksheets[&quot;Sheet1&quot;].Charts[0];
            Assert.AreEqual(&quot;M/d/yyyy&quot;,chart.NSeries[0].XValuesFormatCode);
     
        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


