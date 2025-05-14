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
private void FileFormatUtil_Method_SaveFormatToExtension(string plugin, SaveOptions saveOptions)
        {
            string ext = FileFormatUtil.SaveFormatToExtension(saveOptions.SaveFormat);
            string evalmarker = saveOptions.SaveFormat == SaveFormat.Pdf
                ? "Water marker" : "Extra eval sheet";
            Workbook wb = GetTestWorkbook(evalmarker + " should be ADDED. Next line should be \"Value BEFORE calculation\".");
            Stream streamExcluded = Util.SaveAsBuffer(wb, SaveFormat.Xlsx);
            wb.Dispose();
            wb = GetTestWorkbook(evalmarker + " should NOT be added. Next line should be \"Value BEFORE calculation\".");
            Stream streamLicensed = Util.SaveAsBuffer(wb, SaveFormat.Xlsx);
            wb.Dispose();

            SetExclude(plugin);
            LicenseTest.CountLimit(false);
            ProcessLowCode(streamExcluded, saveOptions, plugin + "Excluded" + ext);
            streamExcluded = null;

            SetLicense(plugin);
            ProcessLowCode(streamLicensed, saveOptions, plugin + "Licensed" + ext);
            streamLicensed = null;
        }
```

### See Also

* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


