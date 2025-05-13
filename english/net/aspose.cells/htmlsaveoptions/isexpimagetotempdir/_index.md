---
title: HtmlSaveOptions.IsExpImageToTempDir
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicates whether exporting image files to temp directory. Only for saving to html stream
type: docs
url: /net/aspose.cells/htmlsaveoptions/isexpimagetotempdir/
---
## HtmlSaveOptions.IsExpImageToTempDir property

Indicates whether exporting image files to temp directory. Only for saving to html stream.

```csharp
public bool IsExpImageToTempDir { get; set; }
```

### Examples

```csharp
// Called: options.IsExpImageToTempDir = true;
public void HtmlSaveOptions_Property_IsExpImageToTempDir()
{
    string filePath = Constants.JohnTest_PATH_SOURCE + @"NET48085/";
    string savePath = CreateFolder(filePath);

    Workbook wb = new Workbook(filePath + "Hidden table header.xlsx");
    wb.Worksheets.ActiveSheetIndex = 0;

    HtmlSaveOptions options = new HtmlSaveOptions();
    options.ExportActiveWorksheetOnly = true;
    options.ExportDataOptions = HtmlExportDataOptions.All;
    options.IsExpImageToTempDir = true;
    options.ExportHeadings = true;
    options.ExportExtraHeadings = true;
    options.ExportGridLines = true;

    wb.Save(savePath + "out.html", options);
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


