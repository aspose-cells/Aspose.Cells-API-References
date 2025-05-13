---
title: Legend.LegendEntries
second_title: Aspose.Cells for .NET API Reference
description: Legend property. Gets a collection of all the LegendEntry objects in the specified chart legend. Setting the legend entries of the surface chart is not supported. So it will return null if the chart type is surface chart type
type: docs
url: /net/aspose.cells.charts/legend/legendentries/
---
## Legend.LegendEntries property

Gets a collection of all the LegendEntry objects in the specified chart legend. Setting the legend entries of the surface chart is not supported. So it will return null if the chart type is surface chart type.

```csharp
public LegendEntryCollection LegendEntries { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[4].Charts[0].Legend.LegendEntries[3].IsDeleted, true);
public void Legend_Property_LegendEntries()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    workbook.Worksheets.AddCopy(0);
    Assert.AreEqual(workbook.Worksheets[4].Charts[0].Legend.LegendEntries[3].IsDeleted, true);
    Assert.AreEqual(workbook.Worksheets[4].Charts[0].CategoryAxis.MajorUnitScale, TimeUnit.Months);
}
```

### See Also

* class [LegendEntryCollection](../../legendentrycollection/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


