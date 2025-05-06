---
title: XlsSaveOptions.LightCellsDataProvider
second_title: Aspose.Cells for .NET API Reference
description: XlsSaveOptions property. The data provider for saving workbook in light mode
type: docs
url: /net/aspose.cells/xlssaveoptions/lightcellsdataprovider/
---
## XlsSaveOptions.LightCellsDataProvider property

The data provider for saving workbook in light mode.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Examples

```csharp
// Called: sopts.LightCellsDataProvider = new LightCellsDataProviderN55651();
[Test]
        public void Property_LightCellsDataProvider()
        {
            Workbook wb = new Workbook();
            XlsSaveOptions sopts = new XlsSaveOptions();
            sopts.LightCellsDataProvider = new LightCellsDataProviderN55651();
            Util.SaveManCheck(wb, &quot;&quot;, &quot;N55651_TruncatedValue.xls&quot;, sopts);
            sopts.LightCellsDataProvider = new LightCellsDataProviderN55651();
            wb = Util.ReSave(wb, sopts, new LoadOptions());
            //Ms excel truncates the LABEL record to 255 characters. But we do not, here the value we read is same with the exprected.
            Cells cells = wb.Worksheets[0].Cells;
            Assert.AreEqual(257, cells[1, 0].StringValue.Length, &quot;String length saved with LightCells&quot;);
            Assert.AreEqual(8217, cells[3, 0].StringValue.Length, &quot;String length saved with LightCells&quot;);
        }
```

### See Also

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


