---
title: FileFormatUtil.SaveFormatToExtension
second_title: Aspose.Cells for .NET API Reference
description: FileFormatUtil method. Converts a save format enumerated value into a file extension
type: docs
url: /net/aspose.cells/fileformatutil/saveformattoextension/
---
## FileFormatUtil.SaveFormatToExtension method

Converts a save format enumerated value into a file extension.

```csharp
public static string SaveFormatToExtension(SaveFormat format)
```

| Parameter | Type | Description |
| --- | --- | --- |
| format | SaveFormat | The save format. |

### Return Value

The returned extension is a lower-case string with a leading dot.

### Examples

```csharp
// Called: string ext = FileFormatUtil.SaveFormatToExtension(saveOptions.SaveFormat);
private void Method_SaveFormat_(string plugin, SaveOptions saveOptions)
        {
            string ext = FileFormatUtil.SaveFormatToExtension(saveOptions.SaveFormat);
            string evalmarker = saveOptions.SaveFormat == SaveFormat.Pdf
                ? &quot;Water marker&quot; : &quot;Extra eval sheet&quot;;
            Workbook wb = GetTestWorkbook(evalmarker + &quot; should be ADDED. Next line should be \&quot;Value BEFORE calculation\&quot;.&quot;);
            Stream streamExcluded = Util.SaveAsBuffer(wb, SaveFormat.Xlsx);
            wb.Dispose();
            wb = GetTestWorkbook(evalmarker + &quot; should NOT be added. Next line should be \&quot;Value BEFORE calculation\&quot;.&quot;);
            Stream streamLicensed = Util.SaveAsBuffer(wb, SaveFormat.Xlsx);
            wb.Dispose();

            SetExclude(plugin);
            LicenseTest.CountLimit(false);
            ProcessLowCode(streamExcluded, saveOptions, plugin + &quot;Excluded&quot; + ext);
            streamExcluded = null;

            SetLicense(plugin);
            ProcessLowCode(streamLicensed, saveOptions, plugin + &quot;Licensed&quot; + ext);
            streamLicensed = null;
        }
```

### See Also

* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


