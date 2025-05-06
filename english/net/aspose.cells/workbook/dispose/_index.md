---
title: Workbook.Dispose
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Performs applicationdefined tasks associated with freeing releasing or resetting unmanaged resources
type: docs
url: /net/aspose.cells/workbook/dispose/
---
## Workbook.Dispose method

Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

```csharp
public void Dispose()
```

### Examples

```csharp
// Called: wb.Dispose();
private void Method_Dispose(string plugin, SaveOptions saveOptions)
        {
            string ext = FileFormatUtil.SaveFormatToExtension(saveOptions.SaveFormat);
            string evalmarker = saveOptions.SaveFormat == SaveFormat.Pdf
                ? &quot;Eval water marker&quot; : &quot;Extra eval sheet&quot;;
            Workbook wb = GetTestWorkbook(evalmarker + &quot; should be ADDED. Next line should be \&quot;Value BEFORE calculation\&quot;.&quot;);
            Workbook wbExcluded = Util.ReSave(wb, SaveFormat.Xlsx);
            wb.Dispose();
            wb = GetTestWorkbook(evalmarker + &quot; should NOT be added. Next line should be \&quot;Value BEFORE calculation\&quot;.&quot;);
            Workbook wbLicensed = Util.ReSave(wb, SaveFormat.Xlsx);
            wb.Dispose();
            wb = GetTestWorkbook(evalmarker + &quot; should be ADDED. Next line should be \&quot;Value AFTER calculation\&quot;.&quot;);
            Workbook wbChanged = Util.ReSave(wb, SaveFormat.Xlsx);
            wb.Dispose();

            SetExclude(plugin);
            Util.SaveManCheck(wbExcluded, &quot;License&quot;, &quot;Plugin&quot; + plugin + &quot;Excluded&quot; + ext, saveOptions);
            wbExcluded.Dispose();

            SetLicense(plugin);
            Util.SaveManCheck(wbLicensed, &quot;License&quot;, &quot;Plugin&quot; + plugin + &quot;Licensed&quot; + ext, saveOptions);
            wbLicensed.Dispose();

            wbChanged.CalculateFormula();
            Util.SaveManCheck(wbChanged, &quot;License&quot;, &quot;Plugin&quot; + plugin + &quot;Changed&quot; + ext, saveOptions);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


