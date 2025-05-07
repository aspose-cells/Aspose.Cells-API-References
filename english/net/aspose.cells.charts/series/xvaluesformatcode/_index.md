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
// Called: Assert.AreEqual("M/d/yyyy",chart.NSeries[0].XValuesFormatCode);
[Test]
        public void Property_XValuesFormatCode()
        {
            Workbook wb = new Workbook(Constants.PivotTableSourcePath + "CellsJava41156.xlsx");
            wb.Worksheets.RefreshAll();
            Chart chart = wb.Worksheets[0].Charts[0];
            
          //  chart = wb.Worksheets["Sheet1"].Charts[0];
            Assert.AreEqual("M/d/yyyy",chart.NSeries[0].XValuesFormatCode);
     
        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


