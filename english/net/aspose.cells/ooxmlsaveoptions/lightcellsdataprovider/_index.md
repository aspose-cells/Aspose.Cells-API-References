---
title: OoxmlSaveOptions.LightCellsDataProvider
second_title: Aspose.Cells for .NET API Reference
description: OoxmlSaveOptions property. The data provider for saving workbook in light mode
type: docs
url: /net/aspose.cells/ooxmlsaveoptions/lightcellsdataprovider/
---
## OoxmlSaveOptions.LightCellsDataProvider property

The data provider for saving workbook in light mode.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Examples

```csharp
// Called: optsO.LightCellsDataProvider = new LightCellsDataProviderStyle();
[Test]
        public void Property_LightCellsDataProvider()
        {
            Workbook wb = StyleCreateWorkbook();
            int styleCount = wb.CountOfStylesInPool;
            OoxmlSaveOptions optsO = new OoxmlSaveOptions();
            optsO.LightCellsDataProvider = new LightCellsDataProviderStyle();
            string fn = Constants.destPath + &quot;LightCellsVerify.xlsx&quot;;
            wb.Save(fn, optsO);
            StyleCheckOriginal(wb, &quot;After saving to XLSX: &quot;, styleCount);
            string fn1 = Constants.destPath + &quot;LightCellsAfterSave.xlsx&quot;;
            wb.Save(fn1);
            wb = new Workbook(fn1);
            StyleCheckOriginal(wb, &quot;Resave to XLSX: &quot;, styleCount);
            wb = new Workbook(fn);
            StyleVerifyWorkbook(wb, &quot;XLSX-&quot;);
            //check string pool in debug mode here.

            wb = StyleCreateWorkbook();
            XlsSaveOptions optsS = new XlsSaveOptions();
            optsS.LightCellsDataProvider = new LightCellsDataProviderStyle();
            fn = Constants.destPath + &quot;LightCellsVerify.xls&quot;;
            wb.Save(fn, optsS);
            StyleCheckOriginal(wb, &quot;After saving to XLS: &quot;, styleCount);
            fn1 = Constants.destPath + &quot;LightCellsAfterSave.xls&quot;;
            wb.Save(fn1);
            wb = new Workbook(fn1);
            StyleCheckOriginal(wb, &quot;Resave to XLS: &quot;, styleCount);
            wb = new Workbook(fn);
            StyleVerifyWorkbook(wb, &quot;XLS-&quot;);
            //check string pool in debug mode here.
        }
```

### See Also

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


