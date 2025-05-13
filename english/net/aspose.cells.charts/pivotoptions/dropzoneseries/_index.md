---
title: PivotOptions.DropZoneSeries
second_title: Aspose.Cells for .NET API Reference
description: PivotOptions property. Specifies whether a control for each PivotTable field on the PivotTable column axis of the source PivotTable appears on the chart when dropZonesVisible is set to true
type: docs
url: /net/aspose.cells.charts/pivotoptions/dropzoneseries/
---
## PivotOptions.DropZoneSeries property

Specifies whether a control for each PivotTable field on the PivotTable column axis of the source PivotTable appears on the chart when dropZonesVisible is set to true.

```csharp
public bool DropZoneSeries { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(options.DropZoneSeries);
public void PivotOptions_Property_DropZoneSeries()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsm");
    PivotOptions options = workbook.Worksheets[0].Charts[1].PivotOptions;
    Assert.IsFalse(options.DropZoneCategories);
    Assert.IsFalse(options.DropZoneData);
    Assert.IsFalse(options.DropZoneSeries);
}
```

### See Also

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


