---
title: OoxmlSaveOptions.OoxmlSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: OoxmlSaveOptions constructor. Creates the options for saving office open xml file
type: docs
url: /net/aspose.cells/ooxmlsaveoptions/ooxmlsaveoptions/
---
## OoxmlSaveOptions() {#constructor}

Creates the options for saving office open xml file.

```csharp
public OoxmlSaveOptions()
```

### Examples

```csharp
// Called: wb = Util.ReSave(wb, new OoxmlSaveOptions(), opts);
[Test]
        public void OoxmlSaveOptions_Constructor()
        {
            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells[0, 0].PutValue(0);
            wb.Worksheets.Add("Sheet2").Cells[0, 0].PutValue(1);
            wb.Worksheets.Add("Sheet3").Cells[0, 0].PutValue(2);
            LoadOptions opts = new LoadOptions();
            LoadFilterOrder lf = new LoadFilterOrder();
            opts.LoadFilter = lf;
            opts.LightCellsDataHandler = lf;
            lf.Reset("Xls");
            wb = Util.ReSave(wb, new XlsSaveOptions(), opts);
            lf.Verify();
            lf.Reset("Xlsx");
            wb = Util.ReSave(wb, new OoxmlSaveOptions(), opts);
            lf.Verify();
        }
```

### See Also

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OoxmlSaveOptions(SaveFormat) {#constructor_1}

Creates the options for saving office open xml file.

```csharp
public OoxmlSaveOptions(SaveFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The file format. It should be one of following types: Xlsx, Xltx, Xlam, Xlsm or Xltm, otherwise the saved format will be set as Xlsx automatically. |

### See Also

* enum [SaveFormat](../../saveformat/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


