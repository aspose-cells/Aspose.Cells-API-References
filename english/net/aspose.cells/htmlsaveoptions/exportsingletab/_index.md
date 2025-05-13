---
title: HtmlSaveOptions.ExportSingleTab
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether exporting the single tab when the file only has one worksheet. The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportsingletab/
---
## HtmlSaveOptions.ExportSingleTab property

Indicates whether exporting the single tab when the file only has one worksheet. The default value is false.

```csharp
public bool ExportSingleTab { get; set; }
```

### Examples

```csharp
// Called: ExportSingleTab = true,
public void HtmlSaveOptions_Property_ExportSingleTab()
{
    string filePath = Constants.HtmlPath + @"NET48191/";
    HtmlSaveOptions options = new HtmlSaveOptions
    {
        ExportImagesAsBase64 = true,
        ExportSingleTab = true,
        IsExportComments = false,
        ExportHiddenWorksheet = false,
        HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove,
        HiddenColDisplayType = HtmlHiddenColDisplayType.Remove,
        ExportGridLines = true
    };

    Workbook wb = new Workbook(filePath + "SourceFile.xlsx");
    wb.Save(_destFilesPath + "example.html", options);

    string content = File.ReadAllText(_destFilesPath + "NET48191_files/sheet001.htm");
    Assert.IsTrue(content.IndexOf("<span style='display:none'>") == -1);
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


