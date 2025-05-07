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
// Called: string evalmarker = saveOptions.SaveFormat == SaveFormat.Pdf
private void Property_SaveFormat(string plugin, SaveOptions saveOptions)
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
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


