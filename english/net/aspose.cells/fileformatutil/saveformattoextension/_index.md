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
                ? "Eval water marker" : "Extra eval sheet";
            Workbook wb = GetTestWorkbook(evalmarker + " should be ADDED. Next line should be \"Value BEFORE calculation\".");
            Workbook wbExcluded = Util.ReSave(wb, SaveFormat.Xlsx);
            wb.Dispose();
            wb = GetTestWorkbook(evalmarker + " should NOT be added. Next line should be \"Value BEFORE calculation\".");
            Workbook wbLicensed = Util.ReSave(wb, SaveFormat.Xlsx);
            wb.Dispose();
            wb = GetTestWorkbook(evalmarker + " should be ADDED. Next line should be \"Value AFTER calculation\".");
            Workbook wbChanged = Util.ReSave(wb, SaveFormat.Xlsx);
            wb.Dispose();

            SetExclude(plugin);
            Util.SaveManCheck(wbExcluded, "License", "Plugin" + plugin + "Excluded" + ext, saveOptions);
            wbExcluded.Dispose();

            SetLicense(plugin);
            Util.SaveManCheck(wbLicensed, "License", "Plugin" + plugin + "Licensed" + ext, saveOptions);
            wbLicensed.Dispose();

            wbChanged.CalculateFormula();
            Util.SaveManCheck(wbChanged, "License", "Plugin" + plugin + "Changed" + ext, saveOptions);
        }
```

### See Also

* enum [SaveFormat](../../saveformat/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


