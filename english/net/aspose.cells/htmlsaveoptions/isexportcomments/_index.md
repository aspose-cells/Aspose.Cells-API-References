---
title: HtmlSaveOptions.IsExportComments
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates if exporting comments when saving file to html the default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/isexportcomments/
---
## HtmlSaveOptions.IsExportComments property

Indicates if exporting comments when saving file to html, the default value is false.

```csharp
public bool IsExportComments { get; set; }
```

### Examples

```csharp
// Called: IsExportComments = false,
public void HtmlSaveOptions_Property_IsExportComments()
{
            
    var options = new HtmlSaveOptions
    {
        ExportImagesAsBase64 = true,
        IsExportComments = false,
        ExportHiddenWorksheet = false,
        HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove,
        HiddenColDisplayType = HtmlHiddenColDisplayType.Remove,
        ExportGridLines = true
    };

    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    wb.Save(_destFilesPath + "example.html", options);
    string text = File.ReadAllText(_destFilesPath + "example.html");
    Assert.IsTrue(text.IndexOf("z-index:1;margin-left:5px;margin-top:2px;width:443px;height:286px'") != -1);
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


