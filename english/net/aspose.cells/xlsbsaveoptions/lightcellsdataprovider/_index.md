---
title: XlsbSaveOptions.LightCellsDataProvider
second_title: Aspose.Cells for .NET API Reference
description: XlsbSaveOptions property. The data provider for saving workbook in light mode
type: docs
url: /net/aspose.cells/xlsbsaveoptions/lightcellsdataprovider/
---
## XlsbSaveOptions.LightCellsDataProvider property

The data provider for saving workbook in light mode.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Examples

```csharp
// Called: optsB.LightCellsDataProvider = new LightCellsDataProviderString();
private void Property_LightCellsDataProvider(bool mem)
        {
            Workbook wb = GetWorkbookForString(mem);
            OoxmlSaveOptions optsO = new OoxmlSaveOptions();
            optsO.LightCellsDataProvider = new LightCellsDataProviderString();
            MemoryStream ms = new MemoryStream(32768);
            wb.Save(ms, optsO);
            ms.Seek(0, SeekOrigin.Begin);
            wb = new Workbook(ms);
            StringVerifyWorkbook(wb, &quot;XLSX-&quot; + (mem ? &quot;M&quot; : &quot;N&quot;) + &quot;-&quot;);
            wb = GetWorkbookForString(mem);
            XlsSaveOptions optsS = new XlsSaveOptions();
            optsS.LightCellsDataProvider = new LightCellsDataProviderString();
            wb.Save(ms, optsS);
            ms.Seek(0, SeekOrigin.Begin);
            wb = new Workbook(ms);
            StringVerifyWorkbook(wb, &quot;XLS-&quot; + (mem ? &quot;M&quot; : &quot;N&quot;) + &quot;-&quot;);
            XlsbSaveOptions optsB = new XlsbSaveOptions();
            optsB.LightCellsDataProvider = new LightCellsDataProviderString();
            wb.Save(ms, optsB);
            ms.Seek(0, SeekOrigin.Begin);
            wb = new Workbook(ms);
            StringVerifyWorkbook(wb, &quot;XLSB-&quot; + (mem ? &quot;M&quot; : &quot;N&quot;) + &quot;-&quot;);
        }
```

### See Also

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


