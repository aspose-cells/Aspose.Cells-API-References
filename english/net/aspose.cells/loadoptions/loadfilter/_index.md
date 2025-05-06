---
title: LoadOptions.LoadFilter
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. The filter to denote how to load data
type: docs
url: /net/aspose.cells/loadoptions/loadfilter/
---
## LoadOptions.LoadFilter property

The filter to denote how to load data.

```csharp
public LoadFilter LoadFilter { get; set; }
```

### Examples

```csharp
// Called: opts.LoadFilter = lf;
[Test]
        public void Property_LoadFilter()
        {
            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells[0, 0].PutValue(0);
            wb.Worksheets.Add(&quot;Sheet2&quot;).Cells[0, 0].PutValue(1);
            wb.Worksheets.Add(&quot;Sheet3&quot;).Cells[0, 0].PutValue(2);
            LoadOptions opts = new LoadOptions();
            LoadFilterOrder lf = new LoadFilterOrder();
            opts.LoadFilter = lf;
            opts.LightCellsDataHandler = lf;
            lf.Reset(&quot;Xls&quot;);
            wb = Util.ReSave(wb, new XlsSaveOptions(), opts);
            lf.Verify();
            lf.Reset(&quot;Xlsx&quot;);
            wb = Util.ReSave(wb, new OoxmlSaveOptions(), opts);
            lf.Verify();
        }
```

### See Also

* class [LoadFilter](../../loadfilter/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


