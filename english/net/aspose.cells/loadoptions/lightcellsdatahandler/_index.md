---
title: LoadOptions.LightCellsDataHandler
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. The data handler for processing cells data when reading template file
type: docs
url: /net/aspose.cells/loadoptions/lightcellsdatahandler/
---
## LoadOptions.LightCellsDataHandler property

The data handler for processing cells data when reading template file.

```csharp
public LightCellsDataHandler LightCellsDataHandler { get; set; }
```

### Examples

```csharp
// Called: new LoadOptions() { LightCellsDataHandler = new LightCellsDataHandlerNone() });
[Test]
        public void Property_LightCellsDataHandler()
        {
            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells[0, 1].PutValue("abc");
            wb = Util.ReSave(wb, new XlsbSaveOptions(),
                new LoadOptions() { LightCellsDataHandler = new LightCellsDataHandlerNone() });
            Assert.AreEqual(1, wb.Worksheets[0].Cells.MaxColumn, "MaxColumn by LightCells for Xlsb");
        }
```

### See Also

* interface [LightCellsDataHandler](../../lightcellsdatahandler/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


