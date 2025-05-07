---
title: PivotOptions.DropZoneCategories
second_title: Aspose.Cells for .NET API Reference
description: PivotOptions property. Specifies whether a control for each PivotTable field on the PivotTable row axis of the source PivotTable appears on the chart when dropZonesVisible is set to true
type: docs
url: /net/aspose.cells.charts/pivotoptions/dropzonecategories/
---
## PivotOptions.DropZoneCategories property

Specifies whether a control for each PivotTable field on the PivotTable row axis of the source PivotTable appears on the chart when dropZonesVisible is set to true.

```csharp
public bool DropZoneCategories { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(options.DropZoneCategories);
[Test]
        public void Property_DropZoneCategories()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet43845.xlsm");
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


