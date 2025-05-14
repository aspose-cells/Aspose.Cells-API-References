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
private void SaveOptions_Property_SaveFormat(string plugin, SaveOptions saveOptions)
        {
            string ext = FileFormatUtil.SaveFormatToExtension(saveOptions.SaveFormat);
            string evalmarker;
            switch (saveOptions.SaveFormat)
            {
                case SaveFormat.Pdf:
                {
                    evalmarker = "Eval water marker";
                    break;
                }
                case SaveFormat.Csv:
                case SaveFormat.Tsv:
                {
                    evalmarker = "Eval water marker(last line)";
                    break;
                }
                default:
                {
                    evalmarker = "Extra eval sheet";
                    break;
                }
            }
            Workbook wb = GetTestWorkbook(evalmarker + " should be ADDED. Next line should be \"Value BEFORE calculation\".");
            Workbook wbExcluded = Util.ReSave(wb, SaveFormat.Xlsx);
            wb.Dispose();
            wb = GetTestWorkbook(evalmarker + " should NOT be added. Next line should be \"Value BEFORE calculation\".");
            Workbook wbLicensed = Util.ReSave(wb, SaveFormat.Xlsx);
            wbLicensed.Worksheets.ActiveSheetIndex = 0;
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
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


