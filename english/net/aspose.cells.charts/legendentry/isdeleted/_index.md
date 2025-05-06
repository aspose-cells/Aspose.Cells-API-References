---
title: LegendEntry.IsDeleted
second_title: Aspose.Cells for .NET API Reference
description: LegendEntry property. Gets and sets whether the legend entry is deleted
type: docs
url: /net/aspose.cells.charts/legendentry/isdeleted/
---
## LegendEntry.IsDeleted property

Gets and sets whether the legend entry is deleted.

```csharp
public bool IsDeleted { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[4].Charts[0].Legend.LegendEntries[3].IsDeleted, true);
[Test]
        public void Property_IsDeleted()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA41038.xlsx&quot;);
            workbook.Worksheets.AddCopy(0);
            Assert.AreEqual(workbook.Worksheets[4].Charts[0].Legend.LegendEntries[3].IsDeleted, true);
            Assert.AreEqual(workbook.Worksheets[4].Charts[0].CategoryAxis.MajorUnitScale, TimeUnit.Months);
        }
```

### See Also

* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


