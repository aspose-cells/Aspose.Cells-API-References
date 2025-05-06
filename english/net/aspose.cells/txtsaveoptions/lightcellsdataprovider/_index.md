---
title: TxtSaveOptions.LightCellsDataProvider
second_title: Aspose.Cells for .NET API Reference
description: TxtSaveOptions property. The data provider for saving workbook in light mode
type: docs
url: /net/aspose.cells/txtsaveoptions/lightcellsdataprovider/
---
## TxtSaveOptions.LightCellsDataProvider property

The data provider for saving workbook in light mode.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Examples

```csharp
// Called: LightCellsDataProvider = new LightCellsDataProviderJ43341(),
[Test]
        public void Property_LightCellsDataProvider()
        {
            Assert.AreEqual(&quot;,,v_2_2,v_2_3,v_2_4\r\n,,v_3_2,v_3_3,v_3_4\r\n,,v_4_2,v_4_3,v_4_4\r\n&quot;,
                CSVTest.SaveAsCsv(new Workbook(), new TxtSaveOptions()
                {
                    Encoding = Encoding.ASCII,
                    LightCellsDataProvider = new LightCellsDataProviderJ43341(),
                }));
        }
```

### See Also

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


