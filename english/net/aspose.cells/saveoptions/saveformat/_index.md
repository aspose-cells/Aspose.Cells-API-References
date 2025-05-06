---
title: SaveOptions.SaveFormat
second_title: Aspose.Cells for .NET API Reference
description: SaveOptions property. Gets the save file format
type: docs
url: /net/aspose.cells/saveoptions/saveformat/
---
## SaveOptions.SaveFormat property

Gets the save file format.

```csharp
public SaveFormat SaveFormat { get; }
```

### Examples

```csharp
// Called: string ext = FileFormatUtil.SaveFormatToExtension(saveOptions.SaveFormat);
private void Property_SaveFormat(string plugin, SaveOptions saveOptions)
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
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


