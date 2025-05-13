---
title: ChartTextFrame.LinkedSource
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame property. Gets and sets a reference to the worksheet
type: docs
url: /net/aspose.cells.charts/charttextframe/linkedsource/
---
## ChartTextFrame.LinkedSource property

Gets and sets a reference to the worksheet.

```csharp
public virtual string LinkedSource { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("='1.3 - Graph II'!$P$1", chart.Title.LinkedSource);
public void ChartTextFrame_Property_LinkedSource()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Chart chart = workbook.Worksheets["1.3 - Graph II"].Charts[0];
    Assert.AreEqual("='1.3 - Graph II'!$P$1", chart.Title.LinkedSource);

}
```

### See Also

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


